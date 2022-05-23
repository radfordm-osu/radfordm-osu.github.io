Oculus Documentation - Converting Code to Oculus-compatible systems
========

Overall, converting a project based on the SteamVR and ValveVR interaction system is not an easy one.
In many cases, you will need to develop components from the ground-up, especially if you do not want to pay for assets or other interaction
systems.

Essentially, the main issue that arises while switching to an Oculus standalone app seems to come from references to SteamVR and ValveVR.

During build time for Android (the operating system that Oculus runs on), builds will typically fail if the selected scenes contained any scripts
that reference the ValveVR interaction system. Additionally, any textures pulled from SteamVR would fail to load properly into the scenes,
resulting in solid magenta colors.

Overall, the development can be broken up into a few main parts:
- Replacing the PlayerVR Prefab
- Replacing the Teleportation Plane
- Replacing ValveVR Interactible scripts
- Converting Development Team code to Interaction System of Choice

# Resources
Below are some helpful resources to get you started.

* [SharkJets](https://www.youtube.com/c/SharkJets/featured) a YouTube channel containing lots of Quest 2 development videos - Primarily uses VRIF, a $60 dollar interaction system.
* [Valem Tutorials](https://www.youtube.com/c/ValemTutorials/featured) a Youtube channel containing Quest 2 development using the OVR interaction system.
* [Oculus Documentation](https://developer.oculus.com/documentation/unity/unity-reference-scripting/) Documentation for the Oculus Integration Unity package.

# Replacing PlayerVR - XR Equivalent
To use the basic XR equivalent, it's fairly simple:

1. Remove the PlayerVR controller from the scene. If there are additional cameras that need to be controlled by a player (e.g. a flycam), they should be removed as well.
2. From the top of the screen go to "GameObject->XR->XR Origin (Action-based)" and add that object to the scene. Do not use the default "XR Origin" as that will not include controllers.

From here, you will be able to control this using the default "Ray-Interactor" System. This does not include hands, and thus does not use hands as an interaction system.
If you would like to add hands, you can visit [this](https://www.youtube.com/watch?v=DVAsL6sGmlc) video for manually adding hands.

# Removing Teleportation Plane - XR Equivalent
While most of our assets can remain in our scenes, one exception is the teleportation plane provided by SteamVR.
If this is left in, your project will build, but a large missing texture will be visible (a large purple plane).

To begin converting to the XR equivalent:
1. Remove the SteamVR teleportation plane.
2. Add in an XR Teleportation Area (GameObject->XR->Teleportation Area).
3. Add a XR TeleportationProvider and Locomotion System to your XR Origin/XR Rig within the scene.

# Removing ValveVR interactible scripts - XR Equivalent
To convert to Quest 2, you will need to convert any interactible scripts tied to your objects to 'XR Grab Interactible. To do so:
1. Remove Interactible and Throwable Scripts
2. Add Component -> XR Grab Interactible

# Converting Development Team code to Desired Equivalent
Converting development team code from any interaction system to another is not a simple process. Most likely you will have to recreate systems from the ground up. For this reason, it is highly recommended that you work on the Oculus version of your program at the same time as the rest of the group, ideally together.
