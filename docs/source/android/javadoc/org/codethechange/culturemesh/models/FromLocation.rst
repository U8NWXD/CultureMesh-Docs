.. java:import:: android.arch.persistence.room Ignore

FromLocation
============

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: public class FromLocation

   Created by Drew Gregory on 2/19/18. Exact copy of Location, but used as Embedded Entity in SQLite Database.

Fields
------
from_city
^^^^^^^^^

.. java:field:: @Ignore public String from_city
   :outertype: FromLocation

from_city_id
^^^^^^^^^^^^

.. java:field:: public long from_city_id
   :outertype: FromLocation

from_country
^^^^^^^^^^^^

.. java:field:: @Ignore public String from_country
   :outertype: FromLocation

from_country_id
^^^^^^^^^^^^^^^

.. java:field:: public long from_country_id
   :outertype: FromLocation

   When stored in the Database, we will store just the id's. The object returned from the API will have the country, region, and city updated. The default value for country, region, city is 0.

from_region
^^^^^^^^^^^

.. java:field:: @Ignore public String from_region
   :outertype: FromLocation

from_region_id
^^^^^^^^^^^^^^

.. java:field:: public long from_region_id
   :outertype: FromLocation

Constructors
------------
FromLocation
^^^^^^^^^^^^

.. java:constructor:: public FromLocation()
   :outertype: FromLocation

FromLocation
^^^^^^^^^^^^

.. java:constructor:: public FromLocation(String from_country, String from_region, String from_city, Point[] points)
   :outertype: FromLocation

FromLocation
^^^^^^^^^^^^

.. java:constructor:: public FromLocation(long cityId, long regionId, long countryId)
   :outertype: FromLocation

Methods
-------
shortName
^^^^^^^^^

.. java:method:: public String shortName()
   :outertype: FromLocation

toString
^^^^^^^^

.. java:method:: public String toString()
   :outertype: FromLocation

