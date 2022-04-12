# Laser Pointers

Laser pointers enable a user to click a button by pointing their hand at it and pressing the trigger button.

The functionality of laser pointers was implemented using the 'SteamVR_LaserPointer' script from the ValveVR library. This is combined with an interactable button script and a highlight script (also from ValveVR) to create buttons that respond to the laser pointers.

These buttons are used in all of the menus so that a user does not need to be close to them to use them.

### Laser Pointer Buttons
These buttons have the following hierarchy:

- UI Button with 'UI Element' and 'Interactable' scripts
  - Text
  - Invisible box collider (hitbox)
    - Highlight prefab
