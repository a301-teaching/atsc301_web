.. include:: refs.txt

ATSC 301: radiation and remote sensing
======================================

:Instructor:   Dr. Phil Austin
:Email:        paustin@eos.ubc.ca
:Office:       EOS South 157, 604-822-2175
:Office hours: tbd

Course objectives
-----------------

By the end of this course you should have a good understanding of


1. how radiation is emitted, absorbed, transmitted and reflected by
   surfaces, clouds, and the atmosphere  (the "forward problem")

2. how radiometers, radars and lidars are used to infer 
   temperature and atmospheric constituents (the "inverse problem")

3. how to write clear, capable code that can ingest, manipulate and tranform
   data, and how to turn equations into computer algorithms in Python
   

Sample lecture learning objectives (provided with each lecture)
---------------------------------------------------------------

1. Understand the principals that determine satellite sensor wavelength, spatial
   resolution, sampling frequencies

2. Use standard satellite data archives to obtain and analyze global atmospheric
   and surface measurements

3. Calculate the net absorption/emission/scattering of the atmosphere
   given vertical profiles of temperature, gas, aerosol, clouds (the forward problem)

4. Use radiance measurements from satellites or ground based sensors to determine
   vertical profiles of temperature, :math:`CO_2` concentration, water vapor (the inverse problem)

5. Calculate rain rate, doppler velocities, attenuation given cloud drop size distributions

6. Calculate equilibrium temperature profiles for changing greenhouse gas concentrations

7. Use basic concepts from calculus and linear algebra to solve atmospheric problems

8. Write programs to analyze satellite and climate data


Evaluation
----------

:Assignments:                     25%
:Pre/in-class quizzes/exercises:  15%
:Mid-term:                        25%
:Final:                           40%

Required texts
--------------

* Wallace and Hobbs, 2006, *Atmospheric Science, an Introductory Survey*, Chapters 4 and 10 (UBC Bookstore, also used
  for ATSC 305)

* Stull, Practical meteorology, Chapters 2 and 8  (will be distributed)


Week by week topics
-------------------

      ======= =============  ===============================================
      Week 1  9/5 - 9/7      | Introduction, course outline, Python intro
                             | Assignment: install python
                             | Reading:  `How to think like a computer scientist`_

      Week 2  9/10 - 9/14    | Python continued
                             | Assignment: Use python for plotting and integration
                             | Reading:  notes, Stull Chapter 2:36-44

      Week 3  9/17 - 9/21    | Blackbody radiation, equilibrium temperature, 
                               Kirchoff's law, scattering and extinction 
                             | Assignment: MODIS cloud top properties
                             | Reading: WH 117-126
    
      Week 4  9/24 - 9/18    | Beers law, absorption/emission, 
                             | Assignment: two-stream code model 
                             | Reading:  W\&H 127-136
    
      Week 5  10/1 - 10/5    | Flux divergence/heating rates, Forward models
                             | Assignment: Atmospheric correction of satellite SSTs
                             | Reading:  notes, WH 130-132 Stull 2: 44-46 

      Week 6  10/10 - 10/12  | Atmospheric sounder: forward model
                             | Assignment: atmospheric sounder code
                             | Reading:  WH 132-136, Stull 8:219-226

      Week 7  10/15 - 10/19  | Satellites continued: AIRES instrument
                             | Assignment: mid-term review, mid-term

      Week 8  10/22 - 10/26  | Rain radar
                             | Assignment: Cloudsat precipitation data
                             | Reading:  Stull 8:240-248 plus handouts

      Week 9  10/29/- 11/2   | Doppler radar
                             | Assignment: Interpting doppler data
                             | Reading:  Stull 8:249-259 plus handouts
    
      Week 10 11/8 - 11/12   | Radiation and climate 
                             | Assignment: Validating climate model data
                             | Reading:  WH 419-422 plus handouts

      Week 11 11/14 - 11/16  | Water vapor, clouds and aerosols I
                             | Assignment: Calipso lidar data -- dust storms
                             | Reading:  handouts

      Week 12 11/19 - 11/23  | Water vapor, clouds and aerosos II
                             | Assignment: Calipso, Cloudsat and MODIS synthesis
                             | Reading:  handouts

      Week 13 11/26 - 11/30  | Catch-up, reiew

      ======= =============  ===============================================
