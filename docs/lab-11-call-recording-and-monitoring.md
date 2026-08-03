# Lab 11: Call recording and monitoring

In this lab, you will learn how to schedule call recording and monitoring.

### Only a percentage of calls in each queue will need to be recorded. Tenant level recording needs to be disabled to allow this at the queue level.

Contact Center > Tenant Settings > Voice

* Disable record all calls

Contact Center > Customer Experience > Queues > Investment Q

* Advanced settings
  + Allow recording: Enable
  + Record all calls: Enable

### The supervisor needs to create a recording schedule to implement the percentage.

In an incognito/private window login as Anita Perez in [Control Hub](http://admin.webex.com/)

* Password is the same as Charles Holland

Contact Center > Customer Experience > Call Recording Schedules > Create a call recording schedule

* Name: Investment Q Recording
* Support Queue: Investment Q
* Date Range: Next week
* Time Range: 9am – 12pm
* Days of the week: Mon – Fri
* Percentage: 50%

### Testing monitoring: Supervisor

* Open new tab in same browser
* Go to: <https://desktop.wxcc-us1.cisco.com/>
* Login as Anita Perez
* Password is the same as Charles Holland
* Use Desktop for Audio / Calls

### Testing monitoring: Agent

* Open new browser (not a new tab but a different browser)
* Go to: <https://desktop.wxcc-us1.cisco.com/>
* Login as Eric Steele or Kellie Melby
  + Password is the same as Charles Holland
  + Start with the Corporate Team
  + Handle calls using Desktop
  + Change state to available
* Call your main number (selected in Lab 10), select 2 for the Investements Queue
* Answer as the agent
* Go to browser where you are logged in as Anita to monitor the call.

| Help articles | | |
| --- | --- | --- |
| [Manage call recording schedules](https://help.webex.com/en-us/article/ejatso/Manage-call-recording-schedules) | [Monitor agents on a call](https://help.webex.com/en-us/article/nda5iqeb/Monitor-agents-on-a-call) | [Manage Interaction History](https://help.webex.com/en-us/article/97823o/Manage-Interaction-History) |

STOP: End of Lab 11

Raise your hand and leave it raised in the Webex Meeting. Wait for further instruction.  
![](assets/docx-image-021.png)
