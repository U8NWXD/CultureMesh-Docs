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

.. java:import:: org.codethechange.culturemesh.models Network

.. java:import:: org.codethechange.culturemesh.models Post

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ListUserPostsFragment
=====================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class ListUserPostsFragment extends Fragment implements RVAdapter.OnItemClickListener

   Created by Drew Gregory on 03/29/18.

Fields
------
emptyText
^^^^^^^^^

.. java:field::  TextView emptyText
   :outertype: ListUserPostsFragment

root
^^^^

.. java:field::  View root
   :outertype: ListUserPostsFragment

rv
^^

.. java:field::  RecyclerView rv
   :outertype: ListUserPostsFragment

Methods
-------
newInstance
^^^^^^^^^^^

.. java:method:: public static ListUserPostsFragment newInstance(long selUser)
   :outertype: ListUserPostsFragment

   Returns a new instance of this fragment for the given section number.

onCreateView
^^^^^^^^^^^^

.. java:method:: @Override public View onCreateView(LayoutInflater inflater, ViewGroup container, Bundle savedInstanceState)
   :outertype: ListUserPostsFragment

onItemClick
^^^^^^^^^^^

.. java:method:: @Override public void onItemClick(FeedItem item)
   :outertype: ListUserPostsFragment

