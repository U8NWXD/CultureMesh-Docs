.. java:import:: android.content Intent

.. java:import:: android.os AsyncTask

.. java:import:: android.os Handler

.. java:import:: android.support.design.widget FloatingActionButton

.. java:import:: android.support.v4.app FragmentActivity

.. java:import:: android.support.constraint ConstraintLayout

.. java:import:: android.support.design.widget Snackbar

.. java:import:: android.support.v7.app AppCompatActivity

.. java:import:: android.os Bundle

.. java:import:: android.support.v7.widget CardView

.. java:import:: android.support.v7.widget LinearLayoutManager

.. java:import:: android.support.v7.widget RecyclerView

.. java:import:: android.util Log

.. java:import:: android.view LayoutInflater

.. java:import:: android.util Log

.. java:import:: android.util SparseArray

.. java:import:: android.util SparseBooleanArray

.. java:import:: android.view View

.. java:import:: android.view.animation Animation

.. java:import:: android.view.animation Transformation

.. java:import:: android.widget AdapterView

.. java:import:: android.widget ArrayAdapter

.. java:import:: android.widget Button

.. java:import:: android.widget ImageButton

.. java:import:: android.widget ImageView

.. java:import:: android.widget LinearLayout

.. java:import:: android.widget ListView

.. java:import:: android.widget ProgressBar

.. java:import:: android.widget TextView

.. java:import:: com.squareup.picasso Picasso

.. java:import:: org.codethechange.culturemesh.models Post

.. java:import:: org.codethechange.culturemesh.models PostReply

.. java:import:: org.w3c.dom Comment

.. java:import:: java.util Date

.. java:import:: java.util List

SpecificPostActivity.SubmitPostReply
====================================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type::  class SubmitPostReply extends AsyncTask<PostReply, Void, NetworkResponse>
   :outertype: SpecificPostActivity

Methods
-------
doInBackground
^^^^^^^^^^^^^^

.. java:method:: @Override protected NetworkResponse doInBackground(PostReply... postReplies)
   :outertype: SpecificPostActivity.SubmitPostReply

onPostExecute
^^^^^^^^^^^^^

.. java:method:: @Override protected void onPostExecute(NetworkResponse response)
   :outertype: SpecificPostActivity.SubmitPostReply

   If POSTing succeeded: Closes the activity and returns the user to the previous screen If POSTing failed: Displays error message and returns uer to composition screen

   :param response: Status of doInBackground method that represents whether POSTing succeeded

onPreExecute
^^^^^^^^^^^^

.. java:method:: @Override protected void onPreExecute()
   :outertype: SpecificPostActivity.SubmitPostReply

   Makes the progress bar indeterminate

