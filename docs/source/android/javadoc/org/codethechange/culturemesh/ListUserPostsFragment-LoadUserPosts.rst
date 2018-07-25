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

ListUserPostsFragment.LoadUserPosts
===================================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type::  class LoadUserPosts extends AsyncTask<Long, Void, Void>
   :outertype: ListUserPostsFragment

Methods
-------
doInBackground
^^^^^^^^^^^^^^

.. java:method:: @Override protected Void doInBackground(Long... longs)
   :outertype: ListUserPostsFragment.LoadUserPosts

onPostExecute
^^^^^^^^^^^^^

.. java:method:: @Override protected void onPostExecute(Void v)
   :outertype: ListUserPostsFragment.LoadUserPosts

onPreExecute
^^^^^^^^^^^^

.. java:method:: @Override protected void onPreExecute()
   :outertype: ListUserPostsFragment.LoadUserPosts

