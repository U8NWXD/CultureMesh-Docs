.. java:import:: android.arch.persistence.db SupportSQLiteDatabase

.. java:import:: android.arch.persistence.room Room

.. java:import:: android.arch.persistence.room.migration Migration

.. java:import:: android.content ContentValues

.. java:import:: android.database Cursor

.. java:import:: android.database.sqlite SQLiteDatabase

.. java:import:: android.os AsyncTask

.. java:import:: android.os Bundle

.. java:import:: android.support.design.widget FloatingActionButton

.. java:import:: android.support.design.widget Snackbar

.. java:import:: android.support.v7.app AppCompatActivity

.. java:import:: android.support.v7.widget Toolbar

.. java:import:: android.util Log

.. java:import:: android.view View

.. java:import:: org.codethechange.culturemesh.data CMDatabase

.. java:import:: org.codethechange.culturemesh.models FromLocation

.. java:import:: org.codethechange.culturemesh.models Location

.. java:import:: org.codethechange.culturemesh.models NearLocation

.. java:import:: org.codethechange.culturemesh.models Network

.. java:import:: java.math BigInteger

.. java:import:: java.util List

DatabaseTest
============

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class DatabaseTest extends AppCompatActivity

Fields
------
MIGRATION_1_2
^^^^^^^^^^^^^

.. java:field:: static final Migration MIGRATION_1_2
   :outertype: DatabaseTest

mDb
^^^

.. java:field::  CMDatabase mDb
   :outertype: DatabaseTest

Methods
-------
onCreate
^^^^^^^^

.. java:method:: @Override protected void onCreate(Bundle savedInstanceState)
   :outertype: DatabaseTest

