.. _p7-globular-cluster-radii:

P07: Globular Cluster Radii
===========================
Observing Goals:
^^^^^^^^^^^^^^^^

In this project you will determine the surface brightness profile and a characteristic scale of a globular cluster (or clusters if there is sufficient observing time). 
Useful Background and References:

    * Information about King models http://adsabs.harvard.edu/abs/1995AJ....109..218T 
    * Core radii of globular clusters http://adsabs.harvard.edu/abs/1995AJ....109..218T

Observation Planning:
^^^^^^^^^^^^^^^^^^^^^

    * Observation Time

        * You will be observing HALF a night shift.

    * Target Selection

        * It is best to find a Messier object that is a Globular Cluster (something with an M-number) as those will likely be large and bright enough. Make sure your choice will be high in the sky during your obsering time.

    * Observations

        * Take images in the B and R bands at least, and also the V band if you have time.

        * Observe standard star fields so that you will be able to calibrate your results.

Data Analysis:
^^^^^^^^^^^^^^^

    * Data Reduction Basic Steps

        * Visit the page :ref:`data-reduction`
        * Register and combine your images so that you have one final image in each band.

    * Further for this project

        * Measure the sky brightness level in the images (e.g. in the corners) and remove this from the whole image.
        * Locate the center of the globular cluster in the image; here a contour plot can be very useful!
        * Next, measure the surface brightnes profile by fitting elipses moving outwards from the center (note there are astropy routines that help with this)

    * Further Analysis for this project

        * You can now plot your surface brightness profile and fit a King model. Find the value of the core radius from your fit and compare that to published results.

Results:
^^^^^^^^

Can you answer these questions with your work?

    * What is the surface brightness profile of your globlar cluster (or clusters)?
    * What are the King model fit parameters for your cluster (or clusters)?
    * How does your measured core radius compare with published results?

Presenting your results:
^^^^^^^^^^^^^^^^^^^^^^^^

   - :ref:`a1-poster`
   - :ref:`a2-talk`
