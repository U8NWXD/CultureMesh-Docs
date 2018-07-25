.. java:import:: android.arch.persistence.room Entity

.. java:import:: android.arch.persistence.room Ignore

.. java:import:: android.arch.persistence.room PrimaryKey

PostReply
=========

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: @Entity public class PostReply

   Created by Drew Gregory on 3/4/18.

Fields
------
author
^^^^^^

.. java:field:: @Ignore public User author
   :outertype: PostReply

id
^^

.. java:field:: @PrimaryKey public long id
   :outertype: PostReply

networkId
^^^^^^^^^

.. java:field:: public long networkId
   :outertype: PostReply

parentId
^^^^^^^^

.. java:field:: public long parentId
   :outertype: PostReply

replyDate
^^^^^^^^^

.. java:field:: public String replyDate
   :outertype: PostReply

replyText
^^^^^^^^^

.. java:field:: public String replyText
   :outertype: PostReply

userId
^^^^^^

.. java:field:: public long userId
   :outertype: PostReply

Constructors
------------
PostReply
^^^^^^^^^

.. java:constructor:: public PostReply(long id, long parentId, long userId, long networkId, String replyDate, String replyText)
   :outertype: PostReply

PostReply
^^^^^^^^^

.. java:constructor:: public PostReply()
   :outertype: PostReply

Methods
-------
getAuthor
^^^^^^^^^

.. java:method:: public User getAuthor()
   :outertype: PostReply

