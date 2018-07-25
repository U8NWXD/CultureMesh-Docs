# Minimal makefile for Sphinx documentation
#

# You can set these variables from the command line.
SPHINXOPTS    =
SPHINXBUILD   = sphinx-build
SPHINXPROJ    = CultureMeshAndroid
SOURCEDIR     = source
BUILDDIR      = build

# Constants
# # SOURCE: https://stackoverflow.com/questions/19331073/get-current-branch-name-for-use-in-git-command
GIT_BRANCH = $(git rev-parse --abbrev-ref HEAD)
ANDROID_PATH = ../code/CultureMeshAndroid
ANDROID_DOCS_PATH = source/android
SERVER_PATH = ../code/culturemesh-api
SERVER_DOCS_PATH = source/server

# Put it first so that "make" without argument is like "make help".
help:
	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)

.PHONY: help Makefile

# Generate Javadoc via: Android Studio's javadoc tool and javasphinx-apidoc
# Use Android Studio's javadoc to create javadoc HTML files in source/_static/API-JavaDoc
# Use javasphinx-apidoc to create javadoc .rst files in the docs directory
javadoc: android
	@rm -r source/_static/API-JavaDoc/*
	@"/Applications/Android Studio.app/Contents/jre/jdk/Contents/Home/bin/javadoc" -private -quiet -splitindex -d source/_static/API-JavaDoc -sourcepath $(ANDROID_PATH)/app/src/main/java/ -bootclasspath /Users/cs/Library/Android/sdk/platforms/android-27/android.jar -Xdoclint:none org.codethechange.culturemesh
	@rm -r $(ANDROID_DOCS_PATH)/javadoc/org
	@rm $(ANDROID_DOCS_PATH)/javadoc/packages.rst
	@javasphinx-apidoc -c cache/javasphinx -u -p html5lib -o $(ANDROID_DOCS_PATH)/javadoc/ $(ANDROID_PATH)/app/src/main/java/org/codethechange/culturemesh/

# Convert swagger into a .rst file
swagger: server
	@swg2rst $(SERVER_PATH)/spec_swagger.yaml -f rst -o $(SERVER_DOCS_PATH)/swagger.rst

docstrings: server
	@sphinx-apidoc -o $(SERVER_DOCS_PATH)/autodoc $(SERVER_PATH)/api

# Ensure android repo on same branch as docs repo, then update with git pull
# SOURCE: https://stackoverflow.com/questions/7149984/how-do-i-execute-a-git-command-without-being-in-the-repository
android:
	@git -C $(ANDROID_PATH) checkout $(GIT_BRANCH)
	@git -C $(ANDROID_PATH) pull

# Ensure server repo on same branch as docs repo, then update with git pull
server:
	@git -C $(SERVER_PATH) checkout $(GIT_BRANCH)
	@git -C $(SERVER_PATH) pull

# Catch-all target: route all unknown targets to Sphinx using the new
# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
# Includes both javadoc and swagger as pre-requisites so they are also run with all unknown targets
%: Makefile javadoc swagger docstrings
	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
