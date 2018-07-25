.. java:import:: android.arch.persistence.room Embedded

.. java:import:: android.arch.persistence.room Entity

.. java:import:: android.arch.persistence.room PrimaryKey

.. java:import:: java.io Serializable

Network
=======

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: @Entity public class Network implements Serializable

   Created by nathaniel on 11/10/17.

Fields
------
fromLocation
^^^^^^^^^^^^

.. java:field:: @Embedded public FromLocation fromLocation
   :outertype: Network

id
^^

.. java:field:: @PrimaryKey public long id
   :outertype: Network

language
^^^^^^^^

.. java:field:: @Embedded public Language language
   :outertype: Network

nearLocation
^^^^^^^^^^^^

.. java:field:: @Embedded public NearLocation nearLocation
   :outertype: Network

networkClass
^^^^^^^^^^^^

.. java:field:: public boolean networkClass
   :outertype: Network

   networkClass is a boolean determining if a network is fromloc->nearLoc or language->nearLoc. true: fromLoc->nearLoc false: lang->nearLoc

Constructors
------------
Network
^^^^^^^

.. java:constructor:: public Network()
   :outertype: Network

   We don't have posts, events, and users fields because they are so large and often unnecessary. Instead, pass the id into an API.Get.networkUsers(), API.Get.networkEvents(), or or API.networkPosts() (asynchronously of course) to get these fields.

Network
^^^^^^^

.. java:constructor:: public Network(NearLocation nearLocation, FromLocation fromLocation, long id)
   :outertype: Network

Network
^^^^^^^

.. java:constructor:: public Network(NearLocation nearLocation, Language lang, long id)
   :outertype: Network

