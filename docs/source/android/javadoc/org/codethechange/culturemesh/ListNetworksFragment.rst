.. java:import:: android.content Context

.. java:import:: android.content Intent

.. java:import:: android.content SharedPreferences

.. java:import:: android.os AsyncTask

.. java:import:: android.os Bundle

.. java:import:: android.support.constraint ConstraintLayout

.. java:import:: android.support.v4.app Fragment

.. java:import:: android.support.v7.widget LinearLayoutManager

.. java:import:: android.support.v7.widget RecyclerView

.. java:import:: android.util Log

.. java:import:: android.view LayoutInflater

.. java:import:: android.view View

.. java:import:: android.view ViewGroup

.. java:import:: android.widget AdapterView

.. java:import:: android.widget ImageButton

.. java:import:: android.widget ListView

.. java:import:: android.widget SearchView

.. java:import:: android.widget TextView

.. java:import:: org.codethechange.culturemesh.models Network

.. java:import:: java.util ArrayList

ListNetworksFragment
====================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class ListNetworksFragment extends Fragment implements NetworkSummaryAdapter.OnNetworkTapListener

   Created by Drew Gregory on 03/27/18.

Fields
------
FIRST_TIME
^^^^^^^^^^

.. java:field:: static final String FIRST_TIME
   :outertype: ListNetworksFragment

SELECTED_USER
^^^^^^^^^^^^^

.. java:field:: static final String SELECTED_USER
   :outertype: ListNetworksFragment

emptyText
^^^^^^^^^

.. java:field::  TextView emptyText
   :outertype: ListNetworksFragment

root
^^^^

.. java:field::  View root
   :outertype: ListNetworksFragment

rv
^^

.. java:field::  RecyclerView rv
   :outertype: ListNetworksFragment

Methods
-------
newInstance
^^^^^^^^^^^

.. java:method:: public static ListNetworksFragment newInstance(long selUser)
   :outertype: ListNetworksFragment

   Returns a new instance of this fragment for the given section number.

onCreateView
^^^^^^^^^^^^

.. java:method:: @Override public View onCreateView(LayoutInflater inflater, ViewGroup container, Bundle savedInstanceState)
   :outertype: ListNetworksFragment

onItemClick
^^^^^^^^^^^

.. java:method:: @Override public void onItemClick(View v, Network network)
   :outertype: ListNetworksFragment

   This is the onClick() passed to NetworkSummaryAdapter. Thus, this is executed when the user taps on of the network card views. We want to view the tapped network in TimelineActivity.

   :param v: the CardView.
   :param network: The Network

