# Pause Menu

The pause menu works almost the same as the [Main Menu](/valvevr/ui/main-menu). The main difference is that the pause menu does not have a scenario selection but instead has the option to return to the main menu. The pause menu may be opened by pressing 'Y' on an oculus controller in any scenario.

## Public Methods
###SpawnMenu():
Makes the pause menu visible and enables laser pointers.

###DeleteMenu():
Hides the pause menu and disables laser pointers.

###ReturnToMain():
Closes the scene and opens the main menu. More on this [here](/valvevr/ui/main-menu).

### OpenMainMenu:
Displays the default pause menu. Called when returning to the pause menu.

### OpenOptionsMenu():
Opens the settings menu. Called when opening the settings menu. More on this [here](/valvevr/ui/settings).

### EnablePointers():
Enables laser pointers when the scene is started. More on this [here](/valvevr/ui/laser-pointers).
