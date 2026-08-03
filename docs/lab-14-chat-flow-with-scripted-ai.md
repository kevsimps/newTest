# Lab 14: Chat flow with scripted AI

In this lab, you will learn how to configure a flow for a Scripted AI.

### Access AI Agent Studio:

Contact Center > Overview > **Webex Connect** > App Tray >

AI Agent Studio

### Customer wants to add a Scripted AI agent

AI Agent Studio > Create agent

* Create agent
* Start From Scratch
* Agent Name: YBBAgent
* Create

### Create an Intent to trigger the custom responses

AI Agent Studio > Script > Intents

**Create intent**

* Intent name: Investment Banking
* Intent Description: Investment
* Utterances: “Investment”
* Add
* Generate
* Description: “I am interested in Investments”
* Generate
* Response name: Create New
  + Response Name: Investment
  + Text Variant 1: “Yellow Brick Bank has the best investments brokers in the market, with years in experience growing your assets. Type human to chat with an broker”
  + Create
* Add

**Create intent**

* Intent name: Corporate Banking
* Intent Description: Corporate
* Utterances: “Corporate”
* Add
* Generate
  + Description: “I want more information about Corporate Banking”
* Generate
* Response name: Create New
  + Response Name: Corporate
  + Text Variant 1: “Corporate Banking services, includes Financial Services as well as Insurance Management. Type human to chat with an Agent.”
  + Create
* Add

Save AI agent configuration

* Publish
* Comment: “bot”
* Publish

### Optional Step for the AI Agent Lab (after class)

* Yellow Brick Bank wants to receive chats with an AI agent with the Contact Center

**Webex Connect** > Services > My First Service > Flows

Disable previous flow: Toggle off the State button for the Chat inbound flow

Create a new Chat Flow

* Flow Name: AI agent Chat
* Upload: Chat\_AI\_Agent
* Save the Configure Mobile & Web App Event

Search Conversation node

* Authorize with Cholland after screen fully loads
* Save

Pre-chat form node

* Form Template: ChatForm
* Save

Receive node

* Form Template: ChatForm
* Save
* 2nd Receive node: Open and Save, DO NOT MAKE CHANGES

Resolve Conversation node

* Authorize with Cholland after screen fully loads
* Add Flow ID: All numbers at the end of URL in your tab, after the equals sign
* Save

Append Conversation node (all 4 nodes)

* Authorize with Cholland after screen fully loads
* Save

AI Agent node

* Agent Type: Scripted
* Agent: YBBBot
* Save

Queue Task node

* Authorize with Cholland after screen fully loads
* Queue Name: Chat Q
* Save

AI Agent Close Session node (2 nodes)

* Agent Type: Scripted
* Bot: YBBBot
* Save

Close Task node

* Authorize with Cholland after screen fully loads
* Save

Setting Gear Icon:

* General: Disable descriptive logs
* Select: Custom Variables
* liveChatDomain: [www.w3schools.com](http://www.w3schools.com)
* AppID: Chat Asset ID copied and saved earlier
* Make Live
* Application: Chat\_Asset

**Testing chat feature: Agent Login**

Open new browser (not a new tab but a different browser)

* Got to: <https://desktop.wxcc-us1.cisco.com/>
* Login as Eric Steele
  + Password is the same as Charles Holland
  + Use Desktop for Audio / Calls
  + Change state to available

**Testing chat feature: Customer experience**

New tab in browser > [www.w3schools.com](http://www.w3schools.com)

* HTML – Try it Yourself
  + Paste copied installation code between <p>This is a paragraph. </p> and </body>.
  + Run the code

Start and new Conversation with the AI, using “Corporate” or “Investment” words, the generated utterances as well, check responses, also try to trigger the handover with the word “human”

| Help articles | |
| --- | --- |
| [Webex AI Agent Studio Administration guide](https://help.webex.com/en-us/article/ncs9r37/Webex-AI-Agent-Studio-Administration-guide) |  |

STOP: End of Lab 14

Raise your hand and leave it raised in the Webex Meeting. Wait for further instruction.  
![](assets/docx-image-025.png)
