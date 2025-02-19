# Gigya-iOS-ObjC-Demo

This is an iOS Demo project written in Objective-C with XCode that provide demos of Gigya's native iOS SDK and related functionality. It provides demos of the following:

 * Login (Native Social)
 * Login with RaaS
 * Logout
 * Facebook and Google+ Native Login
 * Making an API Request
 * Session Linking with GSWebBridge
 * Comments Plugin View
 * Publish User Action with Facebook Additional Permission Request
 
## Configuration
**IMPORTANT** Ensure your version of XCode is updated to the latest version. 

1. Extract the the iOS sample application in your Documents folder.
2. Ensure that you have Cocoapods installed -- see section below.
3. In a Terminal, navigate to where your sample application has been extracted. E.g. ```cd ~/Documents/SampleApp```
4. You should see the ```podfile``` in this folder, run the pod installer with the following command:
```shell
$ pod install
````
5. Cocoapods should now fetch all the files as defined in the podfiles of the root of the project files and copy it into the main xcode project. This will take a bit of time so you must now wait for this process to complete.
6. Open XCode
7. Open the ```.xcworkspace``` file. 
8. Build and run the project. 

If you receive any errors, follow the remediation steps below.

## Installing Cocoapods
1. Open a Terminal
2. Run the following command
```shell
$ sudo gem install cocoapods
```
If you get any errors here, please visit the following guide: https://guides.cocoapods.org/using/troubleshooting#installing-cocoapods

## XCode Remediation Steps
If the project fails to compile, perform the following steps:

1. Completely quit XCode.
2. Reopen XCode, but do not reopen the workspace or project.
3. Open Finder and find the ```.xcworkspace``` file, open the file through the Finder.
4. From the Menu, select **Product > Clean** to clear all temp files.
5. From the Menu, select **Product > Build**. 
6. Ensure that you have a target set for the Apple Simulator.

These steps will ensuer that all cocoapods files installed by ```pod``` are included in xcode and the project should compile and run in the Apple Simulator.
