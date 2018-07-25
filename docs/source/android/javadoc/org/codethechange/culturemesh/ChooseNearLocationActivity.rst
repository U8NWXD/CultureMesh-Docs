.. java:import:: android.app SearchManager

.. java:import:: android.content Context

.. java:import:: android.content Intent

.. java:import:: android.os Bundle

.. java:import:: android.support.design.widget FloatingActionButton

.. java:import:: android.support.design.widget Snackbar

.. java:import:: android.support.v7.app AppCompatActivity

.. java:import:: android.support.v7.widget Toolbar

.. java:import:: android.view View

.. java:import:: android.widget AdapterView

.. java:import:: android.widget ListView

.. java:import:: android.widget SearchView

.. java:import:: android.widget Toast

.. java:import:: java.util ArrayList

ChooseNearLocationActivity
==========================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class ChooseNearLocationActivity extends AppCompatActivity implements SearchView.OnQueryTextListener

Fields
------
CHOSEN_LOCATION
^^^^^^^^^^^^^^^

.. java:field:: public static final String CHOSEN_LOCATION
   :outertype: ChooseNearLocationActivity

RESULT_OK
^^^^^^^^^

.. java:field:: public final int RESULT_OK
   :outertype: ChooseNearLocationActivity

adapter
^^^^^^^

.. java:field::  LocationSearchAdapter adapter
   :outertype: ChooseNearLocationActivity

dummy
^^^^^

.. java:field::  ArrayList<String> dummy
   :outertype: ChooseNearLocationActivity

searchList
^^^^^^^^^^

.. java:field::  ListView searchList
   :outertype: ChooseNearLocationActivity

Methods
-------
onCreate
^^^^^^^^

.. java:method:: @Override protected void onCreate(Bundle savedInstanceState)
   :outertype: ChooseNearLocationActivity

onQueryTextChange
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean onQueryTextChange(String newText)
   :outertype: ChooseNearLocationActivity

onQueryTextSubmit
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean onQueryTextSubmit(String query)
   :outertype: ChooseNearLocationActivity

