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

RVCommentAdapter
================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class RVCommentAdapter extends RecyclerView.Adapter<RVCommentAdapter.PostReplyViewHolder>

   Created by Dylan Grosz (dgrosz@stanford.edu) on 11/10/17.

Constructors
------------
RVCommentAdapter
^^^^^^^^^^^^^^^^

.. java:constructor:: public RVCommentAdapter(List<PostReply> comments, OnItemClickListener listener, Context context)
   :outertype: RVCommentAdapter

Methods
-------
getItemCount
^^^^^^^^^^^^

.. java:method:: @Override public int getItemCount()
   :outertype: RVCommentAdapter

onBindViewHolder
^^^^^^^^^^^^^^^^

.. java:method:: @Override public void onBindViewHolder(PostReplyViewHolder pvh, int i)
   :outertype: RVCommentAdapter

onCreateViewHolder
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public PostReplyViewHolder onCreateViewHolder(ViewGroup parent, int viewType)
   :outertype: RVCommentAdapter

