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

API.Post
========

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: static class Post
   :outertype: API

Methods
-------
addUserToEvent
^^^^^^^^^^^^^^

.. java:method:: static NetworkResponse<EventSubscription> addUserToEvent(long userId, long eventId)
   :outertype: API.Post

addUserToNetwork
^^^^^^^^^^^^^^^^

.. java:method:: static NetworkResponse addUserToNetwork(long userId, long networkId)
   :outertype: API.Post

event
^^^^^

.. java:method:: static NetworkResponse event(Event event)
   :outertype: API.Post

network
^^^^^^^

.. java:method:: static NetworkResponse network(Network network)
   :outertype: API.Post

post
^^^^

.. java:method:: static NetworkResponse post(org.codethechange.culturemesh.models.Post post)
   :outertype: API.Post

removeUserFromNetwork
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: static NetworkResponse removeUserFromNetwork(long userId, long networkId)
   :outertype: API.Post

reply
^^^^^

.. java:method:: static NetworkResponse reply(PostReply comment)
   :outertype: API.Post

user
^^^^

.. java:method:: static NetworkResponse user(User user)
   :outertype: API.Post

