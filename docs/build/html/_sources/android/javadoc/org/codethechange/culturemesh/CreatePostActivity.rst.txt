.. java:import:: android.app Activity

.. java:import:: android.app Dialog

.. java:import:: android.app DialogFragment

.. java:import:: android.content Context

.. java:import:: android.content DialogInterface

.. java:import:: android.content.res ColorStateList

.. java:import:: android.graphics Typeface

.. java:import:: android.os AsyncTask

.. java:import:: android.os Build

.. java:import:: android.os Bundle

.. java:import:: android.support.design.widget FloatingActionButton

.. java:import:: android.support.design.widget Snackbar

.. java:import:: android.support.v4.app ActivityCompat

.. java:import:: android.support.v7.app AlertDialog

.. java:import:: android.support.v7.app AppCompatActivity

.. java:import:: android.support.v7.widget Toolbar

.. java:import:: android.text Editable

.. java:import:: android.text Html

.. java:import:: android.text SpannableStringBuilder

.. java:import:: android.text Spanned

.. java:import:: android.text.method LinkMovementMethod

.. java:import:: android.text.style StyleSpan

.. java:import:: android.text.style URLSpan

.. java:import:: android.text.style UnderlineSpan

.. java:import:: android.util AttributeSet

.. java:import:: android.util Log

.. java:import:: android.util SparseArray

.. java:import:: android.util SparseBooleanArray

.. java:import:: android.util SparseIntArray

.. java:import:: android.view Menu

.. java:import:: android.view MenuInflater

.. java:import:: android.view MenuItem

.. java:import:: android.view View

.. java:import:: android.view.inputmethod InputMethodManager

.. java:import:: android.widget Button

.. java:import:: android.widget EditText

.. java:import:: android.widget ProgressBar

.. java:import:: android.widget TextView

.. java:import:: org.codethechange.culturemesh.models Event

.. java:import:: org.codethechange.culturemesh.models Network

.. java:import:: org.codethechange.culturemesh.models Post

.. java:import:: org.codethechange.culturemesh.models User

.. java:import:: java.io Serializable

.. java:import:: java.lang.reflect Type

.. java:import:: java.math BigInteger

.. java:import:: java.util Calendar

.. java:import:: java.util Date

.. java:import:: java.util HashMap

CreatePostActivity
==================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class CreatePostActivity extends AppCompatActivity implements FormatManager.IconUpdateListener

Fields
------
content
^^^^^^^

.. java:field::  ListenableEditText content
   :outertype: CreatePostActivity

formatManager
^^^^^^^^^^^^^

.. java:field::  FormatManager formatManager
   :outertype: CreatePostActivity

menuItems
^^^^^^^^^

.. java:field::  SparseArray<MenuItem> menuItems
   :outertype: CreatePostActivity

networkLabel
^^^^^^^^^^^^

.. java:field::  TextView networkLabel
   :outertype: CreatePostActivity

Methods
-------
onCreate
^^^^^^^^

.. java:method:: @Override protected void onCreate(Bundle savedInstanceState)
   :outertype: CreatePostActivity

onCreateOptionsMenu
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean onCreateOptionsMenu(Menu menu)
   :outertype: CreatePostActivity

onOptionsItemSelected
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean onOptionsItemSelected(MenuItem item)
   :outertype: CreatePostActivity

   This function handles what happens when our format toggle buttons are clicked. We want to update the content formatting when this happens as well with Spannables. Check out https://stackoverflow.com/questions/10828182/spannablestringbuilder-to-create-string-with-multiple-fonts-text-sizes-etc-examp for more info.

   :param item: the MenuItem that was tapped.

updateIconToggles
^^^^^^^^^^^^^^^^^

.. java:method:: public void updateIconToggles(SparseBooleanArray formTogState, SparseArray<int[]> toggleIcons)
   :outertype: CreatePostActivity

   This fancy function uses our SparseArray's to concisely iterate over our toggle icons and update their colors - white if untoggled, black if toggled.

