.. _p9-asteroid-light-curve:

P09: Asteroid Light Curve
=========================

Observing Goals:
^^^^^^^^^^^^^^^^

You will observe the light curve of a asteroid
Useful Background and References:

    * A list of currently "in the sky" asteroids is available at: https://in-the-sky.org/data/asteroids.php
    * Here are a :download:`Jupyter Notebook </files/Asteroid_LC.ipynb>` and a :download:`csv data file </files/lc_summary.csv>` which let you find properties of asteroid light curves (from the PSI Asteroid Light Curve Database)
    * Make finder charts: https://theskylive.com/ (The search here is quite bad -- but if you use google for the name of the asteroid, you can find the skylive link that way)

Observation Planning:
^^^^^^^^^^^^^^^^^^^^^

    * Observation Time

        * You will be observing a FULL night.

    * Target Selection

        * Select a target that will reach its highest point in the sky at around 1:30am (half way between sunset and sunrise). Possible targets can be found using in the sky, and looking for relativelyy bright, short term variable, asteroids

    * Observations

        * You will observe the asteroid in the B,V and R filters over the duration of the night
        * If possible, take standard star fields at the start, middle, and end of your observations to allow for calibration to the magnitude scale.

Data Ananlysis:
^^^^^^^^^^^^^^^

    * Data Reduction Basic Steps

        *  Visit the page :ref:`data-reduction`

    * Further for this project

        * Next you need to align all of your images -- but do not combine them
        * For each filter, you will do relative photometry (measuring brightness) over time to create a light curve
        * Identify other, non-variable, stars in the field to use as reference

    * Further Analysis for this project

        * Plot the corrected magnitude of the star as a function of time for each filter -- note that you should get the observation time from the header of the image, and account for the length of the exposure!
        * (You can also investigate if the colour between bands changes over time)

Results: 
^^^^^^^^^

Can you answer these questions with your work?

    * What is the shape of the variability? Is it sinusoidal or some other shape?
    * What is the period of the variability (the time between successive peaks or dips)?
    * What is the total amplitude of the variability? Does it change with band?
    * Does the asteroid's colour change with time?
    * What kind of asteroid is this? Why do these asteroids vary in this way?

Presenting your results:
^^^^^^^^^^^^^^^^^^^^^^^^

   - :ref:`a1-poster`
   - :ref:`a2-talk`
