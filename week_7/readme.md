
Codepath
--------------
Time spent: 7 hours spent in total
Note: 
have a problem with vagrant in the installation on my devices, so I use another way to recreate wpdistellery, I use a docker container that will be link in this repo.
--------------
1 CSRF

The attacker can host a malicous website that can have a csrf code:
source:https://github.com/Tomatotech90/wk/blob/main/index.html
making the victim admin click on that link and subminting a post without notice.


video:
https://user-images.githubusercontent.com/96146875/162872381-8c1f2718-fdda-487e-9527-e965a0f8e513.mp4

--------------
2 

Directory Traversal and Informaiton Exposure

A directory listing is inappropriately exposed, yielding potentially sensitive information to attackers.
using this paths on the URL can be acces the follow directories.
vulnerablewordpress/wp-admin/js/
vulnerablewordpress/wp-admin/css/
the attacker can acces 

video:
https://user-images.githubusercontent.com/96146875/162872748-5f1fa0c8-16b9-49d0-883d-2fcf705fc147.mp4


--------------
3

Wordpress Work the flow file upload 2.5.2 Shell Upload Vulnerability
Work the Flow File Upload. Embed Html5 User File Uploads and Workflows into pages and posts. 
Multiple file Drag and Drop upload, Image Gallery display, Reordering and Archiving.
This two in one plugin provides shortcodes to embed front end user file upload capability and / or step by step workflo
source:
https://www.exploit-db.com/exploits/36640

video:
https://user-images.githubusercontent.com/96146875/162873727-6f4fbacc-a522-41dd-b9e5-b5a38e7e636d.mp4

--------------
4
Authenticated Shortcode Tags Cross-Site Scripting


source:
CVE-2015-5714
CVE-2015-5715
code:
BLA BLA BLA
HERE !!![caption width="1" caption='<a href="' ">]</a><a href="http://onMouseOver='alert(1)'">Oi Hai</a>
video:
https://user-images.githubusercontent.com/96146875/162874914-11183481-a8ba-49c7-becc-ae1c5673cf86.mp4

--------------
5

Vulnerability Name or ID: Password Brute Force Attack

source:
wpscan --url wpdistillery.vm --enumerate u
wpscan --url wpdistillery.vm --usernames '<user-name>' --passwords /usr/share/wordlists/rockyou.txt
image:
  ![20220411225944_Moment](https://user-images.githubusercontent.com/96146875/162875415-6096055d-5f72-40ce-a3e4-ffcc67019908.jpg)

  
