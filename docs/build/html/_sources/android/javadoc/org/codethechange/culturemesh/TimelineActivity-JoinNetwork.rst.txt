.. java:import:: android.animation ArgbEvaluator

.. java:import:: android.animation ObjectAnimator

.. java:import:: android.animation ValueAnimator

.. java:import:: android.annotation SuppressLint

.. java:import:: android.app AlertDialog

.. java:import:: android.app Dialog

.. java:import:: android.app DialogFragment

.. java:import:: android.content Context

.. java:import:: android.content DialogInterface

.. java:import:: android.content Intent

.. java:import:: android.content SharedPreferences

.. java:import:: android.content.res ColorStateList

.. java:import:: android.content.res Configuration

.. java:import:: android.net Uri

.. java:import:: android.os Build

.. java:import:: android.os AsyncTask

.. java:import:: android.os Bundle

.. java:import:: android.os Handler

.. java:import:: android.support.annotation RequiresApi

.. java:import:: android.support.design.widget BottomSheetBehavior

.. java:import:: android.support.design.widget BottomSheetDialogFragment

.. java:import:: android.support.design.widget FloatingActionButton

.. java:import:: android.support.v4.widget SwipeRefreshLayout

.. java:import:: android.support.v7.app ActionBarDrawerToggle

.. java:import:: android.support.v7.app AppCompatDelegate

.. java:import:: android.support.v7.widget LinearLayoutManager

.. java:import:: android.support.v7.widget RecyclerView

.. java:import:: android.util Log

.. java:import:: android.view GestureDetector

.. java:import:: android.view MotionEvent

.. java:import:: android.view SubMenu

.. java:import:: android.view View

.. java:import:: android.support.v4.view GravityCompat

.. java:import:: android.support.v4.widget DrawerLayout

.. java:import:: android.view Menu

.. java:import:: android.view MenuItem

.. java:import:: android.view.animation Animation

.. java:import:: android.view.animation AnimationUtils

.. java:import:: android.view.animation DecelerateInterpolator

.. java:import:: android.widget Button

.. java:import:: android.widget ImageButton

.. java:import:: android.widget ImageView

.. java:import:: android.widget LinearLayout

.. java:import:: android.widget TextView

.. java:import:: android.widget Toast

.. java:import:: com.crashlytics.android Crashlytics

.. java:import:: io.fabric.sdk.android Fabric

.. java:import:: org.codethechange.culturemesh.models FromLocation

.. java:import:: org.codethechange.culturemesh.models NearLocation

.. java:import:: org.codethechange.culturemesh.models Network

.. java:import:: org.codethechange.culturemesh.models User

.. java:import:: java.sql Time

.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: java.io Serializable

.. java:import:: java.math BigInteger

.. java:import:: java.util ArrayList

.. java:import:: java.util HashSet

.. java:import:: java.util Set

TimelineActivity.JoinNetwork
============================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type::  class JoinNetwork extends AsyncTask<Long, Void, NetworkResponse>
   :outertype: TimelineActivity

Methods
-------
doInBackground
^^^^^^^^^^^^^^

.. java:method:: @Override protected NetworkResponse doInBackground(Long... longs)
   :outertype: TimelineActivity.JoinNetwork

onPostExecute
^^^^^^^^^^^^^

.. java:method:: @Override protected void onPostExecute(NetworkResponse networkResponse)
   :outertype: TimelineActivity.JoinNetwork

