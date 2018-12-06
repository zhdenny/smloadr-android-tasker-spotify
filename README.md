**Update 1:** Forgot to mention. I did not provide the actual download icon file because I used one from an icon pack I purchased. So, just go inside the AutoTools Webscreen actiosn in the Tasks and look for the icon settings.....change the icon to whatever you want. You might have to size it too.....just play with the settings in there and you'll figure it out.

**Update 2:** Made a slight bug fix to the AutoNotification Actions in the Tasks to ensure the download buttons get triggered to show up when they should. Upadted Taskernet link in the installation instructions.

# smloadr-android-tasker-spotify

Android Tasker project to monitor what you listen to on Spotify and shows a button. Press the button and you'll get a popup verifying the song/album you are currently listening to. After tapping to confirm selection, it will (in the background) SSH into remote server and send smloadr commands related to the selection. See screenshots showing the green-outlined download button and the following verification popup. I have the button strategically placed depending on what app I'm in....I set it up to only show when I'm on the Now Playing Spotify screen or am Actively Navigation somewhere on the Google Maps navigation screen.

**REQUIREMENTS: Tasker, AutoTools, AutoInput, AutoNotification, and AutoWeb, AutoApps. You also need to have an SSH-accessible computer with smloadr functioning.**

Google Play Links to all the Apps:

https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm&hl=en_US

https://play.google.com/store/apps/details?id=com.joaomgcd.autotools

https://play.google.com/store/apps/details?id=com.joaomgcd.autoinput

https://play.google.com/store/apps/details?id=com.joaomgcd.autonotification

https://play.google.com/store/apps/details?id=com.joaomgcd.autoweb

https://play.google.com/store/apps/details?id=com.joaomgcd.autoappshub


**In AutoTools, go to Webscreens and import the "Bubble" webscreen and the "Notification" webscreen. In AutoWeb, go Import the Deezer API.**

**In addition, make you open each app and grant all permissions requested for each one ESPECIALLY TASKER** 

I know it is a lot of stuff required to get this working......but if you are any real Tasker user, you likely already have many of these tools under your belt already. And if you aren't a Tasker user yet, become one. The app is like Beethoven's 5th Symphony for Android.

<img src="/4uks8gp[1].png" width="50%" height="50%">

<img src="/oxrWkPd[1].png" width="50%" height="50%">

<img src="/T0Uy8lH[1].png" width="50%" height="50%">



**Installation:**

1. Once you installed all the apps above and granted permissions, import the Tasker project by visiting the link below. **You MUST go to the link using the Android Device you intend to do this with**

https://taskernet.com/shares/?user=AS35m8msFEo6EHcVYY6he6IGzxTQQrE5O8T1znp4uQKJ2EVnVHamQ%2Fr%2FvA96NayynBE%3D&id=Project%3ASpotify-smloadr

It should look like this (screenshot below)

<img src="/Screenshot_Chrome_20181203-132848.png" width="50%" height="50%">


2. After importing the project, open Tasker, find the project, and click to edit the task named "Dezzer Bubble Pressed" (sorry for the typo).

3. Read the section between the red text that describes setting variables for server_address, port, and username.

4. You'll also need to either type in the password for your SSH connection or the path to your private key. All described in the section between the red text how to do that.

5. Verify both profiles are enabled (they are named "Deezer Download Bubble Created -Spotify" and "Deezer Download Bubble Created -Maps"

6. Back out of Tasker. Test it out by Opening spotify and beginning to listen to something. You will only see the Download bubbles while you are on the Now Playing screen of Spotify OR on the Active Navigation Screen of Google Maps.

7. You MIGHT need to adjust the XY positions of the bubbles depending on your screen size (I'm not sure, I'm no dev). If you need to do this go back into Tasker, find the Tasks for creating the download bubbles. Edit the AutoTools Web Screen actions in Windows Settings, Offset X and Offset Y. The numbers in those fields dictate where on your screen the Download Bubbles will appear.
