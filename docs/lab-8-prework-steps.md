# Lab 8: Prework steps

In this lab, you will learn how to create audio prompts, queues, business hours and surveys. **Note: If a configuration option in Control Hub is not mentioned in the lab, skip that option.**

### Callers should hear appropriate recordings based on when and where they are calling.

Contact Center > Customer Experience > Audio Files

* Upload the following prompts from the lab files downloaded from Webex Academy
  + Office\_Closed.wav
  + Calls\_Recorded.wav

### Calls to queues will be handled based on operating hours.

Contact Center > Customer Experience > Business Hours

*Note: Configure the tabs from right to left*

Overrides

* Name: Emergencies
* Time zone: New York
* Add a new override
  + Name: Inclement Weather
    - Recurrence: Daily
    - No end date
    - Note: Check that the override status is disabled

Holiday Lists

* Name: US Holidays
  + Add a new holiday
    - Christmas
      * Duration: 12/25/2026 – 12/25/2026
      * Recurrence: Yearly
      * Every December on 25 day
      * No end date

Working Hours

* Name: YBB HQ Open Hours
* Time zone: New York
* Add Shift
  + Name: Work Week
  + Mon – Fri: - 9am - 5pm
* Holiday List: US Holidays
* Override: Emergencies

### Separate queues are needed for support teams to ensure customer inquiries are routed to the appropriate team

Contact Center > Customer Experience > Queues

Create Queue: Corporate Q

* + Description: Financial Services and Insurance Management
* Contact routing settings
  + Skills-based routing: Enable
  + Skill assignment type: Assign skills in flows
  + Routing pattern: Best Available
  + Call distribution: Create a group
    - Priority 1
    - Corporate team
  + Call distribution: Create a group
    - Priority 2
    - Add group after 60 Secs
    - Investment Team
  + *Note: Make sure to double check the priority before saving!*
* Advanced Settings
  + Service monitoring: Enable
  + Allow pause/resume for calls: Enable
  + Service level threshold: 120
  + Max time in queue: 3600
  + Default music in queue: defaultmusic\_on\_hold.wav

Create Queue: Investment Q

* + Description: Investments only
* Contact routing settings
  + Skills-based routing: Enable
  + Skill assignment type: Assign skills in queue
  + Routing pattern: Best Available
  + Add skill requirements:
    - Skill type: Proficiency
    - Skill name: Investment\_Lvl
    - Condition: >=
    - Skill Value: 5
  + Add skill requirement
  + Refresh the eligible user list
  + Save
* Advanced Settings
  + Service monitoring: Enable
  + Allow pause/resume for calls: Enable
  + Service Level Threshold: 120
  + Max time in Queue: 3600
  + Default music in queue: defaultmusic\_on\_hold.wav

### Callers will be asked to take a survey after each call.

Contact Center > Customer Experience > Surveys > Create a new survey

IVR Survey

* Survey name: Customer NPS

Questions

* Welcome Note: IVR audio prompt
  + Upload SurveyPrompt.wav from student lab material
* Add a question: NPS
  + IVR audio prompt
    - Upload NPS\_Survey.wav from student lab material
  + Question to show on reporting
    - How likely are you to recommend us?
* Thank you note: IVR audio prompt
  + Upload ThankyouNote.wav from student lab material

Error handling

* Do not make changes

| Help articles | |
| --- | --- |
| [Manage audio files](https://help.webex.com/en-us/article/be12vp/Manage-audio-files) | [Set up business hours](https://help.webex.com/en-us/article/dqekw4/Set-up-business-hours-for-Webex-Contact-Center) |
| [Create queues](https://help.webex.com/en-us/article/ubg5qd/Create-queues-and-configure-routing-patterns) | [Configure surveys](https://help.webex.com/en-us/article/nlu4x20/Experience-Management---Configure-surveys-for-IVR-and-Digital-Channels-for-WebexContact-Center) |

STOP: End of Lab 8

Raise your hand and leave it raised in the Webex Meeting. Wait for further instruction.  
![](assets/docx-image-012.png)
