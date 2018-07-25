.. java:import:: android.content Context

.. java:import:: android.content Intent

.. java:import:: android.content SharedPreferences

.. java:import:: android.net Uri

.. java:import:: android.os AsyncTask

.. java:import:: android.os Bundle

.. java:import:: android.os Handler

.. java:import:: android.support.v4.app Fragment

.. java:import:: android.support.v4.widget SwipeRefreshLayout

.. java:import:: android.support.v7.app AppCompatActivity

.. java:import:: android.support.v7.app AppCompatDelegate

.. java:import:: android.support.v7.widget LinearLayoutManager

.. java:import:: android.support.v7.widget RecyclerView

.. java:import:: android.util Log

.. java:import:: android.view LayoutInflater

.. java:import:: android.view MotionEvent

.. java:import:: android.view View

.. java:import:: android.view ViewGroup

.. java:import:: android.widget TextView

.. java:import:: android.widget Toast

.. java:import:: org.codethechange.culturemesh.models Event

.. java:import:: org.codethechange.culturemesh.models FeedItem

.. java:import:: org.codethechange.culturemesh.models Network

.. java:import:: org.codethechange.culturemesh.models Post

.. java:import:: org.codethechange.culturemesh.models User

.. java:import:: org.json JSONException

.. java:import:: org.json JSONObject

.. java:import:: java.math BigInteger

.. java:import:: java.sql Time

.. java:import:: java.util ArrayList

.. java:import:: java.util Date

.. java:import:: java.util List

PostsFrag.OnFragmentInteractionListener
=======================================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public interface OnFragmentInteractionListener
   :outertype: PostsFrag

   This interface must be implemented by activities that contain this fragment to allow an interaction in this fragment to be communicated to the activity and potentially other fragments contained in that activity.

   See the Android Training lesson \ `Communicating with Other Fragments <http://developer.android.com/training/basics/fragments/communicating.html>`_\  for more information.

Methods
-------
onFragmentInteraction
^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void onFragmentInteraction(Uri uri)
   :outertype: PostsFrag.OnFragmentInteractionListener

