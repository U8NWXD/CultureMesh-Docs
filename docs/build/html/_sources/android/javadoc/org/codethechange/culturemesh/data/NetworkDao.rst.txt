.. java:import:: android.arch.persistence.room Dao

.. java:import:: android.arch.persistence.room Delete

.. java:import:: android.arch.persistence.room Insert

.. java:import:: android.arch.persistence.room OnConflictStrategy

.. java:import:: android.arch.persistence.room Query

.. java:import:: android.arch.persistence.room Update

.. java:import:: org.codethechange.culturemesh.models Network

.. java:import:: java.util List

NetworkDao
==========

.. java:package:: org.codethechange.culturemesh.data
   :noindex:

.. java:type:: @Dao public interface NetworkDao

   Created by Drew Gregory on 2/19/18.

Methods
-------
deleteNetworks
^^^^^^^^^^^^^^

.. java:method:: @Delete public void deleteNetworks(Network... networks)
   :outertype: NetworkDao

getNetwork
^^^^^^^^^^

.. java:method:: @Query public List<Network> getNetwork(long id)
   :outertype: NetworkDao

insertNetworks
^^^^^^^^^^^^^^

.. java:method:: @Insert public void insertNetworks(Network... networks)
   :outertype: NetworkDao

updateNetworks
^^^^^^^^^^^^^^

.. java:method:: @Update public void updateNetworks(Network... networks)
   :outertype: NetworkDao

