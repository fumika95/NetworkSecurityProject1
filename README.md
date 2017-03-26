# NetworkSecurityProject1
The objective of this project is to give myself hands-on experience implementing attacks against vulnerable Web applications


##Attack 1: Cross-site request forgery

Hapless Victim (victim@naive.com) has made an important political announcement on
dncmail.org. Your goal is to replace Hapless’ announcement with your own malicious
announcement, so that you can sabotage his/her opportunity to win the primaries.
Create a malicious HTML page that should work as follows. Suppose the victim has logged
into the Announcement Server, and, while still logged in, visits your HTML page. Your page
should overwrite the victim’s current announcement with this malicious announcement,
designed to sow discord throughout the party:
OtherCandidate is a tooootaallll loooooosssseeerrr

###Bonus
Instead of redirecting the victim as described in the previous paragraph, make the attack
invisible to the victim. In this case, the victim should see only the URL and content of
your malicious HTML page. For example, the victim is browsing his favorite forum and sees
your link promising a cute picture of a kitten. He clicks your link, sees the kitten, nods
appreciatively, then closes the tab, unaware that his data at dncmail.org has been modified.

##Attack 2: Cookie theft 
A user whose email address is victim@naive.com has logged into the DNCMail website. Create
a URL that looks like this (with EVILMAGIC replaced by your exploit):
http://dncmail.org/account.php?email=EVILMAGIC
When the logged in victim visits this URL, the victim’s DNCMail cookie should get sent by
email to user.
The user should notice no difference in the behavior or appearance of the web page
compared to simply typing victim@naive.com into the text box on http://dncmail.
org/account.php and hitting Enter. The source of the page can be arbitrarily different, but it
should look and feel exactly the same.

##Attack3: Password theft
Create a malicious HTML page that should work as follows. Assume your victim is not logged
in. Upon visiting your page, the victim should be redirected to http://dncmail.org/. When the 
6
victim enters a username and password and hits “Log in”, an email should be sent to user
containing the username and password entered by the victim.
Important: This is not a phishing attack. Assuming a valid username/password pair was
entered, the victim should be logged into DNCMail.

##Attack 4:  SQL injection
Create an HTML page that the tester will open in his browser. The tester will not be logged
in. The HTML page should have a form with a single text field and a submit button (note: the
form should not ask the tester for a password). The tester will type a username into the text
field and submit the form. You can assume the username submitted by the tester is already
associated with a registered account.
As a result, the tester should be logged in as the user whose username he submitted. The
browser’s location bar should be http://dncmail.org/account.php, and the page should
function exactly as if the correct username and password were entered on the real site.
