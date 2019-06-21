Apply Kernel To Every Pixel
===========================

.. index::
   single: NeighborhoodOperatorImageFilter
   pair: kernel; pixel

Synopsis
--------

Apply a kernel to every pixel in an image.


Results
-------
.. figure:: input.png
  :scale: 70%
  :alt: input.png

  input.png

.. figure:: output.png
  :scale: 70%
  :alt: output.png

  output.png

Code
----

C++
...

.. literalinclude:: Code.cxx
   :lines: 18-

Classes demonstrated
--------------------

.. breathelink:: itk::NeighborhoodOperatorImageFilter
