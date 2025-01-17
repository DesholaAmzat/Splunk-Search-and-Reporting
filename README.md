<h1>Splunk-Search-and-Reporting
 Lab<br/> 

<h2>Description</h2>
In this lab, I was able to  walk through the installation, configuration, and basic usage of Splunk. With the completion of this project, I feel like I am on my way to becoming a SIEM tool expert! Please let me know if you have any questions!


<h2> Languages and Utilities Used</h2>

- Splunk Enterprise
- Search Processing Language
- Oracle VirtualBox


<h2> Environments Used</h2>

- Windows Server 2019

<h2> Program Walk Through</h2>

<img src="https://i.imgur.com/tEDWgAM.png" height="88%" width="80%" />
Navigate to the splunk website in your VM and download splunk enterprise. It can be found  

[here](https://www.splunk.com/en_us/download.html?utm_campaign=google_amer_en_search_brand&utm_source=google&utm_medium=cpc&utm_content=free_trials_downloads&utm_term=splunk%20free&device=c&_bt=662330344243&_bm=p&_bn=g&gad_source=1&gclid=Cj0KCQiA1p28BhCBARIsADP9HrMeXO3BO27U8uvJd3ZGtVBdH94JRZ-JBDfISjaXFzGBvjKKrn-NFRoaAu0dEALw_wcB)    



<img src="https://i.imgur.com/YKzlNLd.png" height="88%" width="80%" /> 
Create a username and password for logging into the web app. Once you have created an account, select a web browser for the app to open in. Once the app is open, log in with the credentials you have created earlier.
<img src="https://i.imgur.com/osYPbxc.png" height="88%" width="80%" /> 
Once you have reached this landing page, we now need to set our logs up to be ingested within the tool. Navigate to the settings tab in the top right corner, then select Data Inputs, and click on the edit button next to local event log collection. In this lab we will only deal with local events, instead of a remote system. 
<img src="https://i.imgur.com/DnktRws.png" height="88%" width="80%" />
In this project, we will only focus on the application, security, and system logs, because those are the basic logs used in most, if not all SIEMS, Once you have selected these three be sure to click on Save.
<img src="https://i.imgur.com/KTJxTmS.png" height="88%" width="80%" />
Navigate to the apps button in the top left corner, and click on the drop down to go to search and reporting. Start a new search by entering the asterisk or star key in the search bar and pressing enter. This is to display all the known events on the local system .
<img src="https://i.imgur.com/K3jpxDq.png" height="88%" width="80%" />
Next open up the Event Viewer in Windows, click on the Windows log drop-down, right click on security, and then select clear logs. We would like to clear the logs so that we can view the event of logs being cleared within Splunk.
<img src="https://i.imgur.com/eJZgufC.png" height="88%" width="80%" />Now to add more parameters to our search, you can hover your mouse over any part of a specific event and then click on the “Add to Search” . For this lab, we will be adding the host, source, and event code parameters to the search. This means we are specifying events only on this computer, from the windows event viewer security logs, With an event code of 1102. Notice the message on the event says the audit log was cleared. Now we have an event that shows an action we did ourselves in Splunk. Be sure to copy the search parameters from the search bar and paste it into a notepad, as we will need this specific query later on.

<img src="https://i.imgur.com/HI9qgSE.png" height="88%" width="80%" />
<img src="https://i.imgur.com/pNCHXuR.png" height="88%" width="80%" />
<img src="https://i.imgur.com/D0ok6OC.png" height="88%" width="80%" />
<img src="https://i.imgur.com/bLp8oJx.png" height="88%" width="80%" />
