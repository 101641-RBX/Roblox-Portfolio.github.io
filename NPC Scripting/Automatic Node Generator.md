# Scripting Overview

## Description
This script generates parts called "Nodes" that will be placed at fixed intervals on top of the main part. To prevent endless generation of the nodes, cutoffs are generated at the corners and front/back of the main part, which when reached will force the script to start generating further down the main part. **This works for all part sizes, as well as all rotation.**

## Why Use Nodes?
- **More Control:** Allows for you to manually set where the NPC should move to, allowing you to forcefully randomize pathfinding which can make NPCs less predictable.
- **More Gameplay Opportunities**: Since nodes are physical parts, you can access more properties and use them to help influence NPC behavior. Some examples are:
  - Raycasting from a node to enemey, to see if the node is behind cover or not
  - Get all possible nodes in a region, and have NPCs pick a random node based off the region (helps with optimization)
  - Can delete nodes that are inside other parts, guaranteeing that the NPC will never move to that node


## Video Demonstration

### Node Generating

https://github.com/user-attachments/assets/0b060d7c-e629-4db0-96a4-0492c318122b

*Video Example of the node spawning and how it can be used for any shape and rotation. Note that having multiple of these run at once will increase script activity, but the script will terminate itself once completed. This is ok as this script is suppose to run upon server startup where everything is loading in*


### NPC Pathfinding with Nodes
https://github.com/user-attachments/assets/0ab63a68-fbfb-41cb-b00b-15574cf6ebb1

*Vide Example showing how basic NPC pathfinding can work with nodes*

## Code Snippets and Explanation






