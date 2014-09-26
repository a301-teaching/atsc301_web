.. include:: refs.txt

.. toctree::
   :hidden:

   week 1 <week1_submissions>  
   stull <stull>
   
=====================
 Week by week topics
=====================

.. _week1:

Week 1  9/1 - 9/5
=================

Day 1: Wednesday, September 3
-----------------------------

* Learning objectives: get comfortable with simple functions
  and plotting in python
* Assignment: get computer lab account and password ($25) from main office front desk
* Assignment: Due Thursday:  Week 1: Programming Problem on Connect:  `week1.txt <week1.txt>`_
* Reading for Friday:  Install anaconda python and work through as much of `Python crash course`_
  and `Introduction to Python programming`_  as you can in 3 hours

Day 2: Friday, September 5
--------------------------

* My answer for the Wednesday assignment `week1.ipynb <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/35475c23aec925399ead0a77d8797c44f102c89e/notebooks/week1.ipynb>`_

  :ref:`submissions`
  
* Reading for Monday: Stull Chapter 2 pp. 27-34

.. _assign_mon_sept_8:  
  
Assignment for Day 3: Monday Sept. 8
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  
* Assignment for Monday -- before Monday 10 am upload an IPython notebook to Connect that does as much as you can of the following tasks:

  * Use the examples in `Johansson Lecture 1 <http://nbviewer.ipython.org/github/jrjohansson/scientific-python-lectures/blob/master/Lecture-1-Introduction-to-Python-Programming.ipynb>`_  to define a function to calculate `Stull 2.6 <text/stull_chap2_eqn2_6.pdf>`_  to find :math:`\Psi`, the local elevation angle in degrees

  * Evaluate your function for the hours between 3 and 21 and show that the elevation angle agrees with the solved example
    for Vancouver, BC on 22 Dec, 23 Mar. and 22 Jun   (don't have to make a plot, just printing the numbers is ok

Week 2  9/8 - 9/12
==================

* Week 2: Learning objectives

  * Learning goals: Introduce wavenumber, field of view, radiance and irradiance,
    blackbody radiation, Stefan-Boltzman, Wien's Law, equilibrium temperature, Kirchoff's law


Day 4: Monday Sept. 8
---------------------

* Go over the `elevation notebook <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/day3_elevation.ipynb>`_

* Do the "white paper" exercise

* Assignment for Wednesday:  Read Stull pp. 34-38 on flux and blackbody radiation and
  Wallace and Hobbs pp. 113-118 on radiation and complete the `Stefan-Boltzman notebook <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/stefan_boltzman.ipynb>`_

Day 4: Wednesday Sept. 10
-------------------------

* finish white paper example

* go over `the stefan-boltzman answer <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/stefan_boltzman_answer.ipynb>`_

* work with the `planck function library <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/plotplanck.ipynb>`_

* Assignment for Friday:  Read my `Notes on geometry and planck function`_
  and complete `the derivitives notebook <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/derivatives.ipynb>`_
  
Day 5: Friday Sept. 12
----------------------

* Go over the `Notes on geometry and planck function`_ handout

* Review `derivitives solution <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/wiens_law.ipynb>`_

* For Monday, read W&H 116 to 122 and my `Notes on radiative equilibrium`_

* Finish and upload my `Wien's law for wavenumber notebook <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/wiens_law_wavenumber.ipynb>`_


Week 3  9/15 - 9/20
===================

* Learning goals: get calibrated radiances from MODIS data


Day 6: Monday Sept. 15
----------------------

* Review `Wien's wavenumber solution <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/wiens_law_wavenumber_solution.ipynb>`_

* Introduce MODIS -- assignment for Wednesday

  - Take a look at `the MODIS website <http://modis.gsfc.nasa.gov/about/>`_ .
    Click on and read the pages about the design concept, components and
    specification.

  - Do the same for this article about 
    `Terra, Aqua, and the A-train <http://www.spacetoday.org/Satellites/TerraAqua/ATrain.html>`_

  - Following the in-class demo -- go to 
    http://ladsweb.nascom.nasa.gov  and downoad a level1b (geolocated
    and calibrated radiances) collection 5.1 data granule that contains something
    you're interested in looking at (Area 51, your hometown, etc.)

    You can see a screencast on `my youtube channel`_

  - Upload that hdf file to the dropbox you shared with me
    
* Catch up with the `Notes on geometry and planck function`_ handout and
  `Notes on radiative equilibrium`_  

Day 7: Wednesday, Sept. 17
--------------------------

* Read a Modis netCDF file using the `satellite notebook <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/satelliteI.ipynb>`_

* For Friday: do the two analytical problems in the `analytic wiens notebook <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/analytic_wiens.ipynb>`_


Day 8: Friday, Sept. 19
-----------------------

* go over the `wiens analytic notebook solution`_

* Continue with the `satellite notebook`_

* For Monday, upload your solution to the `inverse planck problem`_  (by 10am on connect)

* read: Stull 35-45 on radiation principles  and Wallace and Hobbs 118-122 on Kirchoff's law and the Greenhouse effect

Week 4  9/22 - 9/27
===================

* Learning objectives -- map calibrated, navigated MODIS radiances

* Solve for a two layer atmosphere in radiative equilibrium

Day 9: Monday, Sept. 22
-----------------------

* Go over the solution to the `Inverse Planck Notebook <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/inverse_planck_sol.ipynb>`_
  and `Planck wavenum <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/wiens_law_wavenumber_solution.ipynb>`_

* Objective:  invert level1b channel 31 11 micron radiances for brightness temperatures

* Go over `satelliteII <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/satelliteII.ipynb>`_ exercise
  to calculate the brightness temperature for Modis Channel31 radiances on a 0.05 x 0.05 lat/lon grid.


Day 10: Wed., Sept. 24
-----------------------

* Go over the `satellite3 notebook <http://nbviewer.ipython.org/github/a301-teaching/classcode/blob/master/notebooks/satellite3.ipynb>`_ which uses matplotlib's
  pcolormesh function to make color images of regularly gridded 2-d arrays


Day 11: Fri., Sept. 26
-----------------------

* Go over the satellite4 notebook, which plots a 500 x 500 pixel image of the Channel 1 reflectivity.

* Assignment for Monday:

  1. hand in you won version of my satellite4 notebook which replaces the multiple calls to the gridding routine::

        sat_array=np.zeros([len(lat_bins),len(lon_bins)],dtype=np.float)

        for point_num in range(len(lat_indices)):
            bin_row=lat_indices[point_num]
            bin_col=lon_indices[point_num]   
            sat_array[bin_row,bin_col]=sat_array[bin_row,bin_col] + sat_data.flat[point_num]

        for i in range(lon_array.shape[0]):
            for j in range(lon_array.shape[1]):
                if bin_count[i,j] > 0:
                    sat_array[i,j]=sat_array[i,j]/bin_count[i,j]
                else:
                    sat_array[i,j]=np.nan

     with a function that takes lat_bins, lon_bins and sat_data and returns a gridded sat_array. 

  2. Read Wallace and Hobbs 122-134, focussing on the topics that overlap with my `Notes on Beers law`_
     For Wednesday, do W&H problems 4.20, 4.21, 4.22, 4.23, 4.30, and prove that Kirchoff's law holds
     for an absorbing and transmitting gas using the thought experiment discussed in class.
     

