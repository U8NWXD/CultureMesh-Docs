.. java:import:: android.arch.persistence.room Ignore

.. java:import:: java.util List

FeedItem
========

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: public class FeedItem

   Created by drewgregory on 1/18/18. Superclass for Posts and Events so we can use Polymorphism for feeds.

Fields
------
comments
^^^^^^^^

.. java:field:: @Ignore public List<PostReply> comments
   :outertype: FeedItem

   This list of PostReplies will be where we store the comments for each post.

