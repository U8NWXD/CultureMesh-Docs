.. java:import:: android.arch.persistence.room Entity

.. java:import:: android.arch.persistence.room PrimaryKey

.. java:import:: java.io Serializable

.. java:import:: java.math BigInteger

Location
========

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: public class Location implements Serializable

   Created by nathaniel on 11/10/17.

Fields
------
city
^^^^

.. java:field:: public String city
   :outertype: Location

city_id
^^^^^^^

.. java:field:: public long city_id
   :outertype: Location

country
^^^^^^^

.. java:field:: public String country
   :outertype: Location

country_id
^^^^^^^^^^

.. java:field:: public long country_id
   :outertype: Location

   When stored in the Database, we will store just the id's. The object returned from the API will have the country, region, and city updated.

location_id
^^^^^^^^^^^

.. java:field:: public long location_id
   :outertype: Location

region
^^^^^^

.. java:field:: public String region
   :outertype: Location

region_id
^^^^^^^^^

.. java:field:: public long region_id
   :outertype: Location

Constructors
------------
Location
^^^^^^^^

.. java:constructor:: public Location(String country, String region, String city, Point[] points)
   :outertype: Location

Location
^^^^^^^^

.. java:constructor:: public Location()
   :outertype: Location

Methods
-------
shortName
^^^^^^^^^

.. java:method:: public String shortName()
   :outertype: Location

toString
^^^^^^^^

.. java:method:: public String toString()
   :outertype: Location

