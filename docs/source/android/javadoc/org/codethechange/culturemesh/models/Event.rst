.. java:import:: android.arch.persistence.room Embedded

.. java:import:: android.arch.persistence.room Entity

.. java:import:: android.arch.persistence.room Ignore

.. java:import:: android.arch.persistence.room PrimaryKey

.. java:import:: java.io Serializable

.. java:import:: java.math BigInteger

.. java:import:: java.util Date

Event
=====

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: @Entity public class Event extends FeedItem implements Serializable

   Created by nathaniel on 11/10/17.

Fields
------
address
^^^^^^^

.. java:field:: public String address
   :outertype: Event

authorId
^^^^^^^^

.. java:field:: public long authorId
   :outertype: Event

description
^^^^^^^^^^^

.. java:field:: public String description
   :outertype: Event

id
^^

.. java:field:: @PrimaryKey public long id
   :outertype: Event

networkId
^^^^^^^^^

.. java:field:: public long networkId
   :outertype: Event

timeOfEvent
^^^^^^^^^^^

.. java:field:: public String timeOfEvent
   :outertype: Event

title
^^^^^

.. java:field:: public String title
   :outertype: Event

Constructors
------------
Event
^^^^^

.. java:constructor:: public Event(long id, long networkId, String title, String description, String timeOfEvent, long author, String address)
   :outertype: Event

Event
^^^^^

.. java:constructor:: public Event()
   :outertype: Event

Methods
-------
getAddress
^^^^^^^^^^

.. java:method:: public String getAddress()
   :outertype: Event

getAuthor
^^^^^^^^^

.. java:method:: public long getAuthor()
   :outertype: Event

getDescription
^^^^^^^^^^^^^^

.. java:method:: public String getDescription()
   :outertype: Event

getTimeOfEvent
^^^^^^^^^^^^^^

.. java:method:: public String getTimeOfEvent()
   :outertype: Event

getTitle
^^^^^^^^

.. java:method:: public String getTitle()
   :outertype: Event

setAddress
^^^^^^^^^^

.. java:method:: public void setAddress(String address)
   :outertype: Event

setAuthor
^^^^^^^^^

.. java:method:: public void setAuthor(User author)
   :outertype: Event

setDescription
^^^^^^^^^^^^^^

.. java:method:: public void setDescription(String description)
   :outertype: Event

setTimeOfEvent
^^^^^^^^^^^^^^

.. java:method:: public void setTimeOfEvent(String timeOfEvent)
   :outertype: Event

setTitle
^^^^^^^^

.. java:method:: public void setTitle(String title)
   :outertype: Event

