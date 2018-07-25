.. java:import:: android.content Context

.. java:import:: android.content Intent

.. java:import:: android.content SharedPreferences

.. java:import:: android.support.v7.widget RecyclerView

.. java:import:: android.view LayoutInflater

.. java:import:: android.view View

.. java:import:: android.view ViewGroup

.. java:import:: android.widget TextView

.. java:import:: org.codethechange.culturemesh.models Network

.. java:import:: java.util ArrayList

NetworkSummaryAdapter
=====================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class NetworkSummaryAdapter extends RecyclerView.Adapter<NetworkSummaryAdapter.PostViewHolder>

   Created by Drew Gregory on 03/28/18. This functions as the recyclerview adapter for the listview in ViewProfileActivity, where the user can view other users' subscribed networks.

Constructors
------------
NetworkSummaryAdapter
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor::  NetworkSummaryAdapter(ArrayList<Network> networks, ArrayList<Integer> postCounts, ArrayList<Integer> userCounts, OnNetworkTapListener listener)
   :outertype: NetworkSummaryAdapter

Methods
-------
getItemCount
^^^^^^^^^^^^

.. java:method:: @Override public int getItemCount()
   :outertype: NetworkSummaryAdapter

getNetworks
^^^^^^^^^^^

.. java:method:: public ArrayList<Network> getNetworks()
   :outertype: NetworkSummaryAdapter

getPostCounts
^^^^^^^^^^^^^

.. java:method:: public ArrayList<Integer> getPostCounts()
   :outertype: NetworkSummaryAdapter

getUserCounts
^^^^^^^^^^^^^

.. java:method:: public ArrayList<Integer> getUserCounts()
   :outertype: NetworkSummaryAdapter

onBindViewHolder
^^^^^^^^^^^^^^^^

.. java:method:: @Override public void onBindViewHolder(PostViewHolder holder, int position)
   :outertype: NetworkSummaryAdapter

onCreateViewHolder
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public PostViewHolder onCreateViewHolder(ViewGroup parent, int viewType)
   :outertype: NetworkSummaryAdapter

