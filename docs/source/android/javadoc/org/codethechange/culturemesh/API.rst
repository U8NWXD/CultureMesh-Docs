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

API
===

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type::  class API

   Created by Drew Gregory on 11/14/17. IMPORTANT: If you want to use this class in your activity, make sure you run API.loadAppDatabase() at the beginning of onPreExecute()/doInBackground(), and API.closeDatabase() in onPostExecute(). The app will crash otherwise. TODO: USE ALARMS FOR UPDATING DATA ON SUBSCRIBED NETWORKS TODO: Figure out how we can handle trying to update data. TODO: Figure out alternative to id's other than longs and ints, which cannot represent all numbers. (Maybe just use strings?) - Perhaps check if it comes from subscribed network, if not do network request instead of cache?

Fields
------
CURRENT_USER
^^^^^^^^^^^^

.. java:field:: static final String CURRENT_USER
   :outertype: API

FIRST_TIME
^^^^^^^^^^

.. java:field:: static final String FIRST_TIME
   :outertype: API

NO_JOINED_NETWORKS
^^^^^^^^^^^^^^^^^^

.. java:field:: static final boolean NO_JOINED_NETWORKS
   :outertype: API

PERSONAL_NETWORKS
^^^^^^^^^^^^^^^^^

.. java:field:: static final String PERSONAL_NETWORKS
   :outertype: API

SELECTED_NETWORK
^^^^^^^^^^^^^^^^

.. java:field:: static final String SELECTED_NETWORK
   :outertype: API

SELECTED_USER
^^^^^^^^^^^^^

.. java:field:: static final String SELECTED_USER
   :outertype: API

SETTINGS_IDENTIFIER
^^^^^^^^^^^^^^^^^^^

.. java:field:: static final String SETTINGS_IDENTIFIER
   :outertype: API

mDb
^^^

.. java:field:: static CMDatabase mDb
   :outertype: API

reqCounter
^^^^^^^^^^

.. java:field:: static int reqCounter
   :outertype: API

Methods
-------
addCities
^^^^^^^^^

.. java:method:: static void addCities()
   :outertype: API

addCountries
^^^^^^^^^^^^

.. java:method:: static void addCountries()
   :outertype: API

addEvents
^^^^^^^^^

.. java:method:: static void addEvents()
   :outertype: API

addNetworks
^^^^^^^^^^^

.. java:method:: static void addNetworks()
   :outertype: API

addPosts
^^^^^^^^

.. java:method:: static void addPosts()
   :outertype: API

addRegions
^^^^^^^^^^

.. java:method:: static void addRegions()
   :outertype: API

addReplies
^^^^^^^^^^

.. java:method:: static void addReplies()
   :outertype: API

addUsers
^^^^^^^^

.. java:method:: static void addUsers()
   :outertype: API

   This next section is code that parses JSON dummy data and adds it to the database. We can reuse some of this code later.

closeDatabase
^^^^^^^^^^^^^

.. java:method:: static void closeDatabase()
   :outertype: API

instantiatePost
^^^^^^^^^^^^^^^

.. java:method:: static void instantiatePost(org.codethechange.culturemesh.models.Post post)
   :outertype: API

   For simplicity, we store the id's of other model objects in the database, not the objects themselves. Thus, when we return these objects, we need to instantiate them.

   :param post:

instantiatePostReplies
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: static void instantiatePostReplies(List<PostReply> comments)
   :outertype: API

   For simplicity, we store the id's of other model objects in the database, not the objects themselves. Thus, when we return these objects, we need to instantiate them.

   :param comments: List of PostReplies with which we will get comments for.

instantiatePosts
^^^^^^^^^^^^^^^^

.. java:method:: static void instantiatePosts(List<org.codethechange.culturemesh.models.Post> posts)
   :outertype: API

   For simplicity, we store the id's of other model objects in the database, not the objects themselves. Thus, when we return these objects, we need to instantiate them.

   :param posts:

loadAppDatabase
^^^^^^^^^^^^^^^

.. java:method:: public static void loadAppDatabase(Context context)
   :outertype: API

subscribeUsers
^^^^^^^^^^^^^^

.. java:method:: static void subscribeUsers()
   :outertype: API

