# SurveyCTO-Templates

The SurveyCTO Template library hosts templates for both operational aspects inside SurveyCTO (like randomizing modules or how to measure module duration) and for common modules used for research. 


**TIP:** *You can search for template keywords inside brackets [ ] to find a desired template more easily.For example: you could search [calculate], [date] or [repeat groups]* 

Email [researchsupport@poverty-action.org](mailto:poverty-action.org) with any questions, comments, issues, or additions.

## 1. Multiple Attempts Template

In order to facilitate Computer-Assisted Telephone Interviewing (CATI) during the COVID-19 pandemic, SurveyCTO created the [CATI Starter kit](https://support.surveycto.com/hc/en-us/articles/360044958494-Computer-Assisted-Telephone-Interviewing-CATI-starter-kit), a collection of resources and templates for creating a phone survey in SurveyCTO. Different projects at IPA have created templates based on the CATI Starter kit that address common issues encountered when conducting phone surveys.

The [Multiple Attempts Template](https://github.com/PovertyAction/SurveyCTO-Templates/tree/master/Multiple%20Attempts%20Template) allows enumerators to submit one form per day for each case instead of submitting one form for each attempt. For projects that are trying to limit their number of submissions and save money, this form will drastically lower the number of submissions while saving all information of attempts for each case. 

[CATI] [multiple] [attempt] [phone survey] [phone surveys] [operational]

## 2. Mobilizer Survey Template

The [Mobilizer Survey Template](https://github.com/PovertyAction/SurveyCTO-Templates/tree/master/Mobilizer%20Survey%20Template) includes two xlsforms: the __Mobilizer Form__ and the __Phone Survey Form__. This template is useful when you do not have previous information about your survey sample. The mobilizer form is used by the mobilizer, who calls respondents to check respondents' availability for the phone survey as well as the language in which the respondent would prefer to be surveyed. Cases are then assigned to the phone survey form by matching them to enumerators who speak the same language.

[sample] [mobilizer] [phone survey] [phone surveys] [phone] [matching] [enumerator] [language] [operational] [CATI]

## 3. Advanced Case Management Template

The [Advanced Case management Template](https://github.com/PovertyAction/SurveyCTO-Templates/tree/master/Advanced%20Case%20Management%20Template) is a pre-made complex workflow for phone surveys with multiple respondent contacts and secondary contact. It is designed to make, in only one submission, up to 7 calls to different numbers for the person you are searching for, and call up to 6 third-party contacts that can help you locate the participant, each contact containing up to 3 different phone numbers. This means that in total an enumerator can try to call up to 25 different phone numbers. However, the template can also work if you only have one phone number for the participant and have no contacts.

[CATI] [operational] [cases] [case management] [multiple] [contacts] [phone] [phone survey] [phone surveys]

## 4. Ordinal calculation

Use the [Ordinal calculation Template](https://github.com/PovertyAction/SurveyCTO-Templates/tree/master/Ordinal_calculation) when you have a repeat group and you need a calculate inside the repeat group that calculates the current index in an ordinal way up to the 30th position. With this you could have labels like “What is the name of the third member” instead of the usual “what is the name of the member # 3”.

[repeat groups] [calculate] [ordinal] [roster] [operational]

## 5. Random Module Order

Use the [Random Module Order Template](https://github.com/PovertyAction/SurveyCTO-Templates/tree/master/Random%20Module%20Order) when you want to have random module order (inside every module the order of the questions remains, but the order of the modules as a whole is random). This example can be used for 2 modules (AB or BA) or 3 modules(ABC, ACB, BAC,BCA,CAB,CBA). Given that this type of randomization grows factorially, having more than 3 modules in a random way is already very heavy for SurveyCTO and thus not recommended.

[random] [randomization] [order] [operational]

## 6. Birthday Age calculation

The [Birthday Age calculation Template](https://github.com/PovertyAction/SurveyCTO-Templates/tree/master/birthday_age_calculation) allows you to enter a birthdate in formats “mm/dd/yyyy”, "dd/mm/yyyy" or calendar; or to respond with an estimated age and then calculate the age based on whether a date or an estimation was provided.
This template has great contribution from Emma Davies while in IPA Philippines

[calculate] [age] [birthday] [estimation] [operational]

## 7. Date that allows "doesn't know"

Use the ["Date that allows dk" Template](https://github.com/PovertyAction/SurveyCTO-Templates/tree/master/date_allows_dk) when you need to ask about a date but allowing the response “Doesn’t know/Refuse to answer”. The template has 3 ways of doing that: 1)Have a datetime field and a select_one for the “Doesn’t know/Refuse to answer” inside a field-list group. 2)Enter the day, month and year with integers, each allowing for -999 (Don’t know) and -888(Refuse to answer), and 3) Select the day, month and year from select_one that includes the “Doesn’t know/Refuse to answer” options.

[dates] [datetime] [don’t know] [refuse to answer] [field-list] [operational]

## 8. Enumerator instructions

Use the [Enumerator instructions Template](https://github.com/PovertyAction/SurveyCTO-Templates/tree/master/enumerator_instructions) to provide initial instructions to enumerators regarding which messages are for them (in blue or red). This is a basic template that aims to provide an idea of how instructions can be given to enuemerators regarding showing figures, reading or not the choice lists, or questions to the enumerator instead of the respondent.

[enumerators] [enumerator] [color] [instructions] [operational]

## 9. Likert template
Use the [Likert Template](https://github.com/PovertyAction/SurveyCTO-Templates/tree/master/likert_template) to visualize how different likert questions can look like, including when you need to ask a question using a Likert scale that includes “Doesn’t know/Refuse to answer” but you do not want to have those options inside the same likert scale. Of course you can combine different aspects of these display options.

[likert scale] [likert] [field-list] [[don’t know] [refuse to answer] [operational]
## 10. Module durations
Use the [Module durations template](https://github.com/PovertyAction/SurveyCTO-Templates/tree/master/module_durations) to calculate module duration in seconds and also in minutes. This template includes 4 sample modules.

[duration] [calculate] [module] [time] [operational]

## 11. Repeat that allows selection

Use the [Repeat that allows selection Template](https://github.com/PovertyAction/SurveyCTO-Templates/tree/master/repeat_allows_selection) when you have a roster (or repeat group), and then you have another repeat group in which you decide the order in which you will respond about the items in the first repeat group. For example: You could first list all the household members (Carlos, Luisa and Jake) and then decide the member order based on their disponibility, not necessarily the same order you used in the beginning.

[repeat group] [roster] [select_one] [selection] [order] [calculate] [operational]

## 12. PHQ-A and GADD-7

Use this module to ask the Phq-9 questions and the Gad7 questions.

[module] [phq_a] [gadd_7] [phqa] [gadd7]
