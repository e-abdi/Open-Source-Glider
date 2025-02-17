Background
++++++++++++++
For people who are not coming from Ocean Studies background (as this was the case for me), it might be useful to start with a basic introduction to different types of platforms and systems used to study the oceans. This will help appreciating the gliders for the amazing tool they are but also knowing their limitation. 

Stationary
==============
The simplest type of stationary platform is a buoy held at the same position with an anchor. These are widely used as weather stations.
A mooring is basically a structure with an anchor that can have a surface buoy or it can be completely submerged with sensors at several depths and then recovered using some kind of release mechanism.
A lander is a type of mooring that basically just sits on the seafloor and measures some variable such as currents.

Moving
================
Non-steerable
-------------------
The simplest kind of moving platform is called a drifter. It's basically a buoyant structure that drifts on the water surface with currents and transmits information such as it's location at some specified intervals.  Check out `this <https://www.onelessbottle.org/oceantracking/>`_ project where they used a simple water bottle as a drifter. 

A float is a device that can monitor water column by changing its buoyancy and basically floating up and down with no steering capability. Probably the best example of standardization in the ocean is the `Argo <https://en.wikipedia.org/wiki/Argo_(oceanography)>`_ float program where they have standards in everything. All the way from hardware to data. 
A French team has designed a low-cost float `here <https://github.com/ThomasLeMezo/seabot/tree/master>`_.

.. image:: /images/argo.jpg

Steerable
------------------------
Surface Vehicles
============================
There are a few interesting systems in this category such as the `Waveglider <https://www.liquid-robotics.com/wave-glider/how-it-works/>`_, `Autonaut <https://www.autonautusv.com/>`_ and `Saildrone <https://www.saildrone.com/>`_ but my favorite is a a simple autonomous sail boat called `SailBuoy <http://www.sailbuoy.no>`_. This is probably one of the most elegantly designed vehicles I have seen in this field. It just does what it needs to do, efficiently and  robustly.

.. image:: /images/sailbuoy.jpg

Subsea vehicles
============================
Tethered
-------------------
ROV is probably the best known ocean-going platform since it's basically an underwater drone.


.. image:: /images/bluerov.jpg

Untethered
-------------------------
These are called Autonomous Underwater Vehicles or AUVs. AUVs usually have one or more propeller and some kind of acoustic navigation system. They are usually used for short missions (one day to a week or so) to cover a relatively large area with precision. 

.. image:: /images/auv.jpg

A glider is considered a type of AUV, but the main differences are that:

- It's completely autonomous for hours at a time
- Its propulsion system requires it to move up and down the water column in a sawtooth pattern in order to move forward. 
- It usually has a very long endurance (in the order of few months)
- It can cover extremely large distances, such as the the Atlantic ocean
- It's quite slow; around 1 knot


An underwater glider works on a similar principle as normal air glider where the medium is water. There is no propeller in either glider, but the main difference is that unlike air gliders, underwater gliders use a neat trick to climb back the water column after gliding down. They do this by changing their density. Gliders are carefully designed to have a density very close to that of water. Then by simply changing their volume (which can be achieved using a simple piston pump or an inflating oil bladder), they can change their density and use the buoyancy force to fly up and down the water column.
By moving a large weight internally (usually the battery pack) it can control its pitch and by rotating the weight, it can roll and therefore fly towards a certain heading. 

There is a partial vacuum inside the glider. This serves a few purposes: 

- Sucking all the seal joints together, creating a tighter seal
- By monitoring the internal pressure we will know right away if there is a leak somewhere. 
- In order to get oil from external bladder inside the glider, we just open a solenoid valve and the air pressure pushes the oil inside so we save power on pumping
