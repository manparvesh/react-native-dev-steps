# react-native-dev-steps
Personal notes to run and develop react-native apps

### Creating and running a new project
- Start with connecting the mobile device to the system.
- Check if it's connected by using `adb devices`
- check if the `ANDROID_HOME` variable is set. If not, add these lines to ~/.bashrc file:  
`export ANDROID_HOME=~/Android/Sdk`  
`export PATH=${PATH}:${ANDROID_HOME}/tools`  
`export PATH=${PATH}:${ANDROID_HOME}/platform-tools`  
- To initialize react native project, run `sudo react-native init ProjectName`
- `cd ProjectName`
- `sudo react-native run-android` to build and run app on android device. Red screen appears
- `adb reverse tcp:8081 tcp:8081` to direct the server requests to the system, since we are not using an emulator
- `sudo npm start` to start the server.
- Now just reload the app by tapping on reload.
- Set live editing from the menu (menu appears by shaking the device).
