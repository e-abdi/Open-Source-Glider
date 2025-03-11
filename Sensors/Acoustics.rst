Acoustics
++++++++++
Electromagnetic waves get severely attenuated in salt water so sound is the name of the game for communication, navigation and object detection and characterization underwater. For a fantastic deep dive into the science of sound in the sea I recommend taking a look at `this <https://dosits.org/>`_ website. Also `Blue Robotics <https://bluerobotics.com/learn/a-smooth-operators-guide-to-underwater-sonars-and-acoustic-devices/>`_ has a great guide about acoustics.


Passive
==============

Hydrophones
---------------

Basically a microphone that's molded inside a resin (preferably) with the same density as that of water. 
The hydrophone element is simple. Although the sensitivity can vary greatly, you can build an extremely simple hydrophone using a piezo ceramic element and some resin around it. What you do with the signal is the important and tricky part! In commercial hydrophones, the most expensive thing you pay for is the calibration. We don't need to worry about that for our purposes here, nevertheless I will go through some of the commercial units I have worked with.

Ocean Sonics
^^^^^^^^^^^^^^^^^^^^^^^^^^

Their icListen hydrophones have some nice capabilities. You will get a web interface for the unit in which you can view the live spectrogram, change settings and download files. You also have some simple detection capability in which you can get a notification when a sound level of your chosen frequency range above a set threshold. I have integrated this hydrophone on a Seaglider and designed a board to transmit back these detection events in addition to a text version of the spectrogram events back to shore after every surfacing. 
They are also a good choice if you want to have a mooring with hydrophones. If you use a low power GSM modem, you can easily have a direct connection to a hydrophone deployed a few kilometers away from the shore like we did `here  <https://www.orcaireland.org/smartwhalesounds>`_.

The downside is that they are quite expensive especially compared to something like a SoundTrap. 

SoundTrap
^^^^^^^^^^^^^^^^^^^^^^^^
They make well-designed and relatively affordable hydrophones. I can definitely recommend these. I haven't used these on gliders yet but it should be fairly straightforward to attach one of these to a glider.

Jasco
^^^^^^^^^^^^^^^^^^^^^^^^
They have the most advanced but then also the most expensive hydrophone systems like the `Ocean Observer <https://www.jasco.com/oceanobserver>`_. 

Hydrophone array
--------------------
Hydrophones are usually omnidirectional so in order to get a bearing on the sound source, you either need to use something like a `vector sensor <https://dosits.org/galleries/technology-gallery/basic-technology/vector-sensors/>`_ (which is basically impossible to get a hold of one of these because of their military application) or you could use multiple hydrophones. In order to localize a source three dimensions, you need at least four hydrophones. 

Active
==================

Echo-sounder
--------------

The most basic type of sonar used for detecting the bottom and other targets throughout the water column such as fish





Multibeam
--------------------

These systems use hundreds of beams to get a three dimensional mapping of both seabed and the water column. 

Side-scan sonar
--------------------

These sensors have a transducer array which sends and receives acoustic pulses as it's being towed underneath or behind a vessel at a constant speed. Doing this they can reconstruct an image of the received echos that represents the seafloor and what's on it using dark and bright areas. This is mainly used to cover a large area relatively quickly and inexpensively when looking for a specific feature such as a shipwreck.


Sub-buttom profiler
---------------------------

A system used to penetrate the seafloor and provide an image of subsurface geological layers. 

ADCP
----------------

Stands for acoustic Doppler current profiler and as the name suggests, it uses the doppler shift in the received echos to determine the currents. These are usually deployed on a stationary platform such as a lander or a mooring but they have been integrated and used on all the major gliders as well. Making sense of the data they collect from a moving underwater vehicle however, is a challenging task.


DVL
--------------------

Stands for doppler velocity logger, and it uses yet again the doppler shift to keep track of speed and direction of an underwater vehicle relative to a solid object such as the seafloor or ice.