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

Vulnerability #1: SQLInjection(Salesperson ID)in the URL using ' OR SLEEP(5)=0--'
![Codepath_SQLInjection_Blue](https://user-images.githubusercontent.com/42657573/57168811-6193d880-6db8-11e9-9089-aa09339a0b01.gif)
Vulnerability #2: Session Fixation (Session from Green Target to Session to Blue Target)
![Codepath_SessionFixation_Blue](https://user-images.githubusercontent.com/42657573/57168835-7c664d00-6db8-11e9-9840-f950ffa013cc.gif)

## Green

Vulnerability #1: Username Enumeration at Login Page(Bold/Unbold)Message(Codepath_UsernameEnumeration.gif)
![Codepath_UsernameEnumeration_Green](https://user-images.githubusercontent.com/42657573/57168848-90aa4a00-6db8-11e9-9dfc-f21b7c70ac0c.gif)

Vulnerability #2: XSS Exploit using Javascript in Feedback Section when another user accesses it.
![Codepath_XSS_Green](https://user-images.githubusercontent.com/42657573/57168882-afa8dc00-6db8-11e9-988d-8437def399f8.gif)

## Red

Vulnerability #1: CSRF Vulnerability (update user information in the database via edit page (inspect) without a valid CSRF token)
![Codepath_CSRF_Red](https://user-images.githubusercontent.com/42657573/57168914-d535e580-6db8-11e9-9b2d-29addc17523d.gif)

Vulnerability #2: IDOR Vulnerability where a user can see any accounts including Testy McTesterson (NOT PUBLIC UNTIL SEPT. 1)
And Lazy Lazyman(FIRED FOR STEALING). An attacker just simply guess IDs via URL in Blue, Green,and Red Targets.
![Codepath_IDOR_Red](https://user-images.githubusercontent.com/42657573/57168927-ec74d300-6db8-11e9-8206-52699d8eee92.gif)

##Bonus Objective 2

Build on Objective #4 (Cross-Site Scripting). Experiment to see if you can use XSS to: a) direct the user to a new URL
![Codepath_XSS_ExternalLink](https://user-images.githubusercontent.com/42657573/57169028-568d7800-6db9-11e9-877f-ce4046936722.gif)
