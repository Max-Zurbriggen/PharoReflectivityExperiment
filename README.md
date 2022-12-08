# PharoDebugPoints

  ```Smalltalk
Metacello new
  repository: 'github://Max-Zurbriggen/PharoDebugPoints';
    baseline: 'PharoDebugPoints';
      load.
```

# Guide

## Placement

All debug points can be placed like with previous breakpoints by right-clicking on an expression in the code editor.
(NOTE: only the submenu “Debug Points” is new, all other debugging features are already part of the image)

![Menu](/pictures/debugPointMenuV2.png)

## Debug Point Types
- Breakpoint: 	Break when the node is reached
- Script: 		Execute a script when the node is reached
- Transcript:	Write something to transcript when the node is reached
- Watch: 		Saves the values of the node in a history

## Debug Point Behaviors
Behaviors can be added to all types of debug points in the manager.
- Condition:	The debug point is only executed when the condition returns true.
- Once:		The debug point is deactivated after being executed.
- Count: 	Count how often a debug point is executed.
- Chain:  When the parent debug point is executed it activates the child debug point while deactivating itself. A debug point can be added as a child by drag and dropping it on the desired parent in the debug point manager in the list on the left side.

## Managing Debug Points
You can manage debug points in the manager or when hovering over the icon in the code editor:

![Menu](/pictures/worldMenu.png)
![Menu](/pictures/iconHoverOptions.png)

The manager should be mostly self-explanatory, a debug point can be selected on the left side and edited on the right side:

![Menu](/pictures/managerWithChain.png)

## Object Centric Debug Points

When inspecting an object, you can set the scope of an already existing debug point to this specific object:

![Menu](/pictures/scopeButton.png)
