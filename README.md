# Project 8 - Pentesting Live Targets

Time spent: **15** hours spent in total -Eun Suk Lee-

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

Vulnerability #1: SQL Injection : "'OR SLEEP(5)=0--'" by inserting this SQL statement after id, it will make an SQL query.
				: Other red and green pages indirect.
				: https://github.com/yeunsek9/yeunsek9_project8/raw/master/Blue1.gif
				
Vulnerability #2: Session Hijacking/Fixation					
				: Using the session that is already login, the attacker can change its session and get admin privileges.
				: https://github.com/yeunsek9/yeunsek9_project8/raw/master/blue2.gif
				


## Green

Vulnerability #1: Username Enumeration		
				: the mistake is that the output of valid username is in bold. The message is not the same between valid and non valid accaounts.
				: https://github.com/yeunsek9/yeunsek9_project8/raw/master/Green1.gif
				

Vulnerability #2: Cross-Site Scripting
				: When the admin see the feedback page, the feedback has a xss vulnerability. the script runs automatically whenever admin opens up the feedback page.
				: https://github.com/yeunsek9/yeunsek9_project8/raw/master/Green2.gif
				



## Red

Vulnerability #1: Insecure Direct Object Reference	
				: The saleperson database can be accessed by modifying the id value. For blue and green, it is not working to see id 10 and 11.
				: https://github.com/yeunsek9/yeunsek9_project8/raw/master/Red1.gif
				

Vulnerability #2: Cross-Site Request Forgery	
				: By clicking on the link, it will post request to make changes to the database.
				: https://github.com/yeunsek9/yeunsek9_project8/raw/master/Red2.gif
				


## Notes

Describe any challenges encountered while doing the work
