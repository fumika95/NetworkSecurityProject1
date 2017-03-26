# NetworkSecurityProject1
The objective of this project is to give myself hands-on experience implementing attacks against vulnerable Web applications


#Attack 1: Cross-site request forgery

A malicious HTML page that overwrites the victim’s current announcement with malicious announcement when user is logged in beofre, and visit the page while loggin in.

#Bonus
Instead of redirecting the victim as described in the previous paragraph, make the attack
invisible to the victim. In this case, the victim should see only the URL and content of
your malicious HTML page. 




#Attack 2: Cookie theft 
A user whose email address is victim@naive.com has logged into the DNCMail website. A URL that looks like this (with EVILMAGIC replaced by your exploit):
http://dncmail.org/account.php?email=EVILMAGIC
When the logged in victim visits this URL, the victim’s DNCMail cookie should get sent by
email to attacker.
The user should notice no difference in the behavior or appearance of the web page
compared to simply typing victim@naive.com into the text box on http://dncmail.
org/account.php and hitting Enter. 





#Attack3: Password theft
A malicious HTML page that should work as follows. Assume your victim is not logged
in. Upon visiting your page, the victim should be redirected to http://dncmail.org/. When the 
victim enters a username and password and hits “Log in”, an email should be sent to user
containing the username and password entered by the victim.




#Attack 4:  SQL injection
A HTML page that the tester will open in his browser. The tester will not be logged
in. The HTML page should have a form with a single text field and a submit button (note: the
form should not ask the tester for a password). The tester will type a username into the text
field and submit the form. You can assume the username submitted by the tester is already
associated with a registered account.
As a result, the tester should be logged in as the user whose username he submitted. The
browser’s location bar should be http://dncmail.org/account.php, and the page should
function exactly as if the correct username and password were entered on the real site.

