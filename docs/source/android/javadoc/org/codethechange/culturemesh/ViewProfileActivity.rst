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

ViewProfileActivity
===================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class ViewProfileActivity extends AppCompatActivity

Fields
------
SELECTED_USER
^^^^^^^^^^^^^

.. java:field:: public static final String SELECTED_USER
   :outertype: ViewProfileActivity

mTabLayout
^^^^^^^^^^

.. java:field::  TabLayout mTabLayout
   :outertype: ViewProfileActivity

mViewPager
^^^^^^^^^^

.. java:field::  ViewPager mViewPager
   :outertype: ViewProfileActivity

profilePic
^^^^^^^^^^

.. java:field::  ImageView profilePic
   :outertype: ViewProfileActivity

selUser
^^^^^^^

.. java:field::  long selUser
   :outertype: ViewProfileActivity

userName
^^^^^^^^

.. java:field::  TextView userName
   :outertype: ViewProfileActivity

Methods
-------
onCreate
^^^^^^^^

.. java:method:: @Override protected void onCreate(Bundle savedInstanceState)
   :outertype: ViewProfileActivity

onSupportNavigateUp
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean onSupportNavigateUp()
   :outertype: ViewProfileActivity

   This allows the user to hit the back button on the toolbar to go to the previous activity.

