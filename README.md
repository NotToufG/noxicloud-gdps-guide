# 1 / Getting Started
## Hello! You're probably reading this because you're struggling with making a GDPS, or you're just getting started. I'll show you how to do just that using the tools created by Noxi and the other awesome people behind NoxiCloud.
### NOTE: This is a PC only tutorial.
## 1.1 / Creating the GDPS
So first, you'll start by running /creategdps [GDPS Name] [GDPS Password] inside of #create-gdps. Easy enough, right?
Once you're done with that, you can go to https://ncpanel.noxicloud.es:8083 to manage your GDPS (PMA, File manager, host name, etc). You'll enter the name and password that you gave it while creating the GDPS!
## 1.2 / Making an executable
Great, so you've made your GDPS, and learnt how to access PMA, File Manager etc.! You wanna test some stuff out with your GDPS before getting ready to share it to the public? Or do you just want to make a download? You'll learn how to right here!
### 1.2.1 / For Windows
First things first, go to https://drive.google.com/drive/folders/1uCxe6dkNYu9jq_bV2U-QfobvT4NWOJPH and grab yourself the "Geometry Dash 2.204.zip" compressed folder! Once you're done doing that, **extract the zipped folder inside a folder with a name of your choice.** 
After doing that, **Run /getpc in #create-gdps and place the Geometry Dash.exe inside of your folder!**
(**WARNING: Don't forget to rename the Geometry Dash.exe to anything else, otherwise your GDPS' settings will override your Geometry Dash settings!**)
### 1.2.2 / For Android
Wanna make it available for your mobile peeps? Look no further!

Before starting, I'd like to mention that **you'll need Java.**

The first thing you'll want to do is to once again **go to https://drive.google.com/drive/folders/1uCxe6dkNYu9jq_bV2U-QfobvT4NWOJPH, and get yourself the "Geometry Dash 2.205.apk" package file!**
Once you're done with this, you'll need to **download https://drive.google.com/file/d/1UM2FJgXxN_AFmk0miT-N9PMvrGzRiRLG/ and extract it in a folder of your choice.**
Great! You're almost there.
**Take your "Geometry Dash 2.205.apk" file, and put it inside your APK Tool folder, then Rename it to "GD2.2.apk".**
This is the final stretch before you can start distributing your APK to your mobile players!
**Decompile your APK using the "Decompile GD 2.2.bat" script**, and after that you'll want to **edit the 12th line of "AndroidManifest.xml"**. **Replace all instances of "com.robtopx.geometryjump" with anything you want! (Don't replace the dots or the com!)**
### NOTE: The replacement of "com.robtopx.geometryjump" must be exactly 24 characters long, with "robtopx" being 7 characters and "geometryjump" being 12 characters.
Almost done! **You'll want to go inside of the "smali" folder, and rename the robtopx folder to what you renamed it in "AndroidManifest.xml". After that, go inside of the folder and rename the "geometryjump" folder in the same manner.**
After you're done doing that, you'll **go back to the server in #create-gdps, and you'll run /getapk.** Once you ran it, **download the files, go to the lib folder and move the files the command generated for you in their respective folders after renaming them to the previous files names.**
Once you've done that, **go to the res folder, then the values folder and edit "strings.xml" to change the GDPS's name. You'll replace Geometry Dash with your GDPS's name.**

### You're finally ready to compile your APK!

Get ready to compile your APK! **Open the "Compile your GDPS.bat" script to compile the APK!" After it's done compiling, open the GD2.2 folder and go to the build folder, then grab your APK.**

**Go to the signtool folder, and run the "Sign your APK.bat" script. After it's done doing it's thing, the last file that it generated is your signed GDPS APK! You can now share it to others :)**
# 2 / Configurations
## Awesome! You just made your GDPS's .exe and .apk! You can start adding roles inside of phpMyAdmin.
## 2.1 / phpMyAdmin Roles

**You will go in phpMyAdmin using the Control Panel, and then enter [GDPS name]_gdps, and your password!**

**After that, go to roles, and press insert. 
Then create your roles and put the permissions you want them to have except IsDefault (Unless your GDPS is an All Admin GDPS)**
### NOTE: You will need to set a color using RBG values and give it an icon with modBadgeLevel set from 1-3!

## Troubleshooting
### Forgot your PMA password? Go to the Control Panel, then DB, hover on your GDPS, click the orange edit icon tool and change your password! (you will need to change it inside of the config in File Manager aswell)
### GDPS not working? Send a message in #support or create a forum post in #noxicloud-support.
### Roles not working? check step 2.1 properly!
