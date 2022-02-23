# ValveVR Documentation

VRWTS was originally designed for ValveVR. This version may be more stable and complete than the Oculus version.

<hr>
## Modules
<hr>
### Task System
The task system consists of a **[Task Watcher](/valvevr/tasks/task-watcher)** and **[Task Objects](/valvevr/tasks/task-objects)**.
Simply put, the **Task Watcher** initializes and counts the **Task Objects**.<br />
The **Task Objects** wait for a signal from their target before signaling task completion to the **Task Watcher**.<br />
More about these on the [tasks page](/valvevr/tasks).

<hr>
### Hazard System
The hazards system currently only contains a basic area and a hands area.<br />
More about these on the [hazards page](/valvevr/hazards).

<hr>
### User Interfaces
The UI system has many parts to it. This deals with scene selection, options, pausing, and laser pointers. This system is heavily reliant on the task system (and vice versa).<br />
More about this on the [user interfaces page](/valvevr/ui).

<hr>
### [Interactables](/valvevr/interactables)
There are currently only a few interactable objects, but the purpose of this project was to lay the groundwork for future expansion.<br />
More about interactables on the [interactables page](/valvevr/interactables).

<hr>
### Old Projects
This project re-used and updated assets from older project solutions. You can find the orignal projects from past years below.
- [VR Factory (2020)](https://github.com/jlouis2k4/VR-Construction-Training-System)
