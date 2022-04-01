## Main Menu

The main menu is where a user chooses which scenario to open. Users may also change settings or close the application from this menu. All of the main menu functionality (except for buttons) is done in MainMenuCanvas.


## Adding Scenes to the Menu
For a scene to be visible from the main menu, the following steps must be taken:

1- Create a folder for the scene in Assets/Scenes/Resources/

2- Open the scene and then open Build Settings. Press 'Add Open Scenes' to add the scene to the list. This only needs to be done once per scene.

Optional - To give the scene an icon, add a PNG image named 'icon' to the scene folder created in step 1. In the inspector, change the TEXTURE TYPE field to 'Sprite (2D and UI)' then select 'Apply'.

## Public Methods
The public methods of MainMenuCanvas

### NextPage():
Displays the next scenarios on the menu (up to 3). If the last page is currently shown, it loads the first page.

### LastPage():
Displays the last scenarios on the menu (up to 3). If the first page is currently shown, it loads the last page.

### openScene(string scene_name):
Opens a the scene with the given name.

### OpenScenesMenu():
Displays the scnario selection menu

### OpenMainMenu:
Displays the default main Menu.

### OpenOptionsMenu():
Opens the settings menu. More on this [here](/valvevr/ui/settings).

### EnablePointers():
Enables laser pointers when the scene is started. More on these [here](/valvevr/ui/laser-pointers).
