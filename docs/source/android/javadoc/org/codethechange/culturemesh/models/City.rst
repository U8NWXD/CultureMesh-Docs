.. java:import:: android.arch.persistence.room Entity

City
====

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: @Entity public class City extends Region

   Created by Drew Gregory on 2/23/18.

Fields
------
regionId
^^^^^^^^

.. java:field:: public long regionId
   :outertype: City

regionName
^^^^^^^^^^

.. java:field:: public String regionName
   :outertype: City

Constructors
------------
City
^^^^

.. java:constructor:: public City()
   :outertype: City

City
^^^^

.. java:constructor:: public City(long id, String name, Point latLng, long pop, long countryId, String countryName, long regionId, String regionName)
   :outertype: City

