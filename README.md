# Test Cases 

This repository contains a collection of sample test cases that I have written during my previous QA projects.

*Note: The email addresses and passwords used in these test cases are fictitious and for testing purposes only.*

---
## Test Case 1
**Title:** 
Valid login with correct credentials

**Description:**
Verify if a user will be able to login with correct credentials.

**Pre-conditions:**
User should have a valid account. 

**Steps to reproduce:**

1. Open https://auth.emag.ro/user/login
2. Enter a valid email address
3. Click the "Continue" button
4. Enter a valid password
5. Click the "Continue" button

**Expected result:**
The user should be successfully logged in and redirected to his profile page.

**Test data:**
Email address: alice01m@gmail.com
Password: 1234


---

## Test Case 2
**Title:**
Invalid login with incorrect credentials

**Description:**
Enter an incorrect email address or password and attempt to log in.

**Steps to reproduce:**

1. Open https://auth.emag.ro/user/login
2. Enter a valid email address
3. Click the "Continue" button
4. Enter an invalid password
5. Click the "Continue" button

**Expected result:**
The system should deny access and display the error message: *"Incorrect email or password"*.

**Test data:**
Email address: alice01m@gmail.com
Password: 1236


---

## Test Case 3
**Title:** 
Error message for empty email field

**Description:**
Check if the login is not working without an email.

**Steps to reproduce:**
1. Open https://auth.emag.ro/user/login
2. Click "login" button
3. Click the "Continue" button

**Expected result:**
The system should display the error message "Required field". 


---

## Test Case 4
**Title:**
Search returns correct and relevant results

**Description:**
Verify that the search function returns relevant and accurate items based on a specific query entered by the user.

**Steps to reproduce:**

1. Open https://www.emag.ro/
2. Type a valid product name in the search bar
3. Press Enter

**Expected result:**
The first results include items with that product name in the title or description.

**Test data:**
product name: "laptop"


---

## Test Case 5
**Title:**
Search with autocomplete suggestions

**Description:**
Verifies that autocomplete suggestions are displayed after the user types at least 3 characters into the search bar on the homepage.

**Steps to reproduce:**

1. Open https://www.emag.ro/
2. Type the first character of a valid product keyword in the search bar — verify no suggestions appear  
3. Type the second character — verify no suggestions appear  
4. Type the third character — verify a list of relevant autocomplete suggestions appears
5. Continue typing additional characters and verify the suggestions list updates dynamically according to the input  

**Expected result:**

No autocomplete suggestions are displayed after typing only 1 or 2 characters.

After typing the third character, a list of relevant autocomplete suggestions should appear.

Suggestions such as "phone", "phone holder", etc., should be visible.

The suggestions list should update dynamically as the user continues to type additional characters.

**Test data:**
Search keyword: "pho" 


