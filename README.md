# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.) 

## Blue

Vulnerability #1: SQL Injection

Vulnerability #2: __________________


## Green

Vulnerability #1: Username enumeration - When using a valid username and incorrect password, the error is bold. If user does not exist, the error is not bold. To reproduce: 1. Sign in using an invalid username > Error will appear "Log in was unsuccessful". 2. Sign in again using a valid user with an incorrect password >  Error will appear "Log in was unsuccessful" in bold. > See attached "Challenge Goal 1 Again.gif" file.

Vulnerability #2: Cross-Site Scripting. 1. Click on Contact tab > Type in a name and email address. 2. In the Feedback box, type <script>alert('Gina S. found the XSS!');</script>) > Click Submit button. 3. Click Login > Log in as pperson > Click Staff Menu tab > Click Feedback button. 4. Message will pop up stating Gina S. found the XSS!  See attached "Challenge Goal 4 Cross-Site Scripting.gif" file


## Red

Vulnerability #1: Insecure Direct Object Reference - When logged out, I can view a Salesperson that is not public yet. To reproduce: 1. Sign in with an admin ID such as pperson > Look at Salesperson Testy McTesterson, who is not public yet. The ID (10) is in the browser. 2. Logout and Click on Find Salesperson > Change ID in browser to 10 for Testy McTesterson > Testy's information is displayed, even though not public yet. See attached "Challenge Goal 2.gif" file.

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work
