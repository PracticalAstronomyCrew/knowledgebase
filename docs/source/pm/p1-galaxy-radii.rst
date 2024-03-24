.. _p1-galaxy-radii:

P01: Galaxy Radii
=================

Observing Goals:
^^^^^^^^^^^^^^^^

In this project you'll determine the *characteristic scales* of one
or two galaxies.

Useful Background and References:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

   *  `EllipticalGalaxies.pdf <https://www.astro.rug.nl/~sctrager/teaching/PoG/2013/EllipticalGalaxies.pdf>`__ or `DiskGalaxies.pdf <https://www.astro.rug.nl/~sctrager/teaching/PoG/2013/DiskGalaxies.pdf>`__
   *  The Photometry lecture from the Observational Astronomy Course

Observation Planning:
^^^^^^^^^^^^^^^^^^^^^
   * Observation Time

      *  You will be observing HALF a night shift.

   *  Target Selection

      *  We suggest first looking at the Messier objects to see if
         there's one available at the appropriate right ascension and
         declination. If you can't find an appropriate one, ask for
         help. **Group 1 should pick a spiral galaxy** and **Group 2
         should pick an elliptical galaxy** (note that sometimes more
         than one galaxy can be observed simultaneously!).

   *  Observations

      *  We suggest that you take images in at least two
         bands: :math:`B` and :math:`R`. If you have time, also take images in
         the :math:`V` band.
      *  To calibrate your data you should also observe standard star
         fields.

Data Analysis
^^^^^^^^^^^^^

   *  Data Reduction Basic Steps

      *  Visit the page :ref:`data-reduction`
      *  Produce artifact free images from your observations

   *  Further for this project

      *  You need to register and combine your images together, so that
         you have one final image per band
      *  You need to estimate (using the mode, rather than the mean or
         median) the sky background level in each band and take it off
         the image
      *  Locate the center of the galaxy in the images, and estimate the
         radius of the galaxy
      *  Next use and ellipse fitting program (in astropy) to fit
         ellipses from the center outwards, and create a surface
         brightness profile for the galaxy
   *  Further Analysis for this project

      *  Determine whether a de Vaucouleurs :math:`a^{\frac{1}{4}}` profile or an
         exponential :math:`\exp(a)` profile fits the surface brightness profile
         best
      *  Determine the scale length of the galaxy (the effective radius
         in the de Vaucouleurs profile, or the scale length of an
         exponetial fit)

Results: Can you answer these questions with your work?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

   *  Q1 what is the surface brightness profile of the galaxy, which
      model fits best, and what is the scale length?
   *  Q2 do the position angle and/or ellipticity of the isophotes
      change as a function of semi-major axis?  If so, why?
   *  Q3 for the elliptical galaxies (only), are the galaxies boxy or
      disky?  Does this change with semi-major axis?

Presenting your results:
^^^^^^^^^^^^^^^^^^^^^^^^

   - :ref:`a1-poster`
   - :ref:`a2-talk`
