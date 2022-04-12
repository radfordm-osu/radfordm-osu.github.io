#Task Watcher
The task watcher is used to keep track of the tasks that are incomplete. When a scene loads, the task watcher will find all objects with script classes that extend Task.cs. For each task object it finds, it puts them into a list. If the tasks are ordered, only the first one in the list will be activated on start.

**Note: A scene should only have ONE task watcher.**

##Ordering Tasks
Tasks may be set to the order that they appear in the environment hierarchy or be unordered. This can be toggled with the Execute_Tasks_In_Order flag.

##Performance Ratings
A scene may also have performance ratings at the end based on the time it took to complete all tasks. These ranges can be set in the task watcher. The Use_Times flag must be set in the task watcher for these to work.
