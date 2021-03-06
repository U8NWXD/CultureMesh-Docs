.. java:import:: android.app Activity

.. java:import:: android.content Intent

.. java:import:: android.content SharedPreferences

.. java:import:: android.content.res Configuration

.. java:import:: android.os AsyncTask

.. java:import:: android.os Bundle

.. java:import:: android.support.design.widget NavigationView

.. java:import:: android.support.v4.view GravityCompat

.. java:import:: android.support.v4.widget DrawerLayout

.. java:import:: android.support.v7.app ActionBarDrawerToggle

.. java:import:: android.support.v7.app AppCompatActivity

.. java:import:: android.support.v7.widget Toolbar

.. java:import:: android.text SpannableStringBuilder

.. java:import:: android.text.style RelativeSizeSpan

.. java:import:: android.util Log

.. java:import:: android.util SparseArray

.. java:import:: android.view Menu

.. java:import:: android.view MenuItem

.. java:import:: android.view SubMenu

.. java:import:: android.view View

.. java:import:: android.widget Button

.. java:import:: android.widget FrameLayout

.. java:import:: android.widget ImageView

.. java:import:: android.widget TextView

.. java:import:: com.crashlytics.android Crashlytics

.. java:import:: com.squareup.picasso Picasso

.. java:import:: io.fabric.sdk.android Fabric

.. java:import:: org.codethechange.culturemesh.models Network

.. java:import:: org.codethechange.culturemesh.models User

.. java:import:: java.util HashSet

.. java:import:: java.util List

.. java:import:: java.util Set

DrawerActivity
==============

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class DrawerActivity extends AppCompatActivity implements NavigationView.OnNavigationItemSelectedListener

Fields
------
currentUser
^^^^^^^^^^^

.. java:field:: protected long currentUser
   :outertype: DrawerActivity

frameLayout
^^^^^^^^^^^

.. java:field:: protected FrameLayout frameLayout
   :outertype: DrawerActivity

fullLayout
^^^^^^^^^^

.. java:field:: protected DrawerLayout fullLayout
   :outertype: DrawerActivity

mDrawerLayout
^^^^^^^^^^^^^

.. java:field:: protected DrawerLayout mDrawerLayout
   :outertype: DrawerActivity

mDrawerToggle
^^^^^^^^^^^^^

.. java:field:: protected ActionBarDrawerToggle mDrawerToggle
   :outertype: DrawerActivity

navView
^^^^^^^

.. java:field::  NavigationView navView
   :outertype: DrawerActivity

subscribedNetworkIds
^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected Set<Long> subscribedNetworkIds
   :outertype: DrawerActivity

subscribedNetworks
^^^^^^^^^^^^^^^^^^

.. java:field:: protected SparseArray<Network> subscribedNetworks
   :outertype: DrawerActivity

thisActivity
^^^^^^^^^^^^

.. java:field::  Activity thisActivity
   :outertype: DrawerActivity

Methods
-------
onConfigurationChanged
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void onConfigurationChanged(Configuration newConfig)
   :outertype: DrawerActivity

onNavigationItemSelected
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean onNavigationItemSelected(MenuItem item)
   :outertype: DrawerActivity

onPostCreate
^^^^^^^^^^^^

.. java:method:: @Override protected void onPostCreate(Bundle savedInstanceState)
   :outertype: DrawerActivity

setContentView
^^^^^^^^^^^^^^

.. java:method:: @Override public void setContentView(int layoutResID)
   :outertype: DrawerActivity

