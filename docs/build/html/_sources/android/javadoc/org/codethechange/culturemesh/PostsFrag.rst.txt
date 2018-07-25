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

PostsFrag
=========

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class PostsFrag extends Fragment

   Created by Dylan Grosz (dgrosz@stanford.edu) on 11/10/17.

Fields
------
selectedNetwork
^^^^^^^^^^^^^^^

.. java:field::  long selectedNetwork
   :outertype: PostsFrag

settings
^^^^^^^^

.. java:field::  SharedPreferences settings
   :outertype: PostsFrag

Constructors
------------
PostsFrag
^^^^^^^^^

.. java:constructor:: public PostsFrag()
   :outertype: PostsFrag

Methods
-------
onAttach
^^^^^^^^

.. java:method:: @Override public void onAttach(Context context)
   :outertype: PostsFrag

onCreate
^^^^^^^^

.. java:method:: @Override public void onCreate(Bundle savedInstanceState)
   :outertype: PostsFrag

onCreateView
^^^^^^^^^^^^

.. java:method:: @Override public View onCreateView(LayoutInflater inflater, ViewGroup container, Bundle savedInstanceState)
   :outertype: PostsFrag

onDetach
^^^^^^^^

.. java:method:: @Override public void onDetach()
   :outertype: PostsFrag

