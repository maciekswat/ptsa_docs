.. PTSA documentation master file, created by
   sphinx-quickstart on Wed Jun  1 13:07:22 2016.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

PTSA - EEG Time Series Analysis in Python
=========================================

**PTSA**  is an open source project and Python package that facilitates time-series
analysis of EEG signals using Python. PTSA builds on xarray functionality
and provides several convenience tools that significantly simplify analysis of the EEG data..

To use all features provided by PTSA you will need to install several dependencies:
xarray, scipy, numpy, PyWavelets and make sure you have working c/c++ compiler on your machine when you install PTSA

The main object that you will be interacting in PTSA is called ``TimeSeriesX``
(**X** in ``TimeSeriesX`` signifies the fact that ``TimeSeriesX`` is a subclass of ``xarray.DataArray``).
Besides, PTSA has 3 main categories of objects: readers, writers, filters. Readers ,
read various data formats (e.g eeg files, bipolar electrodes files etc..) to make input operations as smooth as possible.
Writers (still under development) will output data in several formats (currently only NetCDF output is supported). Filters
take as an input ``TimeSeriesX`` object and output diffrent ``TimeSeriesX`` object. Most of the tasks
related to EEG analysis will rely on using those 3 categories of PTSA objects.





Contents:

.. toctree::
   :maxdepth: 1

   installation
   faq




Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

