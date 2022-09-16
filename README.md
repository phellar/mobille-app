# mobille-app
- Init Project
+ Open terminal 
+ cd to Root folder that included project
+ react-native init testmeup --version 0.61.0
+ cd testmeup		

- Install dependencies
+ npm install @react-native-community/async-storage@1.6.2
+ npm install react-native-barcode-mask@1.1.0
+ npm install react-native-camera@3.13.1
+ npm install react-native-gesture-handler@1.5.0
+ npm install react-navigation@4.0.10
+ npm install react-navigation-stack@1.10.3
+ npx react-native link

- Develop environment in MacOs - IOS
+ cd ios
+ pod install
If you run command pod install get error like “Unknown object version“, please run command in global (not in project): sudo gem install -n /usr/local/bin cocoapods
Then run command: pod install
+ cd root/testmeup


+ Run bellow command to surely you init project successfully.
  npx react-native run-ios
If if is fail, you have to follow error and fix it.

+ Copy App.js and ‘src’ from ‘Code’ folder in package to ‘testmeup’ folder

+ Run project:
  npx react-native run-ios


- Develop environment in MacOs - Android

+ Install Android Studio 3.5.3

+ Add permissions to your app android/app/src/main/AndroidManifest.xml file:
<!-- Required -->
<uses-permission android:name="android.permission.CAMERA" />

<!-- Include this only if you are planning to use the camera roll -->
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />

<!-- Include this only if you are planning to use the microphone for video recording -->
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
