# Lab 7: Agents and supervisor resources and access

In this lab, you will learn how to create a user profile **Note: If a configuration option in Control Hub is not mentioned in the lab, skip that option.**

### Supervisors should have access only to features necessary for their roles

Contact Center > User Management > Access > Resource Collections > Create a resource collection

* Name: Supervisor RC
* Resources:
  + Channels: All
  + Queues: All
  + Skill definitions: All
  + Skill profiles: All
  + Sites: All
  + Teams: All

### User profiles must be configured to what a user can edit and view, and which resources they can access through resource collections.

Contact Center > User Management > Access > User profiles > Create a user profile

**General**

* Name: YBB Supervisor
* Description: Includes Supervisor RC
* Profile type: Supervisor

**Permissions (Don’t click next at the bottom until you have done all 3 tabs)**

Configurations tab

* Customer experience
  + Call recording schedules: Edit
* User Management
  + Skill Profiles: Edit
  + Contact center users: Edit
  + Skill definitions: Edit

Analytics tab

* Interactions and recordings > Interactions: View
* Reporting > Analyzer: Edit

Supervisory & desktop tab

* Agent management > Additional Supervisory
  + Edit: enable all
* Monitoring > Call listening
  + - Type and Actions: enable all
* Desktop > Multimedia
  + - Edit: Enable all

**Resource access**

* Allowed resources
  + Selected resource collections: Supervisor RC

### Contact Center must be enabled and all configured profiles must be assigned to each agent for them to take effect.

Contact Center > User Management > Contact Center Users

|  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- |
| Anita Perez - Supervisor Settings | | | | | |
| User Profile | Contact Center | | Primary team | | |
| YBB Supervisor | enable | | Corporate team | | |
| **Agent Settings** | | | | | |
| Site | | Teams | | Desktop Profile | Multimedia Profile |
| YBB HQ | | Investment, Corporate | | YBB Desktop Profile | Voice\_Chat\_MPP |

|  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- |
| Agents | | | | | | |
| User | Contact Center | Site | Teams | Desktop Profile | Multimedia Profile | Skill Profile |
| Eric Steele | enable | YBB HQ | Investment,  Corporate | YBB Desktop Profile | Voice\_Chat\_MPP | Eric\_SP |
| Kellie Melby | enable | YBB HQ | Investment,  Corporate | YBB Desktop Profile | Voice\_Chat\_MPP | Kellie\_ SP |
| Rebekah Barretta | enable | YBB HQ | Investment | YBB Desktop Profile | Voice\_Chat\_MPP | Rebekah\_SP |
| Ricardo Filice | enable | YBB HQ | Corporate | YBB Desktop Profile | Voice\_Chat\_MPP | Ricardo\_SP |
| Stefan Mauk | enable | YBB HQ | Corporate | YBB Desktop Profile | Voice\_Chat\_MPP | Stefan\_SP |
| Taylor Bard | enable | YBB HQ | Corporate | YBB Desktop Profile | Voice\_Chat\_MPP | Taylor\_SP |

| Help articles | |
| --- | --- |
| [Manage Contact Center users](https://help.webex.com/en-us/article/nzk6tpp/Manage-Contact-Center-Users) |  |

STOP: End of Lab 7

Raise your hand and leave it raised in the Webex Meeting. Wait for further instruction.  
![](assets/docx-image-011.png)
