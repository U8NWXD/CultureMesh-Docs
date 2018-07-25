.. java:import:: android.arch.persistence.room Room

.. java:import:: android.content Context

.. java:import:: android.util Log

.. java:import:: org.codethechange.culturemesh.data CMDatabase

.. java:import:: org.codethechange.culturemesh.data CityDao

.. java:import:: org.codethechange.culturemesh.data CountryDao

.. java:import:: org.codethechange.culturemesh.data EventDao

.. java:import:: org.codethechange.culturemesh.data EventSubscription

.. java:import:: org.codethechange.culturemesh.data EventSubscriptionDao

.. java:import:: org.codethechange.culturemesh.data NetworkDao

.. java:import:: org.codethechange.culturemesh.data NetworkSubscription

.. java:import:: org.codethechange.culturemesh.data NetworkSubscriptionDao

.. java:import:: org.codethechange.culturemesh.data PostDao

.. java:import:: org.codethechange.culturemesh.data PostReplyDao

.. java:import:: org.codethechange.culturemesh.data RegionDao

.. java:import:: org.codethechange.culturemesh.data UserDao

.. java:import:: org.codethechange.culturemesh.models City

.. java:import:: org.codethechange.culturemesh.models Country

.. java:import:: org.codethechange.culturemesh.models Event

.. java:import:: org.codethechange.culturemesh.models FromLocation

.. java:import:: org.codethechange.culturemesh.models Language

.. java:import:: org.codethechange.culturemesh.models Location

.. java:import:: org.codethechange.culturemesh.models NearLocation

.. java:import:: org.codethechange.culturemesh.models Network

.. java:import:: org.codethechange.culturemesh.models Place

.. java:import:: org.codethechange.culturemesh.models Point

.. java:import:: org.codethechange.culturemesh.models PostReply

.. java:import:: org.codethechange.culturemesh.models Region

.. java:import:: org.codethechange.culturemesh.models User

.. java:import:: org.json JSONArray

.. java:import:: org.json JSONException

.. java:import:: org.json JSONObject

.. java:import:: java.util ArrayList

.. java:import:: java.util List

API.Put
=======

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: static class Put
   :outertype: API

Methods
-------
event
^^^^^

.. java:method:: static NetworkResponse event(Event event)
   :outertype: API.Put

user
^^^^

.. java:method:: static NetworkResponse<User> user(User user)
   :outertype: API.Put

