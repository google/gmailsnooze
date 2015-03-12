README
------

Gmail Snooze is a Google Apps Script that adds the ability to
"snooze" an email to classic Gmail. To snooze an email means
to have an archived email reappear in the inbox after a set
number of days. This is accomplished using special labels that
the script sets up, and an Apps Script time trigger that moves
emails between the labels around midnight in your local time.

The original Gmail Snooze blog post can be found here:
http://gmailblog.blogspot.com/2011/07/gmail-snooze-with-apps-script.html.
This update works the same way, but is more user friendly
to install and manage, as it no longer relies on a
spreadsheet or changing code to configure it. In fact, the
script has its own installer, and so if one user installs
the code in their own account (using the "code installation"
instructions below), any number of other users can install the
functionality themselves without touching the code, simply
by clicking an install link. This makes it easier to deploy
in large organizations.


TL;DR INSTALLATION
------------------
There is a canonical copy of this script [hosted in the 
Chrome Web Store](https://chrome.google.com/webstore/detail/gmail-snooze/ajhdhpnafihkepjialgccenokkljdlaf).
It can be installed using the piggyback instructions
below; basically, go to that URL and click OK and Install
whenever prompted.


CODE INSTALLATION
-----------------
To install Gmail Snooze from code:

 * Navigate to https://script.google.com
 * Replace the sample code in the text editor with the contents of "Code.gs"
 * Use the File > Save menu and name the script (e.g. "Gmail Snooze")
 * Use the File > New > Html file menu and create a file called "ui"
 * Replace the sample code in the text editor with the contents of "ui.html"
 * Use the Publish > Deploy as Web App menu
 * Click "Save new version" (no need for any text in the box)
 * Change "Execute the app as" to "User accessing the web app"
 * OPTIONAL: If you want to allow piggybacking, change "Who has access to the
   app" to "Anyone". Allowing piggybacking does not give anyone else access to
   your Gmail or scripts.
 * Click Deploy
 * Navigate to the "Current web app URL"
 * Follow the piggyback installation instructions below.


PIGGYBACK INSTALLATION
----------------------
To install Gmail Snooze from an existing code installation:

 * Navigate to the deployed web app URL from a code installation
 * If prompted to authorize or grant permissions, do so
 * Select the options that you prefer
 * Click install


UNINSTALL
---------
You can temporarily uninstall using the Uninstall button at the web app URL.
This will functionally disable Gmail Snooze but preserve all of your options
for reinstalling later. If you would like to fully uninstall Gmail Snooze,
there is a link in the automated email you will receive from Apps Script
at installation time. If you did a code installation you can also delete
the project.


AUTHOR
------
Gmail Snooze was written by Corey Goldfeder at Google.

This is not an official Google product (experimental or otherwise), it is just code that happens to be owned by Google.
