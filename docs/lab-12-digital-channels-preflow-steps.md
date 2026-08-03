# Lab 12: Digital channels preflow steps

In this lab, you will learn how to create a chat queue, an asset, and a channel.

### Yellow Brick Bank wants customers to be able to chat with agents from their website.

Contact Center > Overview > **Webex Connect** > Assets > Integrations

*Hint: Hover over icons in the left navigation bar of Webex Connect to find Assets*

* Webex CC Tasks: Action: Manage
  + Node Authorizations
    - WxCC Authorisation: Action: Add Authentication
      * Cholland email
      * Sign in as Cholland in the popup window
* Webex CC Engage: Action: Manage
  + Node Authorizations
    - WxCC Engage Authorisation: Action
    - Add Authentication: Cholland email

### Customer needs an ability to route chats.

Contact Center > Overview > **Webex Connect** > Assets > Apps > Configure New App > Configure New App: Mobile/Web

* Name: Chat\_Asset
* Channels: Web Push and/or Live Chat
* Live Chat/ In-App Messaging: enable
  + Primary Protocol: MQTT
  + Secondary Protocol: Web Socket
* Use a Secure Port: Enable

After saving:

* Register to Webex Engage: My First Service
* Return to Apps main page
* Copy and save App ID

### Customer needs a queue specifically for chat

Contact Center > Customer Experience > Queues > Create a queue

* Queue Name: Chat Q
* Channel Type: Chat
* Routing Pattern: Longest Available
* Chat distribution: Create a group
* Priority 1 – Corporate and Investment teams
* Service Level Threshold: 7200
* Max time in Queue: 80100

### Customer wants to receive chats into the Contact Center

Contact Center > Customer Experience > Channels > Create a channel

* Name: Chat Entry
* Channel type: Chat
* Asset Name: Chat\_Asset
* Service Level: 7200
* Timezone: NewYork

| Help articles | |
| --- | --- |
| [Set up digital channels](https://help.webex.com/en-us/article/n954r0k/Set-up-digital-channels-in-Webex-Contact-Center) |  |

STOP: End of Lab 12

Raise your hand and leave it raised in the Webex Meeting. Wait for further instruction.  
![](assets/docx-image-022.png)
