Signals
=======

.. _signals:
.. module:: fcm.signals

.. data:: device_registered

   Sent when a device is registered. Provides the following arguments:

   ``sender``
       The resource class used to register the device.

   ``device``
        An instance of ``fcm.models.Device`` (see :ref:`extending_device`)
        represents the registered device.

   ``request``
       The ``HttpRequest`` in which the device was registered.

.. data:: device_unregistered

   Sent when a device is unregistered. Provides the following arguments:

   ``sender``
       The resource class used to unregister the device.

   ``device``
        An instance of ``fcm.models.Device`` (see :ref:`extending_device`)
        represents the unregistered device.

   ``request``
       The ``HttpRequest`` in which the device was unregistered.
