.. _r03-narrow-lines:

R03: Calculating Narrow Lines
=============================

This assumes that you have observations in a Narrow Band filter and a Broad Band Filter that underlies (in wavelength) the Narrow Band Filter. The calculations assume that only one emission or absoprtion line is significant within the range of the broad band filter from the line source, and that the underlying continuum is well represented by other continuum sources in the image. 

Terms that are used:
--------------------

| :math:`f_B` the flux in the Broad Band Filter (e.g. B, V, R, I)
| :math:`f_N` the flux in the Narrow Band Filter (e.g. :math:`\mathrm{H\alpha}`, :math:`\mathrm{H\beta}`, [OIII], [SII])
|
| :math:`f_C` the continuum flux
| :math:`f_L` the line flux
|
| :math:`k` the observed filter scaling factor

Note that the fluxes that emerge will be in the same units as the fluxes in the broad band filter.

Steps:
------

First select a continuum source (or better repeat for several continuum sources) e.g. stars in your image. Your goal here is to find the conversion factor :math:`k` that allows you to scale between the broad and narrow filters.

**For the continuum source(s):**

.. math::

   f_B &= f_C \\
   f_N &= kf_C \\
   \therefore k &= \frac{f_N}{f_B}
   
When you have found your value for k (or average value for k, which is of course more reliable), you can look at your source of interest, which we want to break down into line and continuum fluxes.

**For the line + continuum source:**

.. math::

   f_B &= f_C + f_L \\
   f_N &= (kf_C) + f_L \\
   f_B - f_N &= f_C (1-k) \\
   \therefore f_C &= \frac{f_B - f_N}{1-k} \\
   \\
   f_L &= f_B - f_C \\
   &= f_B - \frac{f_B - f_N}{1-k} \\
   (1-k)f_L &= f_B - kf_B - f_B + f_N \\
   \therefore f_L &= \frac{f_N - kf_B}{1-k}
   
so you have now measured the Line flux from the source, separated from the continuum flux.

Multiple Lines on a single broad filter:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If you have the special case of multiple lines on top of a single broad band filter then the situation is of course more complex

**For the continuum source(s):**

.. math::

   f_B &= f_C \\
   {f_N}_1 &= k_1f_C \\
   {f_N}_2 &= k_2f_C \\
   \therefore k_1 &= \frac{{f_N}_1}{f_B} \\
   k_2 &= \frac{{f_N}_2}{f_B}
   
When you have found your values for :math:`k_1` and :math:`k_2` (or the average values), you can look at your source of interest, which we want to break down into line and continuum fluxes.

**For the line + continuum source:**

.. math::

   f_B &= f_C + {f_L}_1 + {f_L}_2 \\
   {f_N}_1 &= (k_1f_C) + {f_L}_1 \to (1) \\
   {f_N}_2 &= (k_2f_C) + {f_L}_2 \\
   &... \\
   {f_L}_1 + {f_L}_2 &= 2f_B - {f_N}_1 - {f_N}_2 - (2 - k_1 - k_2)f_C \\
   &... \\
   -f_B &= (k_1 + k_2 - 1)f_C - {f_N}_1 - {f_N}_2 \\
   \therefore f_C &= \frac{({f_N}_1 + {f_N}_2) - f_B}{k_1 + k_2 - 1}\\
   \\
   (1) \implies {f_L}_1 &= {f_N}_1 - k_1f_C \mathrm{\ (which\ can\ be\ used\ already)}\\
   &= {f_N}_1 - k_1\left( \frac{({f_N}_1 + {f_N}_2) - f_B}{k_1 + k_2 - 1}\right) \\
   \therefore {f_L}_1 &= \frac{(k_2 - 1){f_N}_1 - ({f_N}_2 + {f_B})/k_1}{k_1 + k_2 - 1} \\
   {f_L}_2 &= \frac{(k_1 - 1){f_N}_2 - ({f_N}_1 + {f_B})/k_2}{k_1 + k_2 - 1}

so you have now measured the Line fluxes from the source, separated from the continuum flux.

   
