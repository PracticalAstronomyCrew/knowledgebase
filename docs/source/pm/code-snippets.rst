.. _code-snippets:

Code Snippets
=============

These are code snippets that can be helpfull to guide you through data analysis. These are general and need to be adjusted depending on the project and goal.

Creating a list of files in a directory
"""""""""""""""""""""""""""""""""""""""

.. code-block:: Python
   import subprocess
   subprocess.call("ls /net/vega/data/users/observatory/images/"+str(sys.argv[1])+"/STL-6303E/i/*BIAS* > /Users/users/*YOU*/rough/bias.list",shell=True)
   biasfiles = [line.rstrip('\n') for line in open("/Users/users/*YOU*/rough/bias.list")]

Making a median from a list of files
""""""""""""""""""""""""""""""""""""

.. code-block:: python
   from astropy.io import fits
   import numpy as np
   data_stack=[]
   for file in biasfiles
        data_stack.append(fits.getdata(file,1))
   medianBias = np.median(data_stack,axis=0)

Getting some header information
"""""""""""""""""""""""""""""""

.. code-block:: python
   from astropy.io import fits
   hdu = fits.open(file)
   exptime = hdu[0].header['EXPTIME']
   whole_header = fits.getdata(fits_image_filename, 0, header=True)

Writing a new fits file while keeping the header
""""""""""""""""""""""""""""""""""""""""""""""""

.. code-block:: python
   from astropy.io import fits
   hdu = fits.open(file)
   hdu[0].data= new_data
   hdu.writeto('new_filename.fits',overwrite=True)
   
Finding the number of counts of a round object using a circular aperture
""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

.. code-block:: python
   from photutils import CircularAperture
   from photutils import aperture_photometry
   aperture = CircularAperture([x, y], r=radius)
   phot_table = aperture_photometry(image, aperture, method='subpixel',subpixels=5)
   total_counts= phot_table['aperture_sum'][0]

How to make a date axis to plot
"""""""""""""""""""""""""""""""

.. code-block:: python
   import datetime
   dates=[]
   dates.append(datetime.datetime(year, month, day, hours, minutes, seconds))

Mask Cosmic Rays and Align Images
""""""""""""""""""""""""""""""""""

.. code-block:: python
   import numpy as np 
   from image_registration import chi2_shift
   from image_registration.fft_tools import shift 
   from astroscrappy import detect_cosmics  
   mask, clean1 = detect_cosmics(image1,gain=1.4,readnoise=15.2,sigclip=3) 
   mask, clean2 = detect_cosmics(image2,gain=1.4,readnoise=15.2,sigclip=3)
   print(np.count_nonzero(mask))  
   xoff, yoff, exoff, eyoff = chi2_shift(clean1, clean2, err=None, return_error=True, upsample_factor='auto') 
   corrected_image2 = shift.shiftnd(clean2, [-yoff, -xoff])print(xoff,yoff)
