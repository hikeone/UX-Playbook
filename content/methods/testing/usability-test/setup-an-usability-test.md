# How to setup a usability test (local)

Following this step-by step tutorial you’ll be able to set up usability test recordings in no time! The initial setup takes some time (around 20 min) but after that you will be able to use your laptop for recording within a couple of seconds!

**It's best to open this guide on your iPhone or print it out since you can't view it on your Macbook during setup!** Short link to the guide to open on your phone: [http://bit.do/hikeone](http://bit.do/hikeone)

### What stuff do I need to get going?

No need for a big suitcase anymore! The following items should be enough when at a client!

* Your Macbook and a charger
* A long HDMI Cable (that can reach the observation room)
* External microphone / webcam (optional)
* Test device (Android / iOS)
* Television in the observation room to see the tests

### Step 1: Creating a Mac OS user account just for testing

To keep things clean and settings separate from your main work account is is recommended to create a new user account on your laptop. Switching to this user account will save time because it's optimised for recording usability tests.

Check out [this guide](https://support.apple.com/en-gb/guide/mac-help/mtusr001/mac) on how to set up new users on Apple's support page, it's strongly advised to give this user admin privileges as well due to application rights!

### Step 2: Get all software!

**Please only download the apps first, don't install them yet!**

For this setup we use the following apps:

* [Reflector 3](https://www.airsquirrels.com/reflector/download) (for wireless screen mirroring from your phone)
* [OBS](https://obsproject.com/download) (for recording )
* [Loopback](https://rogueamoeba.com/loopback/) (for audio pass-through)

The paid license information can be found on our shared [1Password](https://app.gitbook.com/@hikeone/s/company-playbook/getting-started/tools/1password) account!

### Step 3: Setting up Reflector first

In order to wirelessly see your test device screen on your Macbook wirelessly we have to set up Reflector 3 fitst

* Copy Reflector 3 to your Applications folder and open it up
* When asked for the license key, copy it in from our 1Password
* Let's adjust some settings! To open the preferences pane click the Reflector icon on the menu bar and click the cogwheel. Preferences should be first in the list (see screenshot below)

![Where to find the preferences in Reflector 3](<../../../.gitbook/assets/image (13).png>)

* In the general tab: **uncheck "always on top"**
* In the connection tab: **set show frame to "none"**
* Also in the connection tap **set "airplay security" to none**
* Now make sure your test device and Macbook are on the same WiFi network

If all is set up correctly you should be able [Airplay](https://support.apple.com/en-us/HT204289) or [Cast](https://support.google.com/chromecastbuiltin/answer/6059461?hl=en) to your Macbook! Your test device will appear on the Macbook's screen.

### Step 4: Setting up OBS

We use OBS as our main software to capture the test device screen and the webcam footage from the participant!&#x20;

* Copy OBS to your Application folder and open it
* **Accept** **all the permission prompts OBS will throw at you.** This is really important, to make everything function correctly.&#x20;
* Decline the automatic set up wizard

#### Setting up all sources

OBS works as a canvas to combine different input sources into a "scene". These sources can be for example Webcam footage or an application window. We want to set up a new scene for our test that we can re-use in the future. You can easily click the plus button under sources to add one!

![The sources panel](<../../../.gitbook/assets/image (5).png>)

#### Adding the webcam as a source&#x20;

* Click the plus button onder sources and choose "video capture device"
* Give it a name, we will call it "webcam"
* Now from the device dropdown select your Webcam (FaceTime HD Camera) and hit OK
* If all works well your should see your webcam source on the canvas!&#x20;
* You can drag around and resize the webcam footage on the canvas to your liking

#### Getting window capture to work

* In OBS click the plus button again under sources and select "Display capture"
* This should prompt you with the question if OBS can record your screen, grant this permission. **This warning could appear behind the OBS window!**
* Restart OBS
* **Check in&#x20;**_**System Preferences > Security & Privacy > Screen recording**_**&#x20; that OBS is checked**
* In OBS you can delete the display capture under sources that you've just created

![Make sure OBS is checked in the Screen recording permissions!](<../../../.gitbook/assets/image (6).png>)



#### Adding your test device screen as a source

* **Make sure your phone is displayed on your screen using Reflector**
* Go back to OBS when the screen recording is set
* Click the plus button again under sources and choose "Window Capture"
* Again give it a name
* Make sure your phone is displayed on your screen using Reflector
* From the window dropdown choose the Reflector window that is showing your phone screen and click OK
* Your phone screen should now be displayed on the canvas, again give it a nice spot!

#### Bonus: add the Hike One logo

For the professional touch you can also add the [Hike One logo](https://hike.one/static/images/logo-white.png) to the canvas corner.

* Click the plus button one last time
* Choose image and give it a name
* Under image File, browse for the logo and hit OK
* Drag / resize it to the corner of the screen

![Fully set up canvas!](<../../../.gitbook/assets/image (1).png>)

### &#x20;Step 5: Setting the output settings in OBS

Before we do any recording let's check if our video output settings are correct.&#x20;

* In the menu bar click on OBS name on the left top and choose Preferences
* The preference pane will show up, next click on Output
* Here you can set your recording output path (so where the videos will be saved) as well as the file format settings
* Be sure that the Recording format is set to .Mp4 or .Mov for the best compatibility!

### Step 6: Save your Canvas

If you're done with the setup of your canvas it's time to save it!

* In the menu bar choose "scene collection"
* Click on export
* Give it a name and save it on a good spot as a backup!

### Step 7: Connect to the observation room TV

Now let's connect your Macbook to the TV in the observation room!

* Connect your Macbook to the TV in the observation room using a HDMI cable
* Set the TV as a second screen (so no mirroring)
* In OBS, click right anywhere on the canvas and hover over Fullscreen Projector (Preview)
* Choose Display 2 (see screenshot below)&#x20;
* Your Canvas setup should now be displayed on the TV in the observation room!

![How to display your canvas on the external TV screen](<../../../.gitbook/assets/image (16).png>)

### Step 8: Pass-through audio using Loopback

Almost done! We need all audio captured from the Macbook microphone to be passed through to the speakers of the observation room TV. Otherwise we can't hear any feedback from the participants.

* Copy Loopback to your Application folder and open it
* Go through the install
* From the menu bar click license and fill in the name and key from 1Password
* Now click the plus button next to sources and choose the internal microphone
* On the right click the plus button next to monitors
* Here choose the TV from the list that your laptop is connected to through HDMI

All audio should now be passed through to your observation room TV!

![Loopback all set up!](<../../../.gitbook/assets/image (20).png>)

### Step 9: Let's record some stuff!

So how do you actually record all this stuff?

* Get back to OBS
* Click on start recording on the bottom right under controls
* The recording should be going on now!
* Click stop recording to stop it.
* That's it! You can check out the recordings quickly by choosing file in the menu bar and choosing "show recordings"



![Starting / Stopping the recording](https://paper-attachments.dropbox.com/s_128E3DA5466B3A2860D4D63E3F6EE6687154F9E20E3935876EF7EA31A332AE55_1578054883175_image.png)

###

### So how do I record my desktop prototype instead of my phone?

To test a desktop website instead of mobile just do the following:

* Open OBS
* Under scenes, next to sources copy your created scene by right clicking and choosing duplicate
* Rename the existing one to mobile and change the new scene to desktop to find them easier

![The scenes list](<../../../.gitbook/assets/image (19).png>)

* Rename the existing one to mobile and change the new scene to desktop to find them easier
* Open your prototype in your browser of choice
* In OBS in the the desktop scene double click the window capture from sources
* Instead of the reflector window choose your browser window with the prototype in it
* Resize the window on your canvas to your liking
* That's it, hit record to start recording!

### The next time, setup is going to be quick and easy!

Whoo good job, you're all set! This was quite a journey but don't worry the next time wil be quick now all has been set up. Just so the following:

* Switch to your Testing user account
* Make sure Reflector is running and your phone is being displayed on your Macbook
* Connect your Macbook to the observation room TV using the HDMI cable. Use the TV as separate display.
* Start Loopback and **make sure it's set to the right TV under monitors**
* Open OBS and it should load up your canvas with all the sources! If not click the sources and set them to the right ones.
* Right click anywhere on your setup and choose the fullscreen projector mode
* Hit record!

### After setup troubleshooting&#x20;

#### My phone display is not visible in OBS

Make sure the Window capture under sources is set to the right Reflector window that is displaying your phone.

#### My phone mirror keeps disappearing

This might happen because your phone went to sleep mode and stops the airplay. Set auto lock to never  on your phone to prevent this.

#### In the observation room I can't see my laptop's screen via HDMI

Double check that you've enabled projector mode! (In OBS, click right anywhere on the canvas and hover over Fullscreen Projector (Preview) Choose Display 2)

#### There is no sound in the observation room

First off check if the TV is not muted. Second double check if Loopback is running and that the monitor is set to the right TV in loopback!
