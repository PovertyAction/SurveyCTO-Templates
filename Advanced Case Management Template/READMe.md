# README
The Advanced Case Management Template is designed to make, in only one submission, up to seven calls to different numbers for the person you are searching for, and call up to 6 third-party contacts that can help you locate the participant, each contact containing up to 3 different phone numbers.

## Files

### Advanced Case Management Template Manual.pdf

A step-by-step guide for the features of the template, how to set it up, and configure your server to use it for your project's needs. 


### Advanced Case Management Template.xlsx

The SurveyCTO xlsform of the template. All fields to adjust for your project's needs are labelled as well as noted in the manual. 

### Cases Variables.xlsx

A list of the varaibles used in the cases workflow and dynamic updating of the form. All variables are already included in the xlsform and configured in the cases dataset definition.

### Survey Flow

A flow chart of the scenarios the survey logic as an enumerator fills out the survey. This shows all possible responses and how the survey will handle it. 

### field mapping - cases definition.xml

The configuration of the cases dataset and how it relates to your survey. This creates the field mapping within SurveyCTO so you do not have to connect the cases and survey manually.

Before uploading the cases.csv, be sure to use this dataset definition. On your SurveyCTO server, choose [+] > Add server dataset > New dataset from definition.

*You may need to adjust the form ID in this file if you change the form ID in the xlsform.* 

### pulldata

This folder contains all files that will be attached to your xlsform as form attachments when you upload the survey. 

#### call-phone-number.fieldplugin
This zip file allows you to use the [SurveyCTO field plug-in](https://github.com/surveycto/phone-call), so enumerators can call respondents directly from the SurveyCTO Collect app. Include this entire file when attaching. 

#### cases.csv
An example file of the cases dataset. Replace the example data with your project's repsondent infromation following the same variable format. Do not delete variables.

#### launch-sms.fieldplugin
This zip file allows you to use the [SurveyCTO field plug-in](https://github.com/surveycto/launch-sms), so enumerators can text respondents directly from the SurveyCTO Collect app. Include this entire file when attaching. 

__If you have any issues or ideas for this template, please create an issue on this repository or email researchsupport@poverty-action.org.__ 
