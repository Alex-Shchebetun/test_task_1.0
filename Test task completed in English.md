# test_task_1.0
Testing the registration form
Test report
Completed by : Junior Manual QA Sergey Kuznets
1. Conduct full manual testing of the registration form (test link https://serpstat.com/uk/signup/ )
2. Test this form in browsers (DESKTOP) Acer Nitro 5 OS Windows 10 / LCD 15.6 FHD IPS 144 hz Led Lcd :
* Use DevTools browser
*Chrome version 89
* Opera version 75
*Firefox version 87
Use for testing Iphone 6s IOS 13.5.1 Mobile browsers:
*Chrome version 87
*Safari
3.Perform positive tests with valid data
  Test data:
a) E-mail: testopesto7@gmail.com (required field)
         b) Password : Qweasd123! - When creating a password, take into account hints for this field. (required field )
         c) Phone ( is an optional field )
4. Start testing:
   Time : 12-00
   Date : 05.04.2021
5. Below are the checks that were performed for the registration form fields:
5.0 Positive case :
Fill in the fields with valid data


 a) E-mail: testopesto7@gmail.com (required field)
 b) Password : Qweasd123! - When creating a password, take into account hints for this field. (required field )
c) Check the box “I accept the terms of the Public Offer and the Privacy Policy.”
 d) Click the "Create an account" button
Expected result: An account is created and a confirmation email is sent to the user




* Register with Google account (existing account)
Expected Result: Success
* Register using facebook account (existing account
Expected Result: Success


Negative case for checks on required fields
1.Go to the test page
2. Do not fill in the fields, click the “Create an account” button
Expected Result : User will be notified about missing required fields


   The "e-mail" field is a list of positive and negative checks.
5.1. Empty email field.
Expected Result : Message about empty email field


5.2. Email in lowercase
Expected result: carried out successfully


5.3. Email in uppercase
Expected result: carried out successfully


5.4. Email with numbers in account name
Expected result: carried out successfully


5.5. Email with numbers in the domain part
Expected result: carried out successfully


5.6. Email with a dash in the account name
Expected result: carried out successfully


5.7. Email with a dash in the domain part
Expected result: carried out successfully




5.8. Email with an underscore in the account name
Expected result: carried out successfully


5.9. Email with an underscore in the domain part
Expected result: carried out successfully


5.10. Email with dots in account name
 Expected result: The operation is successful


5.11. Email with multiple dots in the domain part
Operation is successful


5.12. Email without dots in the domain part
Expected Result : A message should appear about an incorrect or incorrect e-mail entered in the field


5.13. Email length exceeded (>320 characters)
Expected Result : A message should appear about an incorrect or incorrect e-mail entered in the field


5.14. Missing @ in email
Expected Result: You should see a message about an incorrect or incorrect e-mail entered in the field


5.15. Email with spaces in account name
Expected Result : A message should appear about an incorrect or incorrect e-mail entered in the field


5.16. Email with spaces in the domain part
Expected Result: You should see a message about an incorrect or incorrect e-mail entered in the field


5.17. Email without account name
Expected Result : A message should appear about an incorrect or incorrect e-mail entered in the field


5.18. Email without domain part
Expected Result : A message should appear about an incorrect or incorrect e-mail entered in the field


   




5.19. Email with account name in Cyrillic
Expected Result : A message should appear about an incorrect or incorrect e-mail entered in the field


6. Having defined the requirements for the password field, make a list of checks:


6.1 Generate a strong password using the suggested generator\Enter Valid Email \Check the box “I accept the terms of the Public Offer and Privacy Policy.”\ Click Create an account.
Expected Result: Success

6.2. Enter a valid password ( Qweasd123! \ Enter Valid Email \ Check the box “I accept the terms of the Public Offer and Privacy Policy.”\ Click Create an account.
Expected Result: Success


6.3 Define limit values ​​for the characters of the password field (minimum value 8 characters, maximum value 64)


6.4 Check min value of 8 characters case sensitive\ Valid Had \ Check the box “I accept the terms of the Public Offer and Privacy Policy.”\Create an account
Expected Result: Success


6.5. Check the field for acceptance of 7 characters\ Valid Had \Check the box “I accept the terms of the Public Offer and Privacy Policy.”\ Create an account
Expected result: Rejected, the user will be prompted that this field can accept ("Password must be 8-64 characters long, which contain uppercase and lowercase letters, as well as a number.")


6.6 Leave the field empty\ Valid Had\ Check the box “I accept the terms of the Public Offer and Privacy Policy.”\ Create an account
This field cannot be empty.
6.7 Enter 64 characters \ Valid Had\ Check the box “I accept the terms of the Public Offer and Privacy Policy.”\ Create an account
Expected Result: Success


6.8Enter 65 characters \ Valid Had \ Check the box “I accept the terms of the Public Offer and Privacy Policy.”\Create an account
Expected result: Rejected, the user will be prompted that this field can accept ("Password must be 8-64 characters long, which contain uppercase and lowercase letters, as well as a number.")
 
6.9 Enter 24 characters\ Valid Had \Check the box “I accept the terms of the Public Offer and Privacy Policy.”\Create an account
Expected Result: Success


7.0 Enter 8 characters without a capital letter \ Valid Had \\Check the box “I accept the terms of the Public Offer and the Privacy Policy.” Create an account
Expected result: Rejected, the user will be prompted that this field can accept ("Password must be 8-64 characters long, which contain uppercase and lowercase letters, as well as a number.")


7.1 Check if the Password field accepts <HTML> tags
 enter <script>ALERT123 </script> ;
Expected Result: Rejected, the user will be prompted what the field can accept ("Password must be 8-64 characters long, containing both uppercase and lowercase letters and a number.").


8. Checks for the “Phone number” field (this field is optional)
8.1 Enter a valid phone number for Poland
  +4 8 574-496-389
 For Ukraine +38066-598-4-311
Expected Result: Success


9.Enter the word “Phone number” in the field
Expected Result : Failed (This field must not accept literal values.)


10.Enter <HTML> tags
 enter <script>ALERT123</script>
Expected Result : Failed (This field must not accept literal values ​​or special characters.)


11. Enter special characters +#$#@!#$$$
Expected Result : Failed (This field must not accept literal values ​​or special characters.)


12.Check display of country flags
Expected result : Display all flags
13. Check the search by country for the field “PHONE NUMBER” “Full name of the country” (in the search field, enter the name of the country, in letters):
13.1 In the search field, enter the full code for the country
Expected result : The country is displayed according to the criteria of the search query

13.2 In the search field, enter partially the name of the country
13.3 In the search field, enter partially the code for the strange
Expected Result: Shows countries with values ​​that are similar to the search query.


SUGGESTIONS
for the page (https://serpstat.com/signup/)
1.For the field “Phone number” - make it possible to switch between countries (keyboard arrows) ease of use.
2.For the field “PASSWORD” - the language of the page is “English” - there is no pop-up hint about the number of maximum characters for the field (see example below)
Password (LANGUAGE LAYOUT RUSSIAN)
The password must be 8-64 characters long and contain both upper and lower case letters and a number.
Password (LANGUAGE LAYOUT UKRAINIAN)
The password must be composed of 8-64 characters to cover large letters, small letters and numbers.
Password
Passwords must contain at least 8 characters, one uppercase, one lowercase and one number digit.
3. reCAPTCHA - if the language is “ENGLISH”, then, logically, the captcha should also be translated into the language that is selected as the main language for displaying information.
4. Add the button “Already have an account (LOG IN)” - for the convenience of using this page.
5. The block “These companies trust us” would be nice to align with the information block for greater aesthetics. (See screenshot below)
   




Bug report ID -01
Compiled by: Kuznets Sergey
Assigned to: Developer (full name)
Status : Open


Environment and system settings : Windows 10 Home ( x64 ) . 15.6″, 1920x1080, matte, IPS.
Browsers:Chrome Version 89(64bit) ; Mozilla Firefox Version 87 , Opera 75
Mobile browsers: Chrome version 87.Safari
”Severity : Medium
Priority : Medium
Link :https://serpstat.com/signup/
Name: Sighup > EN > After clicking on the “Create Account” button, nothing happens.


Play steps :
1. Open test link https://serpstat.com/signup/
2. Fill in the field E-mail ytsuytsuyts@gmail.com
3. Enter the password “Qweasd!23”
4. Agree to the privacy policy
5. Click the “Create Account” button
6. Observe


Expected Result: The user should be prompted that the email they entered is not valid.


Actual Result : After clicking on the “Create Account” button, the animation loads and nothing happens. The user does not receive an error message. (Probably the error handler is not connected correctly)


  

Video proof will be available here: https://drive.google.com/file/d/15oZkOIGpijos8B6HAxTCGfUbndppCW4t/view?usp=sharing








Bug report ID -02
Compiled by: Kuznets Sergey
Assigned to: Developer (full name)
Status : Open
Device : Iphone 6s IOS 13.5.1
Mobile browsers: Chrome version 87.Safari
Severity : Medium
Priority : Medium
 Link :https://serpstat.com/signup
Name : signup > In portrait orientation, the user cannot agree to the “Privacy Policy”
 
Play steps :
1.Open test link on mobile browser(Chrome, Safari)
2.Click on the E-mail field
3.Scroll to the “Create Account” button
4. Check the box next to “I accept the terms of the Public Offer and Privacy Policy”
4.Watch
Expected result: A mandatory function is available to the user in portrait mode to confirm his consent to the terms of the public offer and the Privacy Policy.


Actual result: In portrait orientation, the user cannot agree to the “Privacy Policy” does not rotate to this position (he can only do this in the horizontal projection of the device)


The behavior of the site can be traced on browsers: Chrome, Safari.


The video will be available at the following link:


https://drive.google.com/file/d/1--mUFaqW4YeMlG4tSVAI6mnkzwte9ZJQ/view?usp=sharing

Bug report ID -03
Compiled by: Kuznets Sergey
Assigned to: Developer (full name)
Status : Open
Device : Iphone 6s IOS 13.5.1
Mobile browsers: Chrome version 87.Safari
Severity : Low
Priority : Low
 Link :https://serpstat.com/signup
Name: signup >After changing the language in landscape orientation, after returning to portrait, the layout floats.
1.Open test link on mobile browser(Chrome, Safari)
2.Put your device in landscape orientation
3.Click in the upper right corner on the language change icon
4. In the drop-down list, select “RU”
5. After changing the language, return the device to portrait orientation
6.Scroll to the “Create Account” button
7.Watch


Expected Result : All elements on the page will be visible to the user without any overlap.
Actual result: After changing the language in landscape orientation on returning to portrait, the layout floats.
This behavior is observed in the Chrome browser
Link to error video:


https://drive.google.com/file/d/1TybovH3AU2nNr_AeR3C4H01GTeyTPuRW/view?usp=sharing


(See screenshot below)
  

Bug report ID -04
Compiled by: Kuznets Sergey
Assigned to: Developer (full name)
Status : Open
Environment and system settings : Windows 10 Home ( x64 ) . 15.6″, 1920x1080, matte, IPS.
Browsers:Chrome Version 89(64bit) ; Mozilla Firefox Version 87 , Opera 75
Severity : Low
Priority : Low
 Link :https://serpstat.com/uk/signup/
Title : Signup > UK > Chat does not translate into Ukrainian


1. Open a test link
2. Click on the language dropdown in the top right corner
3. Choose Ukrainian language
4. Scroll to the “CHAT” button
5. Click on it
6. Observe


Expected result : Chat content should be translated into Ukrainian .


Actual result: After changing the language to Ukrainian, the chat content is translated into Russian. (See screenshot below)
