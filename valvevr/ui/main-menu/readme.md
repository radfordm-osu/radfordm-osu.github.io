# Main Menu

The main menu is where a user chooses which scenario to open. Users may also change settings or close the application from this menu. All of the main menu functionality (except for buttons) is done in MainMenuCanvas.


## Adding Scenes to the Menu
For a scene to be visible from the main menu, the following steps must be taken:

1- Create a folder for the scene in Assets/Scenes/Resources/

2- Open the scene and then open Build Settings. Press 'Add Open Scenes' to add the scene to the list. This only needs to be done once per scene.

Optional - To give the scene an icon in the main menu, add a PNG image named 'icon' to the scene folder created in step 1. In the inspector, change the TEXTURE TYPE field to 'Sprite (2D and UI)' then select 'Apply'.

Once these steps are completed, the scene will automatically be added to the scenarios list when the application is run.

## Public Methods
### NextPage():
Displays the next scenarios on the menu (up to 3). If the last page is currently shown, it loads the first page. Called on the pressing of the down arrow in the scenes menu.

### LastPage():
Displays the last scenarios on the menu (up to 3). If the first page is currently shown, it loads the last page. Called on the pressing of the up arrow in the scenes menu.

### OpenScene(string scene_name):
Opens the scene with the given name. Called on the pressing of the play button on a scene.

### OpenScenesMenu():
Displays the scenario selection menu. Called when the scenarios button is pressed.

### OpenMainMenu():
Displays the default main menu. Called when returning to the main menu.

### OpenOptionsMenu():
Opens the settings menu. Called when opening the settings menu. More on this [here](/valvevr/ui/settings).

### EnablePointers():
Enables laser pointers when the scene is started. More on this [here](/valvevr/ui/laser-pointers).
