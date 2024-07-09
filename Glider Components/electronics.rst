Electronics
++++++++++++++++++

Both Seaglider and Slocum used a combination of Persistor CF2 and Tattletale 8 (TT8). Persistor was a microcontroller with a compact flash and Tattletale was a mini computer capable of running DOS. My understanding is that Persistor is used as a supervisor and would only turn to TT8 when specific tasks were going to be carried out. I believe this was done to both reduce the power consumption and add a layer of safety.
For our purposes, the initial idea is to design the system around `PX4 <https://docs.px4.io/main/en/>`_. Therefore, we will initially use one of the lower power autopilots compatible with PX4.


`Here <https://lucid.app/lucidchart/8746efec-c75f-44b0-9be7-4c806a048f1b/edit?viewport_loc=-11%2C-155%2C2219%2C1017%2C0_0&invitationId=inv_f7b1ec5a-b75d-4923-b846-12c5eede53f9>`_ you can find the current version of a top level block diagram. Again any comments and contributions are welcome.

.. image:: /images/blockdiagram.png
