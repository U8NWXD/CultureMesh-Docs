.. java:import:: android.arch.persistence.room Embedded

.. java:import:: android.arch.persistence.room Entity

.. java:import:: android.arch.persistence.room PrimaryKey

.. java:import:: java.io Serializable

.. java:import:: java.math BigInteger

Language
========

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: @Entity public class Language implements Serializable

   Created by nathaniel on 11/10/17.

Fields
------
language_id
^^^^^^^^^^^

.. java:field:: @PrimaryKey public long language_id
   :outertype: Language

name
^^^^

.. java:field:: public String name
   :outertype: Language

numSpeakers
^^^^^^^^^^^

.. java:field:: public int numSpeakers
   :outertype: Language

Constructors
------------
Language
^^^^^^^^

.. java:constructor:: public Language(long id, String name, int numSpeakers)
   :outertype: Language

Language
^^^^^^^^

.. java:constructor:: public Language()
   :outertype: Language

Methods
-------
toString
^^^^^^^^

.. java:method:: public String toString()
   :outertype: Language

