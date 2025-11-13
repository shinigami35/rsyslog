.. _param-omhttp-healthchecktimedelay:
.. _omhttp.parameter.input.healthchecktimedelay:

healthchecktimedelay
==================

.. index::
   single: omhttp; healthchecktimedelay
   single: healthchecktimedelay

.. summary-start

Sets the number of seconds omhttp waits before performing an other request to the Health Check URL.
This parameter is disable by default.
To disable, use "-1" as value.

.. summary-end

This parameter applies to :doc:`../../configuration/modules/omhttp`.

:Name: healthchecktimedelay
:Scope: input
:Type: integer
:Default: input=30
:Required?: no
:Introduced: Not specified

Description
-----------
The time after which the health check will be done in seconds.

Input usage
-----------
.. _omhttp.parameter.input.healthchecktimedelay-usage:

.. code-block:: rsyslog

   module(load="omhttp")

   action(
       type="omhttp"
       healthchecktimedelay="60"
   )

See also
--------
See also :doc:`../../configuration/modules/omhttp`.
