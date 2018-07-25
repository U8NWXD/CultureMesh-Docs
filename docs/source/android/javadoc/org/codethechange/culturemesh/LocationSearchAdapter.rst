.. java:import:: android.app Activity

.. java:import:: android.content Context

.. java:import:: android.support.annotation LayoutRes

.. java:import:: android.support.annotation NonNull

.. java:import:: android.support.annotation Nullable

.. java:import:: android.util Log

.. java:import:: android.view LayoutInflater

.. java:import:: android.view View

.. java:import:: android.view ViewGroup

.. java:import:: android.widget ArrayAdapter

.. java:import:: android.widget BaseAdapter

.. java:import:: android.widget Filterable

.. java:import:: java.util ArrayList

.. java:import:: android.widget Filter

.. java:import:: android.widget TextView

.. java:import:: java.util List

.. java:import:: java.util.logging LogRecord

LocationSearchAdapter
=====================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class LocationSearchAdapter extends ArrayAdapter<String> implements Filterable

   Created by Drew Gregory (drewgreg@stanford.edu) on 11/7/17.

Constructors
------------
LocationSearchAdapter
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor::  LocationSearchAdapter(Context context, int resource, List<String> locations)
   :outertype: LocationSearchAdapter

   Initialize context variables

   :param context: application context
   :param resource: int resource layout id
   :param locations: string list of locations

Methods
-------
getCount
^^^^^^^^

.. java:method:: @Override public int getCount()
   :outertype: LocationSearchAdapter

   Get size of user list

   :return: userList size

getFilter
^^^^^^^^^

.. java:method:: @NonNull @Override public android.widget.Filter getFilter()
   :outertype: LocationSearchAdapter

getItem
^^^^^^^

.. java:method:: @Override public String getItem(int position)
   :outertype: LocationSearchAdapter

getView
^^^^^^^

.. java:method:: @NonNull @Override public View getView(int position, View convertView, ViewGroup parent)
   :outertype: LocationSearchAdapter

