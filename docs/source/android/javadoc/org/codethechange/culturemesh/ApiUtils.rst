.. java:import:: android.os AsyncTask

.. java:import:: org.codethechange.culturemesh.models Network

.. java:import:: java.util ArrayList

.. java:import:: java.util.concurrent ExecutionException

ApiUtils
========

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class ApiUtils

   Created by cs on 3/28/18.

Methods
-------
getJoinedNetworks
^^^^^^^^^^^^^^^^^

.. java:method:: public static NetworkResponse<ArrayList<Network>> getJoinedNetworks(long currUser, AsyncTask<Long, Void, NetworkResponse<ArrayList<Network>>> task)
   :outertype: ApiUtils

hasJoinedNetwork
^^^^^^^^^^^^^^^^

.. java:method:: public static boolean hasJoinedNetwork(long currUser, AsyncTask<Long, Void, NetworkResponse<ArrayList<Network>>> task)
   :outertype: ApiUtils

