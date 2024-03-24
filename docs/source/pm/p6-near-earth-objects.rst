.. _p6-near-earth-objects:

P06. Near Earth Objects
=======================

Observing Goals:
^^^^^^^^^^^^^^^^

You will observe the light curves of a selection of near earth objects..
Useful Background and References:

    * For your observing:

        * UpObjs -- https://asteroid.lowell.edu/upobjs/ this lets you know what Near Earth Asteroids are up in the sky you can enter the date, set parameters and it will create a list of possible objects. Make sure you set the V and H limits to the minimum (e.g. the brightest) ... we want to find the brightest ones possible. You can explore other parameters but can be best to leave them as broad as possible. I recommend that you don't set the galactic latitutde too far away from 15-20 (that is the miniumum distance out of the galaxy that it can be). Anything fainter than 17 in V will be difficult to do, unless it is particularly bright in H, in which case maybe we have some hope in the R and I bands.
        * Something like http://catserver.ing.iac.es/staralt/index.php that lets you plot the altitude of the object in the sky -- so you can decide what time, if any during your slot, it would be prime time to observe it.
        * There are other things that might be useful at: https://asteroid.lowell.edu/ so have an explore
        * Finally, most useful is the AstFinder https://asteroid.lowell.edu/astfinder/ where you can make finder charts of the object -- we will need these to make sure that we are in the right part of the sky. Some good settings:

            * Asteroid - is the name of the asteroid you found in 1 and 2
            * UTC Date - you can look at times during your observing run tomorrow -- but we will also need the Current UTC button to do this live in the observations
            * Observatory -- The closest to is is 013 --- Leiden which is fine for these purposes
            * Instrument FoV is ~30'
            * Future steps 5 in 5 mins is a good place to start.

Observation Planning:
^^^^^^^^^^^^^^^^^^^^^

    * Observation Time

        * You will be observing HALF a night shift.

    * Target Selection

        * Select as bright as possible targets that will be high in the sky in the sky during the observing time

    * Observations

        * It is best to use 3x3 binning for you observations to increase signal to noise, and reduce readout time.
        * You will observe the Near Earth object in the B,V and R filters over the duration of the night.
        * If possible, take standard star fields at the start, middle, and end of your observations to allow for calibration to the magnitude scale.
        * It is useful to be logged in to Kapteyn with the AstFinder tool and be able to *quickly* make those finder charts charts and send them to the printer "Spictor" (as opposed to ps0 ps1 etc..)... that sits in the observatory, then you can print and compare to where we are pointing in near real time... as these objects move fast across the sky this is important to do as you are observing.

    * Tools

        * Read the "Automatic filter changer" under "Tools for observing".

Data Ananlysis:
^^^^^^^^^^^^^^^

    * Data Reduction Basic Steps

        * Visit the page :ref:`data-reduction`

    * Further for this project

        * For each filter, you will do relative photometry (measuring brightness) over time to create a light curve.
        * Identify non-variable stars in the field to use as reference.

    * Further Analysis for this project

        * Plot the corrected magnitude of the Near earth Object as a function of time for each filter -- note that you should get the observation time from the header of the image, and account for the length of the exposure!
        * (You can also investigate if the colour between bands changes over time)

Results:
^^^^^^^^

Can you answer these questions with your work?

    * What is the shape of the variability? Is it sinusoidal or some other shape?
    * What is the period of the variability (the time between successive peaks or dips)?
    * What is the total amplitude of the variability? Does it change with different band?
    * Is the object rotating?
    * Does the colour of the object change with time?

Presenting your results:
^^^^^^^^^^^^^^^^^^^^^^^^

   - :ref:`a1-poster`
   - :ref:`a2-talk`
