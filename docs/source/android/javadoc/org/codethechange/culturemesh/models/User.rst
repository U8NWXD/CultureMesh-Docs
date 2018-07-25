.. java:import:: android.arch.persistence.room Entity

.. java:import:: android.arch.persistence.room PrimaryKey

.. java:import:: java.io Serializable

.. java:import:: java.math BigInteger

.. java:import:: java.util ArrayList

User
====

.. java:package:: org.codethechange.culturemesh.models
   :noindex:

.. java:type:: @Entity public class User implements Serializable

   Created by nathaniel on 11/10/17.

Fields
------
aboutMe
^^^^^^^

.. java:field:: public String aboutMe
   :outertype: User

email
^^^^^

.. java:field:: public String email
   :outertype: User

firstName
^^^^^^^^^

.. java:field:: public String firstName
   :outertype: User

id
^^

.. java:field:: @PrimaryKey public long id
   :outertype: User

imgURL
^^^^^^

.. java:field:: public String imgURL
   :outertype: User

lastName
^^^^^^^^

.. java:field:: public String lastName
   :outertype: User

role
^^^^

.. java:field:: public int role
   :outertype: User

username
^^^^^^^^

.. java:field:: public String username
   :outertype: User

Constructors
------------
User
^^^^

.. java:constructor:: public User(long id, String firstName, String lastName, String email, String username, String imgURL, String aboutMe)
   :outertype: User

User
^^^^

.. java:constructor:: public User()
   :outertype: User

Methods
-------
getEmail
^^^^^^^^

.. java:method:: public String getEmail()
   :outertype: User

getFirstName
^^^^^^^^^^^^

.. java:method:: public String getFirstName()
   :outertype: User

getImgURL
^^^^^^^^^

.. java:method:: public String getImgURL()
   :outertype: User

getLastName
^^^^^^^^^^^

.. java:method:: public String getLastName()
   :outertype: User

getUsername
^^^^^^^^^^^

.. java:method:: public String getUsername()
   :outertype: User

setEmail
^^^^^^^^

.. java:method:: public void setEmail(String email)
   :outertype: User

setFirstName
^^^^^^^^^^^^

.. java:method:: public void setFirstName(String firstName)
   :outertype: User

setLastName
^^^^^^^^^^^

.. java:method:: public void setLastName(String lastName)
   :outertype: User

setUsername
^^^^^^^^^^^

.. java:method:: public void setUsername(String username)
   :outertype: User

