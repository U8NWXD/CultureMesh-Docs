.. java:import:: android.content Context

.. java:import:: android.content.res TypedArray

.. java:import:: android.graphics Canvas

.. java:import:: android.graphics Color

.. java:import:: android.graphics Paint

.. java:import:: android.graphics.drawable Drawable

.. java:import:: android.text TextPaint

.. java:import:: android.util AttributeSet

.. java:import:: android.util Log

.. java:import:: android.view View

.. java:import:: android.widget EditText

ListenableEditText
==================

.. java:package:: org.codethechange.culturemesh
   :noindex:

.. java:type:: public class ListenableEditText extends EditText

   This is a custom EditText that allows us to listen for changes in cursor position. CreatePostActivity uses this view so that the format toggle buttons can update their settings when a new near_region in the edit text is selected.

Fields
------
mListener
^^^^^^^^^

.. java:field::  onSelectionChangedListener mListener
   :outertype: ListenableEditText

prevSelStart
^^^^^^^^^^^^

.. java:field::  int prevSelStart
   :outertype: ListenableEditText

Constructors
------------
ListenableEditText
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ListenableEditText(Context context)
   :outertype: ListenableEditText

ListenableEditText
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ListenableEditText(Context context, AttributeSet attrs)
   :outertype: ListenableEditText

ListenableEditText
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ListenableEditText(Context context, AttributeSet attrs, int defStyleAttr)
   :outertype: ListenableEditText

Methods
-------
onSelectionChanged
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void onSelectionChanged(int selStart, int selEnd)
   :outertype: ListenableEditText

setOnSelectionChangedListener
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setOnSelectionChangedListener(onSelectionChangedListener listener)
   :outertype: ListenableEditText

