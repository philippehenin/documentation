====================
Flashing the IoT box
====================

In some circumstances, such as after an Odoo version upgrade or when troubleshooting persistent
issues, the IoT box's SD card must be reflashed to be update it with the latest IoT image.
Reflashing can be performed using `balenaEtcher <https://etcher.balena.io>`, a free and open-source
tool for writing disk images to SD cards.

.. note::
   - A computer with a micro SD card reader/adapter is required to re-flash the micro SD card.
   - An alternative software for flashing the micro SD card is `Raspberry Pi Imager
     <https://www.raspberrypi.com/software/>`_.

#. Download `balenaEtcher <https://etcher.balena.io/#download-etcher>`_.
#. Go to `nightly <http://nightly.odoo.com/master/iotbox>`_, click :guilabel:`iotbox-latest.zip` to
   download the latest IoT image (compatible with with *all*  supported versions of Odoo), then
   extract the files.
#. Insert the IoT box's micro SD card into the computer or adapter.
#. Open balenaEtcher, click :guilabel:`Flash from file`, and select :file:`iotbox-latest.zip`.

   .. tip::
      You can also flash from a URL: Click :guilabel:`Flash from URL` and enter the following URL:
      `http://nightly.odoo.com/master/iotbox/iotbox-latest.zip`.

#. Click :guilabel:`Select target` and select the SD card.
#. Click :guilabel:`Flash` and wait for the process to finish.

.. image:: updating_iot/etcher-flash.png
   :alt:  Flashing the SD card with balenaEtcher