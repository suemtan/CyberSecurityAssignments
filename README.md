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

Vulnerability #2: Session Fixation (Session from Green Target to Session to Blue Target)

## Green

Vulnerability #1: Username Enumeration at Login Page(Bold/Unbold)Message(Codepath_UsernameEnumeration.gif)

Vulnerability #2: XSS Exploit using Javascript in Feedback Section when another user accesses it.

## Red

Vulnerability #1: CSRF Vulnerability (update user information in the database via edit page (inspect) without a valid CSRF token)

Vulnerability #2: IDOR Vulnerability where a user can see any accounts including Testy McTesterson (NOT PUBLIC UNTIL SEPT. 1)
And Lazy Lazyman(FIRED FOR STEALING). An attacker just simply guess IDs via URL in Blue, Green,and Red Targets.
