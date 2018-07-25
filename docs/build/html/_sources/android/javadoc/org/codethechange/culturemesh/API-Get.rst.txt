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

API.Get
=======

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: static class Get
   :outertype: API

Methods
-------
autocomplete
^^^^^^^^^^^^

.. java:method:: static NetworkResponse<List<Place>> autocomplete(String text)
   :outertype: API.Get

event
^^^^^

.. java:method:: static NetworkResponse<Event> event(long id)
   :outertype: API.Get

eventAttendance
^^^^^^^^^^^^^^^

.. java:method:: static NetworkResponse<ArrayList<User>> eventAttendance(long id)
   :outertype: API.Get

network
^^^^^^^

.. java:method:: static NetworkResponse<Network> network(long id)
   :outertype: API.Get

networkEvents
^^^^^^^^^^^^^

.. java:method:: static NetworkResponse<List<Event>> networkEvents(long id)
   :outertype: API.Get

networkPosts
^^^^^^^^^^^^

.. java:method:: static NetworkResponse<List<org.codethechange.culturemesh.models.Post>> networkPosts(long id)
   :outertype: API.Get

networkUsers
^^^^^^^^^^^^

.. java:method:: static NetworkResponse<ArrayList<User>> networkUsers(long id)
   :outertype: API.Get

post
^^^^

.. java:method:: static NetworkResponse<org.codethechange.culturemesh.models.Post> post(long id)
   :outertype: API.Get

postReplies
^^^^^^^^^^^

.. java:method:: static NetworkResponse<List<PostReply>> postReplies(long id)
   :outertype: API.Get

user
^^^^

.. java:method:: static NetworkResponse<User> user(long id)
   :outertype: API.Get

   The protocol for GET requests is as follows... 1. Check if cache has relevant data. If so, return it. 2. Send network request to update data.

userEvents
^^^^^^^^^^

.. java:method:: static NetworkResponse<ArrayList<Event>> userEvents(long id)
   :outertype: API.Get

userNetworks
^^^^^^^^^^^^

.. java:method:: static NetworkResponse<ArrayList<Network>> userNetworks(long id)
   :outertype: API.Get

userPosts
^^^^^^^^^

.. java:method:: static NetworkResponse<List<org.codethechange.culturemesh.models.Post>> userPosts(long id)
   :outertype: API.Get

