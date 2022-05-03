Oculus Documentation - Development Environment Setup
========
Aside from enabling developer mode for your Quest 2, you'll need some other resources to get started.

# Required Resources:
* [Unity - 2020.3.21](https://unity3d.com/get-unity/download)
* [Oculus Desktop App](https://www.oculus.com/setup/)
* [Oculus ADB Drivers](https://developer.oculus.com/downloads/package/oculus-go-adb-drivers/)
* [Android Studio](https://developer.android.com/studio)

Additionally if you would like to install the .apk files (app installation files) that you create without re-opening Unity, you can install
[SideQuest](https://sidequestvr.com/), which is an application that allows you to sideload applications created by other users (or yourself)
onto your Quest 2. This is the preferred method if you are destributing your application with .apk files.

========
# Android Studio
For android studio, you'll simply need to install an Android SDK that is compatible with the Quest 2. This should be Android 10.

========
# Unity
There are numerous items and features you'll have to enable within Unity to begin developing for the Quest 2.

Before getting started, it is recommend you create a new branch (or entirely new repo) containing your project, as
you'll be making significant changes that cannot (and should not) be merged into main.

1. Go to the Package Manager Settings and go to "Advanced Settings"
2. Enable Preview Packages.
3. Open the Package Manager and install the following packages, if not installed already:
    * XR Interaction Tookit
    * XR Plug-in Management.
    * (Optional) Oculus Assets - also available in the Unity Asset store.
4. Go to the XR Plug-in Management settings within Project Settings.
5. Switch to the Android tab, and select "Oculus" as your only plug-in provider.
6. In Player Settings (also within Project Settings), switch to the Android tab and scroll down to the "Identification" section.
7. Set the Minimum API level to at least Android 7.0.
8. In the Build Settings, ensure that you are switched to the Android platform.
9. Set Texture Compression to "ASTC".
10. Plug in your Quest 2, and ensure it is on (and USB communication is turned on).

At this point, you will be given the option to Build, or Build and Run your application. However, if your project is still utilizing the ValveVR Interaction system
as a means of interaction, the build will fail. At this point, you can begin working to convert code to the Quest 2's means of interaction (XR Origin).