# Integrating with Slack 

This tutorial will show you step by step instructions on how you can get your COVID Crisis Communication Assistant up and running with Slack
![Slack Gif](https://github.com/Call-for-Code/Solution-Starter-Kit-Communication-2020/blob/master/starter-kit/slack/readme_images/Slack.gif)

## Learning objectives

In this tutorial, you will:

- Learn about building a Slack App 
- Integrating your Slack App with Watson Assistant
- Build a Call for Code COVID Crisis Communications Slack enabled Chatbot solution

## Prerequisites

This tutorial assumes you have a Slack workspace with administrative rights. 
 - [Learn more about creating your slack workspace](https://slack.com/help/articles/206845317-Create-a-Slack-workspace)

This tutorial also assumes you have created a [Watson Assistant COVID Crisis Bot](https://github.com/Call-for-Code/Solution-Starter-Kit-Communication-2020#getting-started) 

Once you have a Slack Workspace and your Assistant up and running  .... 

## Lets Get Started! 

### Step 1. 
Go to your COVID Crisis Communications Assistant and **Add Integration** 

![Slack Integration Photo1 ](/starter-kit/slack/readme_images/Slack-Photo1.png)

### Step 2.
Scroll down to Third-party integration and Select Slack 

![Slack Integration Photo2 ](/starter-kit/slack/readme_images/Slack-Photo2.png)

### Step 3.
The first thing you will have to do is [Create a Slack App](https://api.slack.com/apps). Click on **Create New App** and give app a name and point to a slack development workspace. Learn more about creating slack apps [here](https://api.slack.com/start) 

![Slack Integration Photo3 ](/starter-kit/slack/readme_images/Slack-Photo3.png)

### Step 4.
On the Slack app settings page, go to the **Basic Information** tab and find the **App Credentials** section. Copy your verification token from that section to **section 1** of Step 2 on Watson Assistant Slack integration page 

![Slack Integration Photo4 ](/starter-kit/slack/readme_images/Slack-Photo4.png)
![Slack Integration Photo5 ](/starter-kit/slack/readme_images/Slack-Photo5.png)

(Optional) : Upload an App Icon and App Name in the Display information section of **Basic Information** tab 

![Slack Integration Photo- ](/starter-kit/slack/readme_images/Slack-Photo.png)


### Step 5.
Go to the **OAuth & Permissions tab**. In the **Bot Token Scopes** section click **Add an Oauth Scope**, and then select the following scopes:`app_mentions:read` `chat:write` `im:history` `im:read` `im:write`
![Slack Integration Photo6 ](/starter-kit/slack/readme_images/Slack-Photo6.png)


### Step 6.
On the **OAuth & Permissions** tab. Click **Install App** to Workspace, and then click **Allow**. You should be redirected back to the OAuth & Permissions page. **Note** Make sure you copy your Bot User OAuth access token (`starts with xoxb`)  to both of the fields in **section 3** of Step 2 on Watson Assistant Slack integration page 

![Slack Integration Photo7 ](/starter-kit/slack/readme_images/Slack-Photo7.png)
![Slack Integration Photo8 ](/starter-kit/slack/readme_images/Slack-Photo8.png)


### Step 7.
On the Slack app settings page, go to the **Event Subscriptions** tab. Switch the **Enable Events** toggle to the On position. On Step 3 of the Watson Assistant Slack Integration page click on **Generate Requestt URL** Paste request url and verify on **Enable Events** page 

![Slack Integration Photo9 ](/starter-kit/slack/readme_images/Slack-Photo9.png)

### Step 8.
On the Event Subscriptions tab, find the Subscribe to Bot Events section. Click Add Bot User Event, and then select the event types you want to subscribe to. You must select at least one of the following types: `message.im: Listens for message events that are posted in a direct message channel.` `    app_mention: Listens for only message events that mention your app or bot.` Make sure you save your changes

![Slack Integration Photo10 ](/starter-kit/slack/readme_images/Slack-Photo10.png)

### Step 9.
On the **App Home** tab. Click **Edit** and enter a display name and default username for your virtual assistant and then click **Save**. Enable the **Always Show My Bot as Online** toggle
![Slack Integration Photo11 ](/starter-kit/slack/readme_images/Slack-Photo11.png)

### Step 10.
On Watson Assistant Slack Integration page click **Save Changes**

### Step 11.
Log in to Slack workspace and click on **Browse App** Find the app you just created and add to workspace
![Slack Integration Photo12 ](/starter-kit/slack/readme_images/Slack-Photo12.png)

### Step 12.
Test app by asking questions based on intents and entities in your dialog tree! If you recieve answers back you have successfully integrated your COVID Crisis Communication Assistant!! 



