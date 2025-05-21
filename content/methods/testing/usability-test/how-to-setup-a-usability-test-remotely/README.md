# How to setup a usability test (remotely)

In this tutorial we're gonna explain how to set up a remote usability test. There are two versions of doing a usability test remote:

**Half remote**: this means that your participants aren't physically with you when doing the tests.

**Fully remote:** this means your participants **and** the observants aren't physically with you when doing the tests.

## Half remote

### What stuff do I need to get going?

No need for a big suitcase anymore! The following items should be enough when at a client!

* Your Macbook and a charger
* Stable internet connection (important!)
* A long HDMI Cable (that can reach the observation room)
* Television in the observation room to see the tests

### Step 1: Get your remote testing software of choice

When testing remotely it's important to use a remote testing / conferencing tool with good stability. We recommend the following ones:

* [Lookback.io](https://lookback.io/) (includes a way to test on mobile)
* [Zoom.us](https://zoom.us/)
* [Skype for Business](https://www.skype.com/nl/business/) (only includes calling / screen sharing)

In this tutorial I won't go into detail on how to use these tools. There are plenty guides online on how to set these up for remote testing. Before the day of the test, make sure before the participants know which tool they are expected to use and also instruct them how to these up.&#x20;

### Step 2: Share your screen and audio with the observation room

In order for the observation room to follow the test they need to see your screen (where the call is happening) and hear your audio. Here's how to set this up:

* Connect the long HDMI cable from your Macbook to the observation room TV
* Make sure to mirror your screen, and not let it act as a separate display
* Install [Loopback](https://rogueamoeba.com/loopback/) to mirror your audio (license can be found on our [1Password](https://app.gitbook.com/@hikeone/s/company-playbook/getting-started/tools/1password))&#x20;

#### Here's how to set up Loopback:

* Copy Loopback to your Application folder and open it
* Go through the install
* From the menu bar click license and fill in the name and key from 1Password
* Now click the plus button next to sources and choose the internal microphone
* On the right click the plus button next to monitors
* Here choose the TV from the list that your laptop is connected to through HDMI

All audio should now be passed through to your observation room TV!

![Loopback all set up!](<../../../../.gitbook/assets/image (20).png>)



### Step 3: Recording the test

Now the observation room is all set we can start testing! Load up your prototype and your favourite tool for remote testing.&#x20;

Most tools like Lookback and Zoom have built in screen recorder to save the tests. If your tool does not you can always use [Quicktime](https://support.apple.com/en-gb/guide/quicktime-player/qtp97b08e666/mac) or [Screenflow](https://www.telestream.net/screenflow/) (download this through our shared Apple ID from the App store)&#x20;

## Fully remote

### What stuff do I need to get going?

* Your Macbook and a charger
* Stable internet connection (important!)
* [Digital observation board ](https://miro.com/app/board/o9J_ksvhwzc=/)

### Step 1: Get your remote testing software of choice

When testing remotely it's important to use a remote testing / conferencing tool with good stability. We recommend the following ones. Check out the [step to step tutorials](set-up-tools-steven.md) to set each one of them.

**First choice**

* [Lookback.io](https://lookback.io/) (includes a way to test on mobile)

**Second choice**

* [Zoom.us](https://zoom.us/)

**Third choice**

* [Skype for Business](https://www.skype.com/nl/business/) (only includes calling / screen sharing)
* Microsoft teams
* Hangouts
* Gotomeeting

### Step 2: Stream the interview with observants

Depending on the choice of software for remote testing you can either allow observants to dial in the same call or share a live stream link.&#x20;

### Step 3: Recording the test

Most tools like Lookback and Zoom have built in screen recorder to save the tests. If your tool does not you can always use [Quicktime](https://support.apple.com/en-gb/guide/quicktime-player/qtp97b08e666/mac) or [Screenflow](https://www.telestream.net/screenflow/) (download this through our shared Apple ID from the App store)&#x20;

Use [otter.ai](https://otter.ai/) for the transcript of the interviews.

### Step 4: write down insights

Check out the [voltage control board](https://voltagecontrol.com/blog/the-voltage-control-design-sprint-scorecard/) to track digital insights and a quick way of answering your assumptions. For the nerdy ones: use this script in script editor to create automatic timestamps:&#x20;

```
function onEdit() {
var s = SpreadsheetApp.getActiveSheet();
if( s.getName() == "Ivo","Frank") { //checks that we're on Sheet1 or not
var r = s.getActiveCell();
if( r.getColumn() == 3 ) { //checks that the cell being edited is in column A
var nextCell = r.offset(0, 1);
if( nextCell.getValue() === '' ) //checks if the adjacent cell is empty or not?
nextCell.setValue(new Date());
}
}
}

```

→ Make sure to check out the [step to step tutorials](set-up-tools-steven.md) for streaming and recording of each of our recommended tools.

## Tips

Some tips especially for doing a remote test:

### **Do's**

* Communicate up front (also let NDA signed if needed)
* Hide and mute the observation team
* Be extra friendly
* Expect every tech failure and prepare for it
* Take time difference into account (protip: user interviews)
* Decrease your research scope
* Use tools you know

### **Don'ts**

* Panic.
* Let yourself get distracted. Try to focus and find a quiet and comfortable work area.
* Trust that participants read the communication up front.
* Let a border be a reason not to do research.

## Template for instructions for the respondents of the test

Before the test takes place, make sure you send emails with the necessary information to the respondents. Below you will find templates to use when the test will be done using Lookback and Zoom. It's best to send one email a week ahead of the test with general information about how the respondent should prepare for the test, and one email a day before the test starts in which you will remind about the most important things the respondent needs to keep in mind.&#x20;

### Lookback&#x20;

#### **Mobile (one week before the test)**

Hi \[participant name],

I am \[your name] from Hike One and I’m really happy to hear you are able to give us feedback about the product we are working on. The product you will be testing is \[shortly explain what the user will be testing]. Your input will help us improve it. I would like to inform you about our interview on the \[date]. Some notes up front:

* The test will be conducted **remotely**.
* To participate, you will need a **tablet** or a **mobile phone** with a properly working **microphone**, **camera** and  **Wi-Fi connection**.
* Please, make sure to have a **headphone set** on hand when participating. That way we will be able to hear you better.
* Before the test begins, please download a **Lookback Participate app**. You can download it for iOS ([https://apps.apple.com/us/app/lookback-participate/id1465098893](https://apps.apple.com/us/app/lookback-participate/id1465098893)) or for Android ([https://play.google.com/store/apps/details?id=io.lookback.participate](https://play.google.com/store/apps/details?id=io.lookback.participate)).
* On the day of the test, you can **join the session** through this link: \[link to the session].
* We will **record** the interview, for internal purposes only. This way the research team can look back at it if needed. The recordings will be deleted when they do not value the research anymore. We will not save the recordings longer than 2 years. You can read information about the processing of personal data in our privacy statement ([https://hike.one/topic/privacy-statement](https://hike.one/topic/privacy-statement)). If you do not want us to record the interview, please let me know up front.
* The recording obtained during the test might be used for commercial goals. For confidentiality purposes, have attached a **NDA form** to this email and we would like to ask you to  fill it in and send it back to us before the test. This can be done digitally.&#x20;

If you have questions let me know. I’m looking forward to meeting you next \[day]!

Best regards,

\[your name]



**Mobile (one day before the test)**

Hi \[name of the participant],

I’m really looking forward to testing \[name of the product] with you tomorrow. My colleague \[Name note-taker] or myself will be the interviewer who is going to guide you through the research. Some things to keep in mind before the interview:

* Please make sure that you have a **headset** on hand, that way we will be able to hear you better.
* Make sure you have installed the **Lookback Participate app** on your phone.
* Use this link to **join the session**: \[link].
* The link will open in the Lookback Participate app. Please follow the instructions on the screen and enable access to your **microphone**, **camera** and **screen recording**.
* We will call you within the app once you are ready.&#x20;

Don’t hesitate to contact me if you have any questions. I am looking forward to meeting you tomorrow!

Best regards,

\[your name]



#### **Desktop (one week before the test)**

Hi \[participant name],

I am \[your name] from Hike One and I’m really happy to hear you are able to give us feedback about the product we are working on. The product you will be testing is \[shortly explain what the user will be testing]. Your input will help us to improve it. I would like to inform you about our interview on the \[date]. Some notes up front:

* The test will be conducted **remotely**.
* To participate, you will need a **desktop computer** or a **laptop** with a properly working **microphone**, **camera** and  **Wi-Fi connection**.
* Please, make sure to have a **headphone set** on hand when participating. That way we will be able to hear you better.
* Before the test begins, please make sure you have **Google Chrome** installed on your computer. If that’s not the case, please download it and install it. You can download it here:[ https://www.google.com/chrome/](https://www.google.com/chrome/).
* On the day of the test, you can **join the session** by clicking on this link: \[link to the session]. Before you are able to join, you will be asked to install a **browser extension**. Follow the instructions that will appear on the screen after you click on the link to the session above.
* We will **record** the interview, for internal purposes only. This way the research team can look back at it if needed. The recordings will be deleted when they do not value the research anymore. We will not save the recordings longer than 2 years. You can read information about the processing of personal data in our privacy statement ([https://hike.one/topic/privacy-statement](https://hike.one/topic/privacy-statement)). If you do not want us to record the interview, please let me know up front.
* The recording obtained during the test might be used for commercial goals. For confidentiality purposes, have attached a **NDA form** to this email and we would like to ask you to  fill it in and send it back to us before the test. This can be done digitally.&#x20;

If you have questions let me know. I’m looking forward to meeting you next \[day]!

Best regards,

\[your name]



#### **Desktop (one day before the test)**

Hi \[name of the participant],

I’m really looking forward to testing \[name of the product] with you tomorrow. My colleague \[Name note-taker] or myself will be the interviewer who is going to guide you through the research. Some things to keep in mind before the interview:

* Please make sure that you have a **headset** on hand, that way we will be able to hear you better.
* Use this link to **join the session**: \[link]. Please, make sure that you open the link in **Google Chrome**.
* After opening the link, you will be asked to install a **browser extension**. Please follow the steps on the screen. Make sure that the access to your **microphone**, **camera** and **screen sharing** is enabled.
* Once you have set up, we will call you to begin the test.

Don’t hesitate to contact me if you have any questions. I am looking forward to meeting you tomorrow!

Best regards,

\[your name]



### Zoom&#x20;

#### **Mobile (one week before the test)**

Hi \[participant name],

I am \[your name] from Hike One and I’m really happy to hear you are able to give us feedback about the product we are working on. The product you will be testing is \[shortly explain what the user will be testing]. Your input will help us to improve it. I would like to inform you about our interview on the \[date]. Some notes up front:

* The test will be conducted **remotely**.
* To participate, you will need a **tablet** or a **mobile phone** with a properly working **microphone**, **camera** and a **Wi-Fi connection**.
* Please, make sure to have a **headphone set** on hand when participating. That way we will be able to hear you better.
* Before the test begins, please download the **Zoom app**. You can download it for iOS ([https://apps.apple.com/nl/app/zoom-cloud-meetings/id546505307](https://apps.apple.com/nl/app/zoom-cloud-meetings/id546505307)) or for Android ([https://play.google.com/store/apps/details?id=us.zoom.videomeetings\&hl=nl\&gl=US](https://play.google.com/store/apps/details?id=us.zoom.videomeetings\&hl=nl\&gl=US))
* Please install \[name of the prototyping app] on your phone. You can download it from here: \[link].
* On the day of the test, you can **join the session** through this link: \[link to the session].
* We will **record** the interview, for internal purposes only. This way the research team can look back at it if needed. The recordings will be deleted when they do not value the research anymore. We will not save the recordings longer than 2 years. You can read information about the processing of personal data in our privacy statement ([https://hike.one/topic/privacy-statement](https://hike.one/topic/privacy-statement)). If you do not want us to record the interview, please let me know up front.
* The recording obtained during the test might be used for commercial goals. For confidentiality purposes, have attached a **NDA form** to this email and we would like to ask you to  fill it in and send it back to us before the test. This can be done digitally.&#x20;

If you have questions let me know. I’m looking forward to meeting you next \[day]!

Best regards,

\[your name]



#### Mobile (one day before the test)

Hi \[name of the participant],

I’m really looking forward to testing \[name of the product] with you tomorrow. My colleague \[Name note-taker] or myself will be the interviewer who is going to guide you through the research. Some things to keep in mind before the interview:

* Please make sure that you have a **headset** on hand, that way we will be able to hear you better.
* Use this link to **join the session**: \[link].
* The link will open in the Zoom app.&#x20;

Don’t hesitate to contact me if you have any questions. I am looking forward to meeting you tomorrow!

Best regards,

\[your name]



#### Desktop (one week before the test)

Hi \[participant name],

I am \[your name] from Hike One and I’m really happy to hear you are able to give us feedback about the product we are working on. The product you will be testing is \[ shortly explain what the user will be testing]. Your input will help us to improve it. I would like to inform you about our interview on the \[date]. Some notes up front:

* The test will be conducted **remotely**.
* To participate, you will need a **desktop computer** or a **laptop** with a properly working **microphone**, **camera** and **Wi-Fi connection**.
* Please, make sure to have a **headphone set** on hand when participating. That way we will be able to hear you better.
* Before the test begins, please make sure you have **Zoom** installed on your computer. If that’s not the case, please download it and install it. You can download it here:[ https://zoom.us/download](https://zoom.us/download).&#x20;
* On the day of the test, you can **join the session** by clicking on this link: \[link to the session].
* We will **record** the interview, for internal purposes only. This way the research team can look back at it if needed. The recordings will be deleted when they do not value the research anymore. We will not save the recordings longer than 2 years. You can read information about the processing of personal data in our privacy statement ([https://hike.one/topic/privacy-statement](https://hike.one/topic/privacy-statement)). If you do not want us to record the interview, please let me know up front.
* The recording obtained during the test might be used for commercial goals. For confidentiality purposes, have attached a **NDA form** to this email and we would like to ask you to  fill it in and send it back to us before the test. This can be done digitally.&#x20;

If you have questions let me know. I’m looking forward to meeting you next \[day]!

Best regards,

\[your name]



#### Desktop (one day before the test)

Hi \[name of the participant],

I’m really looking forward to testing \[name of the product] with you tomorrow. My colleague \[Name note-taker] or myself will be the interviewer who is going to guide you through the research. Some things to keep in mind before the interview:

* Please make sure that you have a **headset** on hand, that way we will be able to hear you better.
* Use this link to **join the session**: \[link].

Don’t hesitate to contact me if you have any questions. I am looking forward to meeting you tomorrow!

Best regards,

\[your name]\


## Declaration of consent&#x20;

When sending an email a week in advance of the test, you should also include a declaration of consent form that the respondent should fill in and send back to us. For this purpose, use the following text:

**Declaration of consent**

We process your personal data in order to be able to carry out our research and to report on it. You have been informed about this prior to the research. Information about the processing of personal data can be found in our privacy statement: ([https://hike.one/topic/privacy-statement](https://hike.one/topic/privacy-statement)).\


In addition, we would like to ask your permission for photos and video material on which you are recognizable to use for promotional purposes, for example for display on our website. This permission is not mandatory and can be revoked at any time by you.

* I authorize Hike One to use photos for promotional purposes (website, presentation of this project to third parties). - optional -&#x20;
* I realize that all information about the products and / or services we test during the investigation is confidential. I declare that I will treat all information that I will keep strictly confidential during or in connection with the study and that I will not disclose it to third parties.

Only Dutch law applies to this statement. In the event of a dispute with regard to this statement, only the court in The Hague is competent to take cognizance.\


\
Name

\---------------------------------------------------------------&#x20;

Date

\---------------------------------------------------------------&#x20;

Signature

\---------------------------------------------------------------&#x20;
