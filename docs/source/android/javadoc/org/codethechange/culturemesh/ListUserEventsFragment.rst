.. java:import:: android.content Intent

.. java:import:: android.os AsyncTask

.. java:import:: android.os Bundle

.. java:import:: android.support.v4.app Fragment

.. java:import:: android.support.v7.widget LinearLayoutManager

.. java:import:: android.support.v7.widget RecyclerView

.. java:import:: android.view LayoutInflater

.. java:import:: android.view View

.. java:import:: android.view ViewGroup

.. java:import:: android.widget TextView

.. java:import:: android.widget Toast

.. java:import:: org.codethechange.culturemesh.models FeedItem

.. java:import:: org.codethechange.culturemesh.models Post

.. java:import:: java.util ArrayList

ListUserEventsFragment
======================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class ListUserEventsFragment extends Fragment implements RVAdapter.OnItemClickListener

   Created by Drew Gregory on 03/29/18. This fragment lists the the events a user is subscribed to. It is used in ViewProfileActivity.

Fields
------
emptyText
^^^^^^^^^

.. java:field::  TextView emptyText
   :outertype: ListUserEventsFragment

rv
^^

.. java:field::  RecyclerView rv
   :outertype: ListUserEventsFragment

Methods
-------
newInstance
^^^^^^^^^^^

.. java:method:: public static ListUserEventsFragment newInstance(long selUser)
   :outertype: ListUserEventsFragment

   Returns a new instance of this fragment for the given section number.

onCreateView
^^^^^^^^^^^^

.. java:method:: @Override public View onCreateView(LayoutInflater inflater, ViewGroup container, Bundle savedInstanceState)
   :outertype: ListUserEventsFragment

onItemClick
^^^^^^^^^^^

.. java:method:: @Override public void onItemClick(FeedItem item)
   :outertype: ListUserEventsFragment

