.. java:import:: android.arch.persistence.room Entity

.. java:import:: android.arch.persistence.room Ignore

.. java:import:: android.arch.persistence.room PrimaryKey

.. java:import:: java.io Serializable

.. java:import:: java.math BigInteger

Post
====

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: @Entity public class Post extends FeedItem implements Serializable

   Created by nathaniel on 11/10/17.

Fields
------
author
^^^^^^

.. java:field:: @Ignore public User author
   :outertype: Post

content
^^^^^^^

.. java:field:: public String content
   :outertype: Post

datePosted
^^^^^^^^^^

.. java:field:: public String datePosted
   :outertype: Post

id
^^

.. java:field:: @PrimaryKey public long id
   :outertype: Post

imgLink
^^^^^^^

.. java:field:: public String imgLink
   :outertype: Post

network
^^^^^^^

.. java:field:: @Ignore public Network network
   :outertype: Post

networkId
^^^^^^^^^

.. java:field:: public long networkId
   :outertype: Post

userId
^^^^^^

.. java:field:: public long userId
   :outertype: Post

vidLink
^^^^^^^

.. java:field:: public String vidLink
   :outertype: Post

Constructors
------------
Post
^^^^

.. java:constructor:: public Post(int id, int author, int networkId, String content, String imgLink, String vidLink, String datePosted)
   :outertype: Post

Post
^^^^

.. java:constructor:: public Post(int author, String content, String datePosted)
   :outertype: Post

Post
^^^^

.. java:constructor:: public Post()
   :outertype: Post

Methods
-------
getAuthor
^^^^^^^^^

.. java:method:: public User getAuthor()
   :outertype: Post

getContent
^^^^^^^^^^

.. java:method:: public String getContent()
   :outertype: Post

getDatePosted
^^^^^^^^^^^^^

.. java:method:: public String getDatePosted()
   :outertype: Post

getImageLink
^^^^^^^^^^^^

.. java:method:: public String getImageLink()
   :outertype: Post

getNetwork
^^^^^^^^^^

.. java:method:: public Network getNetwork()
   :outertype: Post

getVideoLink
^^^^^^^^^^^^

.. java:method:: public String getVideoLink()
   :outertype: Post

setContent
^^^^^^^^^^

.. java:method:: public void setContent(String content)
   :outertype: Post

setDatePosted
^^^^^^^^^^^^^

.. java:method:: public void setDatePosted(String datePosted)
   :outertype: Post

setImageLink
^^^^^^^^^^^^

.. java:method:: public void setImageLink(String imgLink)
   :outertype: Post

setVideoLink
^^^^^^^^^^^^

.. java:method:: public void setVideoLink(String vidLink)
   :outertype: Post

