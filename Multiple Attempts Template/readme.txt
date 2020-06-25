0. Purpose:
Instead of submitting forms for each attempt, submitting one form per day and storing attempts per day inside the 
form. 


1. Attempt variables in data:

attemptthis*: 	Repeated for each phone number. Records number of times called in corresponding phone number.
attemptany: 	Records number of times at least one phone number tried while using this form (i.e., a single day)
		For example, one sample has 2 phone numbers, phone1 was tried twice and phone2 was tried once. 
		This variable will record 2.
totalattempt: 	Records total number times any phone number tried while using this form (i.e., a single day)
		For example, one sample has 2 phone numbers, phone1 was tried twice and phone2 was tried once. 
		This variable will record 3.



2. Variables to be deleted from data:

The form generates series of calculate varibales which are safe to drop from the survey dataset.
Stata code: 	drop plugin_metadata plugin_len broken_index_* character_*


3. cases.xml file variables:
The cases.xml file has one additional variable in <fieldNames> section - attemptany 
and one additional field mapped in <fieldMap> section - "attemptany":"lastdayattempt".
<showColumnsWhenTable> has one additional field - lastdayattempt


4. How to use
Enumerator will open a new form for a particular case each day and will submit only if the respondent was found.
Otherwise, she will save the form. She will open the saved form whenever she wants to make another attempt. 
Each time she makes attempts using the saved form, the form will store number of attempts. 

Attempt is defined as trying at least one phone number. Therefore, the maximum number of trying one number
is defined as number of attempts. Therefore, if a sample has 2 phone numbers, and the enumerator tried calling 
the first phone number, but found switched off, number of attempts is 1. If she tries the second phone number now, 
the number of attempts is still 1. Now, the enumerator can save the form, and later on the same day can open the 
saved form and navigate to the second phone number because the first phone number is a wrong number. Now if she
makes a phone call on the second phone number, total number of attempts will be 2. This value is recorded in
attemptany variable.

The attemptany variable can be used as part of instancename, so that the enumerator can see how many times the case
was attempted on the saved form (i.e., today). The enumerator can make necessary attempts, if she did not make
enough attempts as per protocol.

The cases table in the tablets also has a column titled "lastdayattempt" which shows number of attempts made for
that case in the last form. This can give an idea to the enumerator if she did not make enough attempts the last day.

 
4. Possible advanced usage
This variable can be inserted as condition to not to close the case if the number of attempt days is made, but required
number of attempts per day is not made. 