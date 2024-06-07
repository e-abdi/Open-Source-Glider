Underwater Navigation
++++++++++++++++++++++++++

Dead reckoning
--------------------
This is the basic way all gliders navigate when they are underwater. The only inputs available to the glider at this point are its heading, attitude and depth. Therefore the glider inputs these parameters in its flight model and calculates where it thinks it should be at any moment. Once it completes a yo and surfaces, it can then measure the difference between where it thought it surface with where it actually  ended up by getting a new GPS fix, therefore calculating the average current faced by the glider during that yo which is called the depth-averaged current. 