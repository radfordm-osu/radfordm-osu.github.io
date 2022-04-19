Oculus Documentation - Converting Code to XR Origin
========

# Resources
Below are some helpful resources to get you started.

* [SharkJets](https://www.youtube.com/c/SharkJets/featured) a YouTube channel containg lots of Quest 2 development videos.

# Removing Teleportation Plane
While most of our assets can remain in our scenes, one exception is the teleportation plane provided by SteamVR.
If this is left in, your project will build, but a large missing texture will be visible (a large purple plane).

To begin converting to the XR equivalent:
1. Remove the SteamVR teleportation plane.
2. Add in an XR Teleportation Area.
3. Add a XR TeleportationProvider and Locomotion System to your XR Origin/XR Rig

# Removing ValveVR interactible scripts
To convert to Quest 2, you will need to convert any interactible scripts tied to your objects to 'XR Grab Interactible. To do so:
1. Remove Interactible and Throwable Scripts
2. Add Component -> XR Grab Interactible