.. java:import:: android.app AlertDialog

.. java:import:: android.content DialogInterface

.. java:import:: android.os AsyncTask

.. java:import:: android.os Bundle

.. java:import:: android.provider Settings

.. java:import:: android.support.design.widget FloatingActionButton

.. java:import:: android.support.design.widget Snackbar

.. java:import:: android.support.v7.app AppCompatActivity

.. java:import:: android.support.v7.widget LinearLayoutManager

.. java:import:: android.support.v7.widget RecyclerView

.. java:import:: android.support.v7.widget Toolbar

.. java:import:: android.support.v7.widget.helper ItemTouchHelper

.. java:import:: android.text.format Time

.. java:import:: android.util Log

.. java:import:: android.view View

.. java:import:: android.widget Button

.. java:import:: android.widget EditText

.. java:import:: android.widget ImageView

.. java:import:: android.widget TextView

.. java:import:: com.squareup.picasso Picasso

.. java:import:: org.codethechange.culturemesh.models Network

.. java:import:: org.codethechange.culturemesh.models User

.. java:import:: java.util ArrayList

SettingsActivity
================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class SettingsActivity extends DrawerActivity implements NetworkSummaryAdapter.OnNetworkTapListener

Fields
------
bio
^^^

.. java:field::  EditText bio
   :outertype: SettingsActivity

emptyText
^^^^^^^^^

.. java:field::  TextView emptyText
   :outertype: SettingsActivity

profilePicture
^^^^^^^^^^^^^^

.. java:field::  ImageView profilePicture
   :outertype: SettingsActivity

rv
^^

.. java:field::  RecyclerView rv
   :outertype: SettingsActivity

updateProfile
^^^^^^^^^^^^^

.. java:field::  Button updateProfile
   :outertype: SettingsActivity

user
^^^^

.. java:field::  User user
   :outertype: SettingsActivity

Methods
-------
onCreate
^^^^^^^^

.. java:method:: @Override protected void onCreate(Bundle savedInstanceState)
   :outertype: SettingsActivity

onItemClick
^^^^^^^^^^^

.. java:method:: @Override public void onItemClick(View v, Network network)
   :outertype: SettingsActivity

resetAdapter
^^^^^^^^^^^^

.. java:method::  void resetAdapter()
   :outertype: SettingsActivity

