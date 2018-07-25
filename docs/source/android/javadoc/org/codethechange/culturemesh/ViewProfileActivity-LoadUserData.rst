.. java:import:: android.os AsyncTask

.. java:import:: android.os Bundle

.. java:import:: android.support.design.widget TabLayout

.. java:import:: android.support.v4.app Fragment

.. java:import:: android.support.v4.app FragmentManager

.. java:import:: android.support.v4.app FragmentStatePagerAdapter

.. java:import:: android.support.v4.view PagerAdapter

.. java:import:: android.support.v4.view ViewPager

.. java:import:: android.support.v7.app AppCompatActivity

.. java:import:: android.support.v7.widget Toolbar

.. java:import:: android.widget ImageView

.. java:import:: android.widget TextView

.. java:import:: com.squareup.picasso Picasso

.. java:import:: org.codethechange.culturemesh.models User

ViewProfileActivity.LoadUserData
================================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type::  class LoadUserData extends AsyncTask<Long, Void, NetworkResponse<User>>
   :outertype: ViewProfileActivity

Methods
-------
doInBackground
^^^^^^^^^^^^^^

.. java:method:: @Override protected NetworkResponse<User> doInBackground(Long... longs)
   :outertype: ViewProfileActivity.LoadUserData

onPostExecute
^^^^^^^^^^^^^

.. java:method:: @Override protected void onPostExecute(NetworkResponse<User> res)
   :outertype: ViewProfileActivity.LoadUserData

