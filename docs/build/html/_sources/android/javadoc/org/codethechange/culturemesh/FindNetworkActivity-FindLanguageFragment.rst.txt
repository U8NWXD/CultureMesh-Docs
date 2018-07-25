.. java:import:: android.app AlertDialog

.. java:import:: android.app SearchManager

.. java:import:: android.content Context

.. java:import:: android.content DialogInterface

.. java:import:: android.content Intent

.. java:import:: android.content SharedPreferences

.. java:import:: android.media Image

.. java:import:: android.os AsyncTask

.. java:import:: android.support.constraint ConstraintLayout

.. java:import:: android.support.design.widget TabLayout

.. java:import:: android.support.v7.app AppCompatActivity

.. java:import:: android.support.v7.widget Toolbar

.. java:import:: android.support.v4.app Fragment

.. java:import:: android.support.v4.app FragmentManager

.. java:import:: android.support.v4.app FragmentPagerAdapter

.. java:import:: android.support.v4.view ViewPager

.. java:import:: android.os Bundle

.. java:import:: android.text TextUtils

.. java:import:: android.view LayoutInflater

.. java:import:: android.view Menu

.. java:import:: android.view MenuItem

.. java:import:: android.view View

.. java:import:: android.view ViewGroup

.. java:import:: android.widget AdapterView

.. java:import:: android.widget ArrayAdapter

.. java:import:: android.widget Button

.. java:import:: android.widget ImageButton

.. java:import:: android.widget ListView

.. java:import:: android.widget SearchView

.. java:import:: android.widget TextView

.. java:import:: android.widget Toast

.. java:import:: org.w3c.dom Text

.. java:import:: java.util ArrayList

.. java:import:: org.codethechange.culturemesh.models User

.. java:import:: java.util ArrayList

FindNetworkActivity.FindLanguageFragment
========================================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public static class FindLanguageFragment extends Fragment implements SearchView.OnQueryTextListener
   :outertype: FindNetworkActivity

   The fragment for finding language networks.

Constructors
------------
FindLanguageFragment
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public FindLanguageFragment()
   :outertype: FindNetworkActivity.FindLanguageFragment

Methods
-------
newInstance
^^^^^^^^^^^

.. java:method:: public static FindLanguageFragment newInstance(int sectionNumber)
   :outertype: FindNetworkActivity.FindLanguageFragment

   Returns a new instance of this fragment for the given section number.

onCreateView
^^^^^^^^^^^^

.. java:method:: @Override public View onCreateView(LayoutInflater inflater, ViewGroup container, Bundle savedInstanceState)
   :outertype: FindNetworkActivity.FindLanguageFragment

onQueryTextChange
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean onQueryTextChange(String newText)
   :outertype: FindNetworkActivity.FindLanguageFragment

onQueryTextSubmit
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean onQueryTextSubmit(String query)
   :outertype: FindNetworkActivity.FindLanguageFragment

