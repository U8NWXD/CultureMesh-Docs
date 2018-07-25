.. java:import:: android.arch.persistence.room Entity

Region
======

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: @Entity public class Region extends Place

   Created by Drew Gregory on 2/23/18.

Fields
------
countryId
^^^^^^^^^

.. java:field:: public long countryId
   :outertype: Region

countryName
^^^^^^^^^^^

.. java:field:: public String countryName
   :outertype: Region

Constructors
------------
Region
^^^^^^

.. java:constructor:: public Region()
   :outertype: Region

Region
^^^^^^

.. java:constructor:: public Region(long id, String name, Point latLng, long pop, long countryId, String countryName)
   :outertype: Region

