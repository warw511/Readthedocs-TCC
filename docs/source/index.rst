.. TCC userguide documentation master file, created by
   sphinx-quickstart on Thu Jul  2 13:32:52 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

###############################
TCC Web Application: User guide
###############################

.. toctree::
   :maxdepth: 2
   :caption: Contents:

************
Introduction
************

*****************************
TCC APPLICATION CONFIGURATION
*****************************
**!This doc is a test for creating a user guide. Edit this out when entire doc draft is finished.!**

The TCC application behavior is controlled through these
configuration Pages:

1. The Campus Configuration page
2. The device/criteria configuration page
3. The Agent Configuration page
4. The *Inputs* page
5. The *Outputs* page
6. The *Schedule* page 


Importing the Master Driver Configuration Store
***********************************************
At the initial homepage, the user will be prompted to upload the **Master Driver Configuration Store** file. Values within the Master Driver Configuration Store will be parsed to provide options for Campus, Building, Time Zone and Points throughout the application.

.. image:: _images/master_Driver.jpg


Once the user has selected the Master Driver Configuration Store, this homepage will not appear again. However, if the user needs to upload a different Master Driver Configuration Store at any point, this option can be accessed via the Menu icon in the top left of the application.

.. Warning:: Uploading a new Master Driver Configuration Store will remove all current data in the application.

.. image:: _images/hamburger_Drop.jpg

Campus Configuration
********************

When a Master file has been uploaded, the application will go into the *Campus Configuration*
page. The first selections that will be shown are the *Campus*, *Building*, and *Time Zone* dropdown's. 

.. image:: _images/campus_Page.jpg

.. image:: _images/campus_Config.jpg

**Campus** 
   The campus name as published by the VOLTTRON
   platform.driver service. 

**Building**
   The building name as published by the VOLTTRON
   platform.driver service.

**Time Zone**
   Time Zone has default strings implemented into the program.

 