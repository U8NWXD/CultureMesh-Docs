.. java:import:: android.arch.persistence.room Ignore

NearLocation
============

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: public class NearLocation

   Created by Drew Gregory on 2/19/18. Exact copy of Location, but used as Embedded Entity in SQLite Database.

Fields
------
near_city
^^^^^^^^^

.. java:field:: @Ignore public String near_city
   :outertype: NearLocation

near_city_id
^^^^^^^^^^^^

.. java:field:: public long near_city_id
   :outertype: NearLocation

near_country
^^^^^^^^^^^^

.. java:field:: @Ignore public String near_country
   :outertype: NearLocation

near_country_id
^^^^^^^^^^^^^^^

.. java:field:: public long near_country_id
   :outertype: NearLocation

   When stored in the Database, we will store just the id's. The object returned near the API will have the country, region, and city updated. The default value for country, region, city is 0.

near_region
^^^^^^^^^^^

.. java:field:: @Ignore public String near_region
   :outertype: NearLocation

near_region_id
^^^^^^^^^^^^^^

.. java:field:: public long near_region_id
   :outertype: NearLocation

Constructors
------------
NearLocation
^^^^^^^^^^^^

.. java:constructor:: public NearLocation()
   :outertype: NearLocation

NearLocation
^^^^^^^^^^^^

.. java:constructor:: public NearLocation(String near_country, String near_region, String near_city, Point[] points)
   :outertype: NearLocation

NearLocation
^^^^^^^^^^^^

.. java:constructor:: public NearLocation(long cityId, long regionId, long countryId)
   :outertype: NearLocation

Methods
-------
shortName
^^^^^^^^^

.. java:method:: public String shortName()
   :outertype: NearLocation

toString
^^^^^^^^

.. java:method:: public String toString()
   :outertype: NearLocation

