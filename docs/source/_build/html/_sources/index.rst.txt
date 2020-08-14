.. TCC userguide documentation master file, created by
   sphinx-quickstart on Thu Jul  2 13:32:52 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

###############################
TCC Web Application: User Guide
###############################

.. toctree::
   :maxdepth: 2
   

************
Introduction
************

*****************************
TCC Application Configuration
*****************************
**!This doc is a test for creating a user guide. Edit this out when entire doc draft is finished.!**

The TCC application behavior is controlled through these
configuration Pages:

1. The Campus Configuration page
2. The Device/Criteria configuration page
3. The Agent Configuration page
4. The *Inputs* page
5. The *Outputs* page
6. The *Schedule* page 


Importing the Master Driver Configuration Store
***********************************************
At the initial homepage, the user will be prompted to upload the **Master Driver Configuration Store** file.
Values within the Master Driver Configuration Store will be parsed to provide options for Campus, Building,
Devices, Topics, and Points throughout the application.

.. image:: _images/master_Driver.JPG

Once the user has selected the Master Driver Configuration Store, this homepage will not appear again. However, if the user needs to upload a different Master Driver Configuration Store at any point, this option can be accessed via the Menu icon in the top left of the application.

If a new file needs to be uploaded to the application, in the top left corner of the screen there will be a *hamburger dropdown* icon.

.. image:: _images/hamburger_Drop.JPG

Once this item is selected, there will be two options to choose from. 

.. image:: _images/hamburger_Button.JPG

.. Warning:: Uploading a new Master Driver Configuration Store will remove all current data in the application.


Campus Configuration
********************

When a Master file has been uploaded, the application will go into the *Campus Configuration*
page. The first selections that will be shown are the *Campus*, *Building*, and *Time Zone* dropdowns. 

.. image:: _images/campus_Pg.JPG

.. image:: _images/campus_Config.JPG

**Campus**

The campus name as published by the VOLTTRON
platform.driver service.

**Building**

The building name as published by the VOLTTRON
platform.driver service.

**Time Zone**

Time Zone has default options implemented into the program.

Device Configuration
********************

*Device Configuration* is the second page in the list of configuration pages.
Once this page is selected, there will be a list dropdowns shown in the center. 

.. image:: _images/device_Confg.JPG

There are 4 different selections with device. When the device drop down is selected, these 
4 items will be shown:

.. image:: _images/device_Options.JPG

After a Device is chosen, there is an option below it to choose the model type. 
The two options will be *First Order Zone* and *Simple*. Once an option of these are chosen,
the option will be stored inside of the JSON code.

.. image:: _images/simple_First.JPG

The last value(s) will be determined based upon the device chosen. This list will go over
each of the different options the device configurations will go over. 

**AHU**

When *AHU* is selected, new items will appear. These will be *Equipment Configuration* and *Model Configuration*.

.. image:: _images/ahu_Config.JPG

**Equipment Configuration:**

Configuration of the *AHU* starts with the *Equipment Configuration*.

.. image:: _images/equip_Config.JPG

.. Note:: Each of these check boxes are stored as boolean values. If checked, it will be stored as "True". 
   if unchecked, it will be stored as "false".

**Has an Economizer:**

Input is a checkbox inside *Equipment Configuration*.

.. image:: _images/has_Eco.JPG

**Building Chiller**

Input is a checkbox inside *Equipment Configuration*.

.. image:: _images/build_Chill.JPG

**Variable Volume**

Input is a checkbox inside *Equipment configuration*.

.. image:: _images/variable_Vol.JPG

**Economizer Limit**

Item takes in a floating point precision based value. 

.. image:: _images/econ_Limit.JPG

**Supply Air Set Point**

Item takes in a floating point precision based value.

.. image:: _images/supply_Set.JPG

**Nominal Zone Set Point**

Item takes in a floating point precision based value.

.. image:: _images/nom_Set.JPG

**Model Configuration**

Model Configuration is another option that will be available upon selection of the 
*AHU* Device. Inside of *Model Configuration* there are a selection of inputs to use. 
*cpAir*, *COP*, *mDotAir*, *c0*, *c1*, *c2*, and *c3*. 

**cpAir**

Item takes in a floating point precision based value.

.. image:: _images/cp_Air.JPG

**COP**

Item takes in a floating point precision based value.

.. image:: _images/cop.JPG

**mDotAir**

Item takes in a floating point precision based value.

.. image:: _images/m_Dot.JPG

**c0**

Item takes in a floating point precision based value.

.. image:: _images/c_0.JPG

**c1**

Item takes in a floating point precision based value.

.. image:: _images/c_1.JPG

**c2**

Item takes in a floating point precision based value.

.. image:: _images/c_2.JPG

**c2**

Item takes in a floating point precision based value.

.. image:: _images/c_2.JPG

**c3**

Item takes in a floating point precision based value.

.. image:: _images/c_3.JPG


``End AHU``

**Light**

Light is the second selection of the device list inside of *Device Configuration*. 
*Light* consists of *Model Type* and *Rated Power*.

.. image:: _images/light.JPG


**Model Type** 

Drop down that consists of two items: *Simple* and *Simple Profile**

.. image:: _images/model_Type.JPG

**Rated Power**

Item takes in a floating point precision based value.

.. image:: _images/rated_Power.JPG

**Light Hourly Parameters File Upload**

*Light Hourly Parameters File Upload* will allow a file to be uploaded into.

.. image:: _images/rtu_Hourly.JPG

.. Warning:: Light Hourly Parameters File Upload will only read .json or .csv files. 

Once a file is uploaded, the results will be displayed in the json code on the right side of the 
screen. 

.. image:: _images/hourly_Paramupload.JPG

.. Note:: The example used displays the results of a .json file. 

The items within the file uploaded will be placed in their corresponding areas inside of the json code 
on the right. 



``End Light``

**RTU**

*RTU* is the third selection of the device list inside of *Device Configuration*.
Once *RTU* is selected, there will be a new selection of items to insert info.

.. image:: _images/rtu.JPG

**Temp DB**

Item takes in a floating point precision based value.

.. image:: _images/temp_Db.JPG

**Rated Power**

Item takes in a floating point precision based value.

.. image:: _images/rate_Power.JPG

**On Min**

Item takes in a floating point precision based value.

.. image:: _images/on_Min.JPG

**Off Min**

Item takes in a floating point precision based value.

.. image:: _images/off_Min.JPG

**RTU Hourly Parameters File Upload**

*RTU Hourly Parameters File Upload* will allow a file to be uploaded into.

.. image:: _images/rtu_Hourly.JPG

.. Warning:: RTU Hourly Parameters File Upload will only read .json or .csv files. 

Once a file is uploaded, the results will be displayed in the json code on the right side of the 
screen. 

.. image:: _images/hourly_Paramupload.JPG

.. Note:: The example used displays the results of a .json file. 

The items within the file uploaded will be placed in their corresponding areas inside of the json code 
on the right. 

``End RTU``

**VAV**


*VAV* is the last item on the device list inside of *Device Configuration*.
When *VAV* is selected, there will be a new selection of items to insert info. 

.. image:: _images/vav.JPG

**Model Type**

Drop down that consists of two items: *Simple* and *Simple Profile**

.. image:: _images/model_Type.JPG

**VAV Hourly Parameters File Upload**

*VAV Hourly Parameters File Upload* will allow a file to be uploaded into.

.. image:: _images/rtu_Hourly.JPG

.. Warning:: VAV Hourly Parameters File Upload will only read .json or .csv files. 

Once a file is uploaded, the results will be displayed in the json code on the right side of the 
screen. 

.. image:: _images/hourly_Paramupload.JPG

.. Note:: The example used displays the results of a .json file. 

The items within the file uploaded will be placed in their corresponding areas inside of the json code 
on the right. 


Agent Configuration
*******************

*Agent Configuration* is the third page in the TCC config tool.

.. image:: _images/agent_Ahu.JPG

Within Agent Configuration, the first prompt will be to add an Agent Name.

the second prompt within Agent Configuration will be *device*. This will include
a dropdown list of items: *AHU*, *Light*, *RTU*, and *VAV*.

After selecting an item in devices, there will be different input options
depending on what is selected.

**AHU**

.. image:: _images/ahu_Agent.JPG

When *AHU* is selected in Agent Configuration
there will be 2 new options to input into.


**Supplier Market Name**

Item that takes in a name of a *Supplier Market*

.. image:: _images/supplier_Market.JPG


**Consumer Market Name**

Item that takes in a name of a *Consumer Market*.

.. image:: _images/consumer_Market.JPG

``End of AHU agent``

**Light**

.. image:: _images/light_Agent.JPG

Light will be the second item in the dropdown. 

**Enable Actuation On Start**.

Input is a checkbox inside *Light*

.. image:: _images/enable_Actuation.JPG

**Control Interval**

Item takes in a floating point precision based value.

.. image:: _images/control_Interval.JPG

**Market Name**

Item that takes in a name of a *Market*

.. image:: _images/marketname_Agent2.JPG

**RTU**


.. image:: _images/rtu_Agent.JPG

RTU is the third item in the dropdown selection list. This item, once selected, will place
2 checkboxes below the list. The two checkboxes are *Enable Actuation On Start* and *TNS*. 

**Enable Actuation On**

Input is a checkbox inside *RTU*
.. image:: _images/enable_Actuationrtu.JPG

**TNS**

Input is a checkbox inside *RTU*

.. image:: _images/tns.JPG


**Control Interval**

This item takes in a floating point precision value.

.. image:: _images/control_Interval2.JPG


**VAV** 

.. image:: _images/vav_Agent.JPG

*VAV* is the last item on the list in *Devices* for the Agent Configuration page. 

**Enable Actuation On Start**

Input is a checkbox inside *VAV*
.. image:: _images/enable_Actuationrtu.JPG


**Control Interval**

This item takes in a floating point precision value.

.. image:: _images/control_Interval2.JPG


**Market Name**

Item that takes in a name of a *Market*

.. image:: _images/marketname_Agent2.JPG


**Actuation Method** 

Drop down that consists of two items: *Periodic* and *Market Clear*

.. image:: _images/dropdown_Vav.JPG

Inputs
******

*Inputs* is the fourth page in the TCC application. Inside of the *Inputs* page the first thing
is that, automatically, the first input there is is named *Input 0*. There is also the option to remove
or reset this input as well.

.. image:: _images/inputs.JPG


**Add Input**

The *Add Input* button is an item that allows the user to add another 
*Input* to the page. Each Input is named by default. The first Input will automatically
be named *Input 0*. The next: *Input 1*.. etc.

.. image:: _images/inputs_Pageadd.JPG

**Remove**
In the top right of the *Inputs* page, there is a red button called *remove*. This 
will remove the selected input that you want to remove.

.. image:: _images/remove.JPG

**Topic**

The first tab you will see in the *Inputs* page is *Topic*.

.. image:: _images/inputs_Page.JPG

inside of *Topic* there is a dropdown list. The dropdown list will be determined based upon the 
*Main Configuration File*. Once an option is chosen, different *Points* in the Points tab will be available based upon the 
Topic chosen.

**Point**

Points change based on the topic that is selected.
The points that will be displayed are the ones that are stored
within that device's data structure that is passed in the
platform.driver.store file.

In the first example the topic will be: *VAV213C_SETTINGS*

.. image:: _images/points_1.JPG

The second example the topic will be: *METERS*

.. image:: _images/points_2.JPG

**Initial Value**

This tab will take in a floating point precision number as a value.

.. image:: _images/initial_Value.JPG

**Type**

Type has a drop down of *AHU*, *Light*, and *VAV*.

.. image:: _images/type_Inputspage.JPG

.. image:: _images/type_Drop.JPG

**Mapped**

Once *Type* is selected, mapped will be an available drop down. 

.. image:: _images/mapped.JPG

.. image:: _images/mapped_Drop.JPG

Outputs
*******

The *Outputs* page is the fifth page in the TCC application. Inside of the *Outputs* page the first thing
is that, automatically, the first item there is is named *Output 0*. There is also the option to remove
or reset this input as well.

In the top right of the *Outputs* page, there is a red button called *remove*. This 
will remove the selected input that you want to remove.

.. image:: _images/remove.JPG

**Topic**

inside of *Topic* there is a dropdown list. The dropdown list will be determined based upon the 
*Main Configuration File*. Once an option is chosen, different *Points* in the Points tab will be available based upon the 
Topic chosen.

**Point**

Points change based on the topic that is selected.
The points that will be displayed are the ones that are stored
within that device's data structure that is passed in the
platform.driver.store file.

Example: Topic is set to *VAV120A_SETTINGS*

.. image:: _images/point_Output1.JPG

Example: Topic is set to *METERS*

.. image:: _images/point_Output2.JPG

**Type**

.. image:: _images/type_Outputs.JPG

Depending on the chosen type (*AHU*, *Light*, and *VAV*), the *Mapped* dropdown
will defer.

**Output Configuration**

Below the Type option there are various different tabs to configure.

.. image:: _images/output_Options.JPG

Each tab takes in a floating point precision value.

**Actuator**

Actuator is displayed below the Output configuration tabs. This field is disabled by default.

.. image:: _images/actuator.JPG

Below the Actuator, there is a dropdown to chose from. The dropdown will 
give a list between *default* and *None*.

Schedule
********

Schedule is the last page of the TCC application.

.. image:: _images/schedule.JPG

This page has every day of the week listed (mon-sun).
on each tab there is a *Start* time, an *Always on* button, an *Always off*
button, and an *End* time.

.. image:: _images/schedule_Ex.JPG

**Clock**

When the *Start* and *End* tabs are selected, a pop up of a clock will appear
to select the correct time needed.

.. image:: _images/clock_Schedule.JPG

**Always Off/On**

The buttons for always off and always on determine which days of the week
will be *Always On* or *Always Off*.

.. Note:: When an icon is selected, and another is selected, the previous icon
   will return back to its previous state. They can both be off, but both cannot be on.

.. image:: _images/always_On.JPG

.. image:: _images/always_Off.JPG

Settings
********

**Dark Mode** : There is an option for this document to be used in Dark mode. Click the *Contrast* icon on the top right corner of the page to toggle this option. 

.. image:: _images/dark_Mode.JPG


