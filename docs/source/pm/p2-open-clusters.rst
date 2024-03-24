.. _p2-open-clusters:

P02: Open Clusters
==================

Observing Goals:
^^^^^^^^^^^^^^^^

In this project you will observe an open cluster in two bands: B and V (and R, since it's easy to do), and determine the age and metallicity of the cluster.

Useful Background and References:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

    * isochrones for different age and compositions from http://stev.oapd.inaf.it/cgi-bin/cmd

Observation Planning:
^^^^^^^^^^^^^^^^^^^^^
    * Observation Time

        * You will be observing HALF a night shift.

    * Target Selection

        * You should select an open cluster that is available high in the sky for the duration of your observing time, and that is not too big

    * Observations

        * observe your open cluster in two bands: B and V (and R, since it's easy to do). Try to observe at least twice as long in the B band as the V band.
        * Your results will be much better if you take some observations to measure the bright stars, and some longer observations to observe the fainter stars (where the bright stars may be saturates)
        * To calibrate your observations you should also observe standard star fields

Data Ananlysis:
^^^^^^^^^^^^^^^

    * Data Reduction Basic Steps

        *  Visit the page :ref:`data-reduction`
        * Reduce the data to remove the instrumental effects

    * Further for this project

        * Register and Combine the images for each band
        * For each star in the image measure its B and V magnitude (and R) and create a Colour-Magnitude diagram

    * Further Analysis for this project

        * You can download individual isochrones for different age and compositions from http://stev.oapd.inaf.it/cgi-bin/cmd. You can use the defaults, except that the metallicity should be Z=0.0152 (not Z=0.019 as in the default), and you want to choose appropriate ages. If you want to change the composition, remember that we use :math:`[{\rm Fe/H}]=\log_{10} ({\rm Z/Z_{\rm solar}})`  — so change the composition in steps of, say, Delta [Fe/H] = 0.2 dex. The output file will contain the absolute magnitudes you need. Remember that m–M=5 log d[pc]–5, so the shift in magnitude between your (apparent) magnitudes and the isochrones gives the distance modulus. Any shift in color needed tells you about the extinction towards the cluster. Make sure you use the correct combination of magnitudes to compare with your data.

Results:
^^^^^^^^

Can you answer these questions with your work?

    * What is the distance to the cluster?
    * What are the the extinction and reddening to the cluster?
    * What is the age of the cluster?
    * What is the metallicity of the cluster (difficult: it's close to solar metallicity, but without a well-defined giant branch, this can be difficult to determine)

Presenting your results:
^^^^^^^^^^^^^^^^^^^^^^^^

   - :ref:`a1-poster`
   - :ref:`a2-talk`
