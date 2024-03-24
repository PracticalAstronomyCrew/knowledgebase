.. _p12-satellite-constellations:

P12: Consequences of Satellite Constellations
=============================================

Observing Goals:
^^^^^^^^^^^^^^^^

In this project you will observe regions of the sky to determine the rate at which satelites are currently observed in the skies above us.
Useful Background and References:

    * Finding Satellites:

        * https://heavens-above.com/AllSats.aspx?lat=0&lng=0&loc=Unspecified&alt=0&tz=UCT can produce maps of satellite paths (with half degree grid to zoom in to)
        * https://in-the-sky.org/satpasses.php provides a tool to locate upcoming satellite passes, you may be particularly interested in clustered staellite constellations
        * https://www.n2yo.com/ provides coordinates and tracks for any satellite

    * About the consequences of satellite constellations:

        * https://www.iau.org/news/pressreleases/detail/iau2001/
        * https://www-nature-com.proxy-ub.rug.nl/articles/s41550-020-01238-3
        * https://www-aanda-org.proxy-ub.rug.nl/articles/aa/full_html/2020/04/aa37501-20/aa37501-20.html

Observation Planning:
^^^^^^^^^^^^^^^^^^^^^

    * Observation Time

        * You will be observing HALF a night shift.

    * Target Selection

        * You can choose to sample random regions of the sky, or you can select regions where you anticipate that satelites may pass
        * The default in the tool is 4th magnitude, but you should be able to find sattelites much fainter than that 

    * Observations

        * In the region of the sky that you choose you should take a series of short (~60 sec) observations, in quick succession
        * The LUM filter at LDST allows for a broad band collecting all light
        * So that you can calibrate the brightnesses of the satellites, you should observe standard star fields at a range of airmasses, using all of the LDST filters.

Data Ananlysis:
^^^^^^^^^^^^^^^


    * Data Reduction Basic Steps

        *  Visit the page :ref:`data-reduction`
        * Reduce the images to remove artefacts

    * Further for this project

        * For each region you observe, you should create a median image from all observations to act as the background
        * You can then subtract that background from each individual image to identify transient events (such as satellites)

    * Further Analysis for this project

        * When you have identified a satellite path, produce some calibrated properties such as magnitude
        * You should make a brightness profile along the path of the satellite -- does it show any signs of rotation or changing reflectivity?
        * Perform astrometry on your background image to get precise coordinates and timing for the satellite

Results: 
^^^^^^^^^

Can you answer these questions with your work?

    * Q1: For targeted observations of satellites or clusters of satellites, did you observe the satellites expected? What were their magnitues? What else can you say about the consequences for observations?
    * Q2: For randomly selected regions of sky what can you say about statistics for how much observations are affected by satellite constellations? Taking the field of view of this telescope into account, what could you say about the consequences for wide field survey telescopes? Can you provide statistics for observers in Groningen about what to expect in terms of satellites interfering with observations?
    * Q3: Using astrometry and timing to can you use look up tools to identify specific satellites that were in your observations?

Presenting your results:
^^^^^^^^^^^^^^^^^^^^^^^^

   - :ref:`a1-poster`
   - :ref:`a2-talk`
