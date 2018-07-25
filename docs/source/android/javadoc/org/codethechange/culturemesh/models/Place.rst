.. java:import:: android.arch.persistence.room Embedded

.. java:import:: android.arch.persistence.room Entity

.. java:import:: android.arch.persistence.room PrimaryKey

.. java:import:: kotlin.internal HidesMembers

Place
=====

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: @Entity public class Place

   Created by Drew Gregory on 2/23/18. This is the superclass for cities, regions, and countries.

Fields
------
featureCode
^^^^^^^^^^^

.. java:field:: public String featureCode
   :outertype: Place

id
^^

.. java:field:: @PrimaryKey public long id
   :outertype: Place

latLng
^^^^^^

.. java:field:: @Embedded public Point latLng
   :outertype: Place

name
^^^^

.. java:field:: public String name
   :outertype: Place

population
^^^^^^^^^^

.. java:field:: public long population
   :outertype: Place

Constructors
------------
Place
^^^^^

.. java:constructor:: public Place()
   :outertype: Place

Place
^^^^^

.. java:constructor:: public Place(long id, String name, Point latLng, long pop)
   :outertype: Place

