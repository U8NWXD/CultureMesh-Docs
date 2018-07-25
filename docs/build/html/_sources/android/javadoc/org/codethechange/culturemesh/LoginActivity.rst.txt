.. java:import:: android.app Activity

.. java:import:: android.content Intent

.. java:import:: android.content SharedPreferences

.. java:import:: android.os AsyncTask

.. java:import:: android.os Bundle

.. java:import:: android.support.constraint ConstraintLayout

.. java:import:: android.support.constraint ConstraintSet

.. java:import:: android.support.v7.app AlertDialog

.. java:import:: android.support.v7.app AppCompatActivity

.. java:import:: android.support.v7.widget Toolbar

.. java:import:: android.util DisplayMetrics

.. java:import:: android.view View

.. java:import:: android.view.animation Animation

.. java:import:: android.view.animation Transformation

.. java:import:: android.widget Button

.. java:import:: android.widget EditText

.. java:import:: android.widget TextView

.. java:import:: org.codethechange.culturemesh.models User

LoginActivity
=============

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class LoginActivity extends RedirectableAppCompatActivity

Fields
------
confirmPassword
^^^^^^^^^^^^^^^

.. java:field::  EditText confirmPassword
   :outertype: LoginActivity

firstNameText
^^^^^^^^^^^^^

.. java:field::  EditText firstNameText
   :outertype: LoginActivity

lastNameText
^^^^^^^^^^^^

.. java:field::  EditText lastNameText
   :outertype: LoginActivity

needAccountText
^^^^^^^^^^^^^^^

.. java:field::  TextView needAccountText
   :outertype: LoginActivity

passwordText
^^^^^^^^^^^^

.. java:field::  EditText passwordText
   :outertype: LoginActivity

Methods
-------
isLoggedIn
^^^^^^^^^^

.. java:method:: public static boolean isLoggedIn(SharedPreferences settings)
   :outertype: LoginActivity

onCreate
^^^^^^^^

.. java:method:: @Override protected void onCreate(Bundle savedInstanceState)
   :outertype: LoginActivity

setLoggedIn
^^^^^^^^^^^

.. java:method:: public static void setLoggedIn(SharedPreferences settings, long userID)
   :outertype: LoginActivity

   Largely for testing, this public method can be used to set which user is currently logged in This is useful for PickOnboardingStatusActivity because different login states correspond to different users. No logged-in user is signalled by a missing SharedPreferences entry.

   :param settings: The SharedPreferences storing user login state
   :param userID: ID of the user to make logged-in

setLoggedOut
^^^^^^^^^^^^

.. java:method:: public static void setLoggedOut(SharedPreferences settings)
   :outertype: LoginActivity

