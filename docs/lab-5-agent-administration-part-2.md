# Lab 5: Agent administration: Part 2

In this lab, you will learn how to create sites, teams, desktop layouts, address books and Idle/Wrap-up codes.

### Yellow Brick Bank needs an easy way of reporting for single locations.

Contact Center > User Management > Sites

* Name: YBB HQ
* Multimedia Profile: Voice\_Chat\_MPP

### Agents may be part of more than one team and need to choose which team to log into.

Contact Center > User Management > Teams

* Name: Investment Team
  + Site: YBB HQ
  + Type: Agent Based
* Name: Corporate Team
  + Site: YBB HQ
  + Type: Agent Based

### Agents will use Webex messaging while in the agent desktop. The title of the desktop layout should say Yellow Brick Bank instead of Webex Contact Center.

Contact Center > Desktop Experience > Desktop Layouts

* Name: YBB Layout
* Teams: Corporate and Investment
* Download the default desktop layout
* Open the file with a text editor
* Look for “agent”
  + "appTitle": "Webex Contact Center" change to “Yellow Brick Bank”
  + “desktopChatApp”: “webexConfigured”: change false to true
* Save the file as YBBDesktopLayout.json
* Upload it to Desktop Layout
* Create the Layout

### Outcomes for each customer/agent interaction and agent idle times need to be categorized and tracked for reporting and analysis.

Contact Center > Desktop Experience > Idle/Wrap-up Codes

Create 2 Wrap-up codes

Name: Account inquiry

* Description: DEFAULT - General account questions
* Make it default: enable
* Code type: Default Wrapup Work Type

Name: Complaint

* Description: Customer issues
* Type: Default Wrapup Work Type

Create 2 Idle Codes

Name: Administration Time

* Description: Agent default non-available state
* Make it default: enable
* Type: Default idle Work Type

Name: Break

* Description: All scheduled breaks
* Type: Default idle Work Type

| Help articles | |
| --- | --- |
| [Manage sites](https://help.webex.com/en-us/article/nqipixt/Manage-sites-in-Webex-Contact-Center) | [Idle/Wrap-up codes](https://help.webex.com/en-us/article/n5595zd/Webex-Contact-Center-Setup-and-Administration-Guide#topic_39CCD35745C5E4E4629965AC29165CE8) |
| [Manage teams](https://help.webex.com/en-us/article/mqf72s/Manage-teams-in-Webex-Contact-Center) | [Manage desktop layouts](https://help.webex.com/en-us/article/60x9ji/Manage-desktop-layouts) |

STOP: End of Lab 5

Raise your hand and leave it raised in the Webex Meeting. Wait for further instruction.  
![](assets/docx-image-009.png)
