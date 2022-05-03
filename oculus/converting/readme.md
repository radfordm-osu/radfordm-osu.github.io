Oculus Documentation - Converting Code to XR Origin
========

Overall, converting project based on the SteamVR and ValveVR interaction system is not an easy one.
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
- Converting Development Team code to XR Equivalent

# Resources
Below are some helpful resources to get you started.

* [SharkJets](https://www.youtube.com/c/SharkJets/featured) a YouTube channel containing lots of Quest 2 development videos (contains some paid solutions).

# Replacing PlayerVR
Details to come.

# Removing Teleportation Plane
While most of our assets can remain in our scenes, one exception is the teleportation plane provided by SteamVR.
If this is left in, your project will build, but a large missing texture will be visible (a large purple plane).

To begin converting to the XR equivalent:
1. Remove the SteamVR teleportation plane.
2. Add in an XR Teleportation Area.
3. Add a XR TeleportationProvider and Locomotion System to your XR Origin/XR Rig

# Removing ValveVR interactible scripts - Free Equivalent
To convert to Quest 2, you will need to convert any interactible scripts tied to your objects to 'XR Grab Interactible. To do so:
1. Remove Interactible and Throwable Scripts
2. Add Component -> XR Grab Interactible

# Converting Development Team code to XR Equivalent
Details to come...

