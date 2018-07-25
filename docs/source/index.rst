.. CultureMesh Android documentation master file, created by
   sphinx-quickstart on Mon Jul 23 15:18:26 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

=====================================
Documentation for CultureMesh Android
=====================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   Android App Javadoc <android/javadoc/packages>
   Server API Documentation <server/swagger>
   Server Docstrings <server/autodoc/modules.rst>

--------------
Code Reference
--------------

Android Documentation
=====================
The Android code is documented using Javadoc, which can be viewed in three
forms:

* Traditional `Javadoc <_static/API-JavaDoc/index.html>`_
  (includes ``Private`` methods)
* javasphinx :doc:`android/javadoc/packages` (excludes ``Private`` methods)
* The comments in the code itself

Specific sections of the javasphinx Javadoc are referenced throughout the
documentation like so: :java:ref:`API.Get`.

Server Documentation
====================

Swagger
-------
See the API documentation in the Swagger documentation: :doc:`server/swagger`.
If you prefer the representation used by the Swagger editor, navigate to
https://editor.swagger.io, go to ``File`` > ``Import URL``, and paste in
``https://raw.githubusercontent.com/alanefl/culturemesh-api/master/spec_swagger.yaml``

Docstrings
----------
The server code is also documented with docstrings. That documentation can be
viewed in the following ways:

* HTML format: :doc:`server/autodoc/modules`
* The comments in the code itself.

------------------
Indices and tables
------------------

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
