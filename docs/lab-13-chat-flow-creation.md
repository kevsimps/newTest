# Lab 13: Chat flow creation

In this lab, you will learn how to connect chats to a flow and to receive a chat on an Agent Desktop.

### Add a form to collect information.

Contact Center > Overview > **Webex Connect** > Tools > Templates

* *Hint: Hover over icons in the left navigation bar of Webex Connect to find Assets*
* Add New Template
* Name: ChatForm
* Channel: Live Chat / In-App Messaging
* Message Type: Form
* Title: Welcome. Please tell us about you in this form and indicate if you are interested in Corporate or Investment Banking.
* Form Fields: Add Field
  + Type: Email
  + Name: customerEmail
  + Label: customerEmail
  + Mandatory Field: enable
  + Description: Email Address
  + Save
* Form Fields: Add Field
  + Type: Name
  + Name: customerName
  + Label: customerName
  + Mandatory Field: enable
  + Description: Your Name
  + Save
* Save

### The chat experience must be user friendly and match Yellow Brick Bank’s branding

Contact Center > Overview > **Webex Engage** > Assets > Channel Assets > LiveChat

* **Edit Chat\_Asset (pencil icon)**
* **Websites tab:** Add Website
  + Domain: www.w3schools.com
  + Display Name: Example Chat Window
  + Byline Text: This is the future!
  + Greeting message: How are you doing today? You will be connected shortly.
  + First Message: Hello World.
  + PCI Compliance Message: We have this.
* Customize widget style
  + Change color and widget button to your taste
* Widget Visibility
  + Consider Business hours: enable
  + Show without restrictions: enable
  + Save
  + Click back arrow next to Website Settings at top of page
* **Installation Tab**
* Copy code to use later

### Customer chats need to be routed to appropriate agents

Contact Center > Overview > **Webex Connect >** Services > My First Service > Flows > Create Flow

* Flow Name: Chat inbound
* Method: Upload Flow
* Provided by instructor: LiveChatInboundFlow
* Save the Configure APP Event
* IMPORTANT: Double click nodes to edit them.
* **Search Conversation node**
  + Node Authentication: Authorize with Cholland after screen fully loads
  + Save
* **Pre-chat form node**
  + Form Template: ChatForm
  + Save
* **Receive node**
  + Form Template: ChatForm
  + Save
* **Resolve Conversation node**
  + Node Authentication: Authorize with Cholland after screen fully loads
  + Flow ID: All numbers at the end of URL in your tab, after the equals sign
  + Save
* **Append Conversation node**
  + Node Authentication: Authorize with Cholland after screen fully loads
  + Save
* **Queue Task node**
  + Node Authentication: Authorize with Cholland after screen fully loads
  + Queue Name: Chat Q
  + Save
* **Close Task node**
  + Node Authentication: Authorize with Cholland after screen fully loads
  + Save
* **Setting Gear Icon:** (Top right of page)
  + General Tab: Disable descriptive logs
  + Custom Variables Tab
    - liveChatDomain: [www.w3schools.com](http://www.w3schools.com/)
    - AppID: Chat Asset ID copied and saved earlier (Ex: CH06153705)
* **Save**
* Make Live (upper right)
* Assets Configuration: App Selection
  + Application: Chat\_Asset
  + Make Live

### Testing chat feature: Agent Login

* Open new browser (not a new tab but a different browser)
* Got to: <https://desktop.wxcc-us1.cisco.com/>
* Login as Eric Steele or Kellie Melby
  + Password is the same as Charles Holland
  + Use Desktop for Audio / Calls
  + Change state to available

### Testing chat feature: Customer experience

New tab in browser > [www.w3schools.com](http://www.w3schools.com)

* HTML – Try it Yourself
* Paste copied installation code between <p>This is a paragraph. </p> and </body>
* Run the code
* Start a new conversation and converse between agent and “customer”

| Help articles | |
| --- | --- |
| [Configure flows for digital channels](https://help.webex.com/en-us/article/n954r0k/Set-up-digital-channels-in-Webex-Contact-Center#configure-flows-for-digital-channels) | [Connect Flow builder](https://help.webexconnect.io/docs/flows) |

STOP: End of Lab 13

Raise your hand and leave it raised in the Webex Meeting. Wait for further instruction.  
![](assets/docx-image-023.png)
