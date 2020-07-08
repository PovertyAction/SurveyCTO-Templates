# README
The Mobilizer Survey Template is designed for a sample where you do not know the respondent's availability or preferred language. There are 2 xlsforms with for 2 different roles: the mobilizer and the enumerator. The mobilizer calls the respondent, creates an appointment time if the respondent answers, and records the respondent's preferred language. This allows the enumerators to only call respondents who have expressed interest, set an appointment, and speak the same language.

## Expected Workflow
All respondents to be reached are added to the cases file and assigned to the user mobilizer and the mobilizer form ID. Mobilizers log in with their username and password.

<img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/mobilizer%20login.jpg" width="200" />

Mobilizers will go to "Manage "Cases" and select a case to call.

<img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/manage%20cases.jpg" width="200" /> <img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/cases%20screen.jpg" width="200" /> <img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/case%20101.jpg" width="200" />

When a respondent is reached, the mobilizer survey allows the enumerator to set a time and the respondent's language.

<img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/appointment%20screen.jpg" width="200" /> <img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/appointment%20english.jpg" width="200" /> 

Once the form is finalized, the case will be assigned to the user that speaks the same language and no longer appear as a case for the mobilizer.

<img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/finalize%20form.jpg" width="200" /> <img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/manage%20cases.jpg" width="200" /> <img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/mobilizer%20cases%20updated.jpg" width="200" /> 

This example case has been assigned to the "english" user because the respondent speaks english. The english user can log in to the Collect app and look at their cases to see their assigned cases.

<img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/english%20login.jpg" width="200" /> 

The english user will only see the case they have been assigned, and will see the set appointment time.

<img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/manage%20cases.jpg" width="200" /> <img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/case%20101%20english.jpg" width="200" /> <img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/callback%20time%20english.jpg" width="200" /> 

The english user can now call the respondent at the assigned time and conduct the survey. If the survey is completed, and the form is finalized and sent to the server, the case will no longer appear in the english user's cases.

<img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/consented.jpg" width="200" /> <img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/finalize%20form.jpg" width="200" /> <img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/manage%20cases.jpg" width="200" /> <img src="https://github.com/PovertyAction/SurveyCTO-Templates/blob/master/Mobilizer%20Survey%20Template/readme%20images/no%20cases%20english.jpg" width="200" /> 


## The Files

### cases.xml

The cases.xml is the cases dataset definition. This file sets up the cases server dataset and connects the variables from the dataset, to the survey, back into the dataste. This allows the cases dataset to update as respondents are reached. Change the form ID to your mobilizer survey's form ID on lines 10 and 20, and to your phone survey's form ID in lines 13 and 28.

Before uploading the cases.csv, be sure to use this dataset definition. On your SurveyCTO server, choose [+] > Add server dataset > New dataset from definition.

### cases.csv

The cases.csv file holds all the respondents that will be attempted. Keep all variable names the same and fill in with your project's respondents and phone numbers. The variables `last_call`, `num_calls`, `next_call` and `callback_time` will be empty when you begin the survey and will be updated as the mobilizer survey and phone survey are conducted.

### Phone Survey Mobilizer Form.xlsx

This is the mobilizer form xlsform. Adjust the languages choice list to the languages that your enumerators can speak. You should also change the form IDs in `pb_formids` if you change the form ID of the mobilizer form or the phone survey form. 

### Phone Survey Form.xlsx

This is the phone survey xlsform. Add your project's consent script in `consent_note` and include all your survey variables within the `app_grp` group. 
