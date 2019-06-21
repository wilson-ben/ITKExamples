Apply A Filter Only To A Specified Region Of An Image
=====================================================

.. index::
   single: DerivativeImageFilter
   pair: image; random

Synopsis
--------

To apply a filter to only operate on a specified ImageRegion.


Results
-------
Output::

  Created random image.
  Computed derivative.

Code
----

C++
...

.. literalinclude:: Code.cxx
   :lines: 18-

Classes demonstrated
--------------------

.. breathelink:: itk::DerivativeImageFilter
