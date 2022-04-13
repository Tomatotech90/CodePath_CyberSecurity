
# Project 8 - Pentesting Live Targets

Time spent: 4 hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each color is vulnerable to only 2 of the 6 possible exploits. First discover which color has the specific vulnerability, then write a short description of how to exploit it, and finally demonstrate it using screenshots compiled into a GIF.

## GREEN

Vulnerability #1: User Enumeration

Description: 
A careless developer mistake has created a username enumeration vulnerability. Determine which color has the vulnerability. You can use the existing username "jmonroe99" as a test. Next, figure out what mistake the developer made.

the developer maker a mistake in the css (falure), where a real account exist but the password is wrong wil display bold the messgae, but when the account doesnt exist will be (fail) the message will eb normal.

gif:
[ezgif com-gif-maker (4)](https://user-images.githubusercontent.com/96146875/163218012-b8be641b-ee31-4fc6-bc91-179e04620063.gif)

video:



https://user-images.githubusercontent.com/96146875/163218109-86e566a1-76d5-4acf-b9fe-d6e25e13d7b3.mp4

--------------------------------------------------------------------------------------------------------------------------------------------------------

## RED

Vulnerability #2: Insecure Direct Object Reference

Description:
One of the three sites is missing code which would prevent some sensitive information from being made public. Determine which color has the vulnerability. Then, figure out what the other two sites did correctly to prevent the information leak.

video:


https://user-images.githubusercontent.com/96146875/163219877-bde77202-7e78-4644-a3d2-c22f501a8b44.mp4

gif:


![ezgif com-gif-maker (3)](https://user-images.githubusercontent.com/96146875/163219954-cc0ea5c7-0e9d-4970-baaf-39491526610b.gif)



--------------------------------------------------------------------------------------------------------------------------------------------------------
## Blue

Vulnerability #3: SQL Injecton

Description:
Most of the data input received by these websites is being sanitized properly. However, one of the three sites has one place where the input is not being sanitized before being used in an SQL query. Determine which color has the vulnerability.

video:

https://user-images.githubusercontent.com/96146875/163220449-846d070a-d2d4-41db-9acb-457daeff9ce0.mp4


gif:

![ezgif com-gif-maker (2)](https://user-images.githubusercontent.com/96146875/163220494-38137ea4-dd4d-476c-8cf9-905937529528.gif)



--------------------------------------------------------------------------------------------------------------------------------------------------------

## Green

Vulnerability #4: Cross-Site Scripting

Description:
All three sites do a good job of protecting against a reflected XSS attack. However, one of the sites has a mistake which leaves the site vulnerable to a stored XSS attack. A reflected XSS attack would be easy to reveal, while a stored XSS does not provide instant feedback. You will need to log into the admin area and look through the CMS in order to "spring the trap" and find out if your attack succeeded. Determine which color has the vulnerability. Remember, others will be attacking these sites alongside you. Use your name in the XSS so that your results won't be confused with anyone else's (example: <script>alert('Mallory found the XSS!');</script>).

video:



https://user-images.githubusercontent.com/96146875/163220838-62aeba37-d01e-47f6-910f-f4f4064d7870.mp4



gift:


![ezgif com-gif-maker (1)](https://user-images.githubusercontent.com/96146875/163220866-da1e1408-9675-4e1e-aa91-853adbbf133c.gif)


-------------------------------------------------------------------------------------------------------------------------------------------------------
## Red

Vulnerability #5:Session Hijacking/Fixation

Description:
Two of the three websites expire their active sessions and require users to re-login every 30 minutes. That is probably too aggressive for the real world, but it is better than the third site which allows sessions to be a year old, and never regenerates the session ID, even when the user agent string changes. This makes it vulnerable to both session hijacking and session fixation attacks.

video:



https://user-images.githubusercontent.com/96146875/163221233-2ea482c8-b0b3-4514-8203-711027dd0876.mp4



gif:

![ezgif com-gif-maker](https://user-images.githubusercontent.com/96146875/163221267-d38aac68-abf7-4452-8deb-e512dc6e914f.gif)




