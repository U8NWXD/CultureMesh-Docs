.. java:import:: android.content Context

.. java:import:: android.content DialogInterface

.. java:import:: android.support.v7.app AlertDialog

.. java:import:: java.util Random

NetworkResponse
===============

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class NetworkResponse<E>

   Class to store responses after attempting networking tasks

Constructors
------------
NetworkResponse
^^^^^^^^^^^^^^^

.. java:constructor:: public NetworkResponse()
   :outertype: NetworkResponse

   Constructor that randomly chooses a failure state and a generic message based on that state

NetworkResponse
^^^^^^^^^^^^^^^

.. java:constructor:: public NetworkResponse(boolean inFail)
   :outertype: NetworkResponse

   Constructor that creates a generic message based on "inFail"

   :param inFail: Failure state provided by user (true if failed)

NetworkResponse
^^^^^^^^^^^^^^^

.. java:constructor:: public NetworkResponse(boolean inFail, int inMessageID)
   :outertype: NetworkResponse

   Constructor that sets message and failures state based on arguments

   :param inFail: Failure state provided by user (true if failed)
   :param inMessageID: ID for string resource containing message

NetworkResponse
^^^^^^^^^^^^^^^

.. java:constructor:: public NetworkResponse(E inPayload)
   :outertype: NetworkResponse

   Constructor that stores a payload and sets the failure state to false

   :param inPayload: Payload returned by networking request

NetworkResponse
^^^^^^^^^^^^^^^

.. java:constructor:: public NetworkResponse(boolean inFail, E inPayload)
   :outertype: NetworkResponse

   Constructor that both stores a payload and sets the failure state from parameters

   :param inFail: Whether or not the network operation failed
   :param inPayload: Payload returned by networking request

NetworkResponse
^^^^^^^^^^^^^^^

.. java:constructor:: public NetworkResponse(boolean inFail, E inPayload, int messageID)
   :outertype: NetworkResponse

   Constructor that both stores a payload and sets the failure state from parameters

   :param inFail: Whether or not the network operation failed
   :param inPayload: Payload returned by networking request

Methods
-------
fail
^^^^

.. java:method:: public boolean fail()
   :outertype: NetworkResponse

   Check whether the network request failed

   :return: true if the request failed, false if it succeeded

getErrorDialog
^^^^^^^^^^^^^^

.. java:method:: public AlertDialog getErrorDialog(Context context)
   :outertype: NetworkResponse

   Get an error dialog that can be displayed to show message from messageID to user

   :param context: Context upon which to display error dialog
   :return: Dialog that can be shown

getMessageID
^^^^^^^^^^^^

.. java:method:: public int getMessageID()
   :outertype: NetworkResponse

   Get the resource ID of the message to display to the user

   :return: Resource ID of message

getPayload
^^^^^^^^^^

.. java:method:: public E getPayload()
   :outertype: NetworkResponse

   Get the payload returned by the network operation

   :return: Payload returned by network operation

showErrorDialog
^^^^^^^^^^^^^^^

.. java:method:: public void showErrorDialog(Context context)
   :outertype: NetworkResponse

   Show an error dialog that can be displayed to show message from messageID to user

   :param context: Context upon which to display error dialog

