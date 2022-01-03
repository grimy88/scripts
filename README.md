# Python and batch scripts


1) Protractor script:
Protractor script is used to generate a new project for Protractor.
User will be given options to generate configuration for protractor project.
Read release notes for protractor project script.

2) Delete old files:
Batch script to delete files older then given number of days.

3) Helper functions in python:
helper functions to clean folder and to create a directory (folder) if it does not exist on a specific location.

4) Parse XML in python:
This method is used to search for element inside xml file and its value, depending on the type of value we are doing different searches. The searched value type can be an elements attribute value and the nodes value. Also we have a couple more parameters in case we have multiple instances of the same tag in the xml.
We have a couple of cases for which this code is for:

    We search for the tag and that nodes value.
    We search for tag and an attribute inside the tag and check the value of the attribute.
    We search for the tag which has multiple instances with same name so we use one attribute and its value to go through all of the instances to find the one we need, after which we look for the actual attribute we need and check its value.

In the xml example you can find all of the noted cases. For the first two cases you can take any tag you want, for the last case the tag with name "SameTag" or "Function" can be used. 

5) Read CSV file in python:
This is a short script which just reads an .csv file where the user inputs the number of the line or value you want to read from the csv file and afterwards clean (delete) that value from the csv file

6) Change registry on windows using python:
Change the registry value on Windows you can use this short script to automate the process easily. In this script i have used python 2.4. The user just sends the location of the registry, the name of the registry, its value and type. Since python does not have sufficient permissions on Windows to change the registry we are generating the command line (batch) script which will be executed and after that deleted so that no unnecessary files will stay on the system. In this code snippet we generate a random name for the file which we generate so that it will be unique also we have logs in case something goes wrong. The default location is hard coded but you can change that to your liking or delete it and just send the absolute path to your registry.
