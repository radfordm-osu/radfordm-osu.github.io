# ValveVR Documentation

VRWTS was originally designed for ValveVR. This version may be more stable and complete than the Oculus version.

***
## Modules
***
### Task System
The task system consists of a **[Task Watcher](/valvevr/tasks/task-watcher)** and **[Task Objects](/valvevr/tasks/task-objects)**.
Simply put, the **Task Watcher** initializes and counts the **Task Objects**.
The **Task Objects** wait for a signal from their target before signaling task completion to the **Task Watcher**.
More about these on the [tasks page](/valvevr/tasks).
***
### Hazard System
The hazards system currently only contains a basic area and a hands area. More about these on the [hazards page](/valvevr/hazards).
***
### User Interfaces
The UI system has many parts to it. This deals with scene selection, options, pausing, and laser pointers. This system is heavily reliant on the task system (and vice versa).
More about this on the [user interfaces page](/valvevr/ui).
***
### [Interactables](/valvevr/interactables)
There are currently only a few interactable objects, but the purpose of this project was to lay the groundwork for future expansion.
More about interactables on the [interactables page](/valvevr/interactables).
***
### Old Projects
This project re-used and updated assets from older project solutions. You can find the orignal projects from past years below.
1) [VR Factory (2020)](https://github.com/jlouis2k4/VR-Construction-Training-System)
