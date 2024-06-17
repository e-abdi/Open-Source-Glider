UVP6
++++++++++
Develosped by `LOV <https://www.obs-vlfr.fr/web/index.php>`_ and commercially available from `Hydroptic <http://www.hydroptic.com/index.php/public/Page/home>`_, this is a camera for detection and classification of particles in water. Currently it's mostly used for studying planktons. 
It automatically analyzes the frame and outputs a table of particle count for different size ranges. A standardized subset of this data can be transmitted back to shore in near-real-time and can even be uploaded and viewed on `EcoPART <https://ecopart.obs-vlfr.fr/>`_ depending on the level of integration as described in this document.
There are basically two basic ways to run UVP6 on gliders. One is simply by having a pre-defined acquisition profile on UVP6 and just supplying power. The second is to have two different profiles, one for depths above 100m and one below 
Please note that because the shape of this sensor and the constraints for its integration (must be in the nose for the least disturbed water flow), all gliders will have a less efficient flight mostly due to the added drag. This is something that needs to be taken into account.  

Seaexplorer
-----------
This integration was the earliest to be finalized and therefore is the most mature. Mostly because of the proximity of Alsemar to the Hydroptic, the sensor manufacturer.
They have both a very good mechanical integration and full software integration for real-time data.

.. image:: /images/uvpseaex.png

Slocum
------------
This physical integration was carried out by LOV/Hydroptic and the integration kit is commercially available from Hydroptic. The kit essentially allows the users to install and remove the UVP6 with minimal ballasting.
The software integration and flight tests were carried out under the `Bioglider <https://bioglider.eu/>`_ project. The software integration uses the Slocum Back Seat Driver and `Smart Cable <https://github.com/e-abdi/Smart-Cable>`_ as an interface. Therefore it requires a G3 Slocum with BSD and some wiring of a board inside your glider.
It is however possible to skip the full software integration and just supply power the UVP6 and have it record autonomously without any real-time data and no profile change according to depth.
For G2, there seem to be a new firmware release that includes BSD but users will need to contact Teledyne to see if you are eligible for getting that firmware!

.. image:: /images/uvpslo.png

Seaglider
---------------
This integration was carried out from scratch under the Bioglider project. After a few iteration of mechanical integrations, the last deployment in June 2024 resulted in a good Seaglider flight. This integration requires the user to modify their glider front fairing. This includes a few simple cuts of the fiberglass nose and replacing it with a plastic part which also acts as a bracket for the UVP6. 
The software integration uses the Seaglider LogDev interface together with the `Smart Cable <https://github.com/e-abdi/Smart-Cable>`_ to achieve a full integration with real-time data capability, however the data upload on EcoPART has not yet been tested.

.. image:: /images/uvpseag.jpg
