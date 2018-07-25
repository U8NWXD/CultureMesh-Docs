.. java:import:: android.content Context

.. java:import:: android.graphics Color

.. java:import:: android.support.constraint ConstraintLayout

.. java:import:: android.support.constraint ConstraintSet

.. java:import:: android.support.v7.widget CardView

.. java:import:: android.support.v7.widget RecyclerView

.. java:import:: android.util Log

.. java:import:: android.view LayoutInflater

.. java:import:: android.view View

.. java:import:: android.view ViewGroup

.. java:import:: android.widget ImageView

.. java:import:: android.widget LinearLayout

.. java:import:: android.widget RelativeLayout

.. java:import:: android.widget TextView

.. java:import:: com.squareup.picasso Picasso

.. java:import:: org.codethechange.culturemesh.models Event

.. java:import:: org.codethechange.culturemesh.models FeedItem

.. java:import:: org.codethechange.culturemesh.models Post

.. java:import:: org.codethechange.culturemesh.models PostReply

.. java:import:: java.util List

RVCommentAdapter.PostReplyViewHolder
====================================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: static class PostReplyViewHolder extends RecyclerView.ViewHolder
   :outertype: RVCommentAdapter

Fields
------
cv
^^

.. java:field::  CardView cv
   :outertype: RVCommentAdapter.PostReplyViewHolder

images
^^^^^^

.. java:field::  ImageView[] images
   :outertype: RVCommentAdapter.PostReplyViewHolder

layout
^^^^^^

.. java:field::  ConstraintLayout layout
   :outertype: RVCommentAdapter.PostReplyViewHolder

personName
^^^^^^^^^^

.. java:field::  TextView personName
   :outertype: RVCommentAdapter.PostReplyViewHolder

personPhoto
^^^^^^^^^^^

.. java:field::  ImageView personPhoto
   :outertype: RVCommentAdapter.PostReplyViewHolder

reply
^^^^^

.. java:field::  boolean reply
   :outertype: RVCommentAdapter.PostReplyViewHolder

Constructors
------------
PostReplyViewHolder
^^^^^^^^^^^^^^^^^^^

.. java:constructor::  PostReplyViewHolder(View itemView)
   :outertype: RVCommentAdapter.PostReplyViewHolder

Methods
-------
bind
^^^^

.. java:method:: public void bind(PostReply item, OnItemClickListener listener)
   :outertype: RVCommentAdapter.PostReplyViewHolder

isPostReply
^^^^^^^^^^^

.. java:method:: public boolean isPostReply()
   :outertype: RVCommentAdapter.PostReplyViewHolder

