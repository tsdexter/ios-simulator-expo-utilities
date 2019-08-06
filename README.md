# Run iOS Simulator App
### Background

I develop native apps with Expo and generally don't open xcode very often, however, I need to open the iOS Simulator all the time for testing/demos. You can do this from the expo server when running a dev app but I also run testing/demos from hosted expo apps in which case I need to open the simulator and enter the `exps` url into Safari directly. 

This is a simple automator app that uses the scripts from this answer: https://stackoverflow.com/a/10379712/786094 and gives you an app that you can keep in your dock (or run via spotlight/finder) to launch the iOS simulator without opening xcode.

Currently only supports xcode 7+

#### Todo

- add logic to check the xcode version and run appropriate script from stack answer (feel free to submit a pull request)

#### How to use

- make sure you have xcode 7+ installed
- download and unzip this repo 
- open the new directory and either run the `iOS Simulator` app directly from there or drag it to your dock and/or `Applications` folder for easy access
- You may have to allow this in your `Privacy/Security` preferences for it to run

---

# Expo Client installer for iOS Simulator
### Background

My clients want to be able to do demos of their apps for partners/clients/users etc... via skype/hangouts/etc. For this, they generally bring me on the call to screenshare my simulator. I wanted an easy way for them to run the simulator and an Expo app without having to install `expo-cli` and run the dev app.

This is a simple automator app that installs the Expo Client app on the iOS Simulator using the manual instructions available here: https://docs.expo.io/versions/latest/introduction/installation/ 

#### How to use

- make sure you have xcode 7+ installed
- download and unzip this repo 
- open the new directory and run the `Install Expo Client` app. 
- You may have to allow this in your `Privacy/Security` preferences for it to run
- this will take 30 seconds or so, depending on your internet connection (approx ~55mb currently to download expo client app, no progress indicator). It will be done when the simulator opens and `Expo` app is available
- If the app is not there, try running it again
