# Prompt: 3D t-SNE Explorer (Part 3) - Add Layouts
version: v2
status: experimental
model: gemini

## Purpose
Add Alternative Layouts to the experimental Interactive Data Visualisation 3D t-SNE Explorer

## Prompt 1
Add a new Toggle UI menu with options for “T-SNE” and “Cube”.
The “T-SNE” Option should activate the current node layout, this T-SNE layout should be remembered for later display.
Selecting the “Cube” option should activate an alternative network display layout, as specified by:
•	Move all the nodes associated with each cluster to one of the sides of the display 3D cube, keeping the connections between the nodes and maintaining the Force-Directed Graph Layout as a cluster (not a uniform layout). •	Position any connections between clusters on the inside of the cube, and move the outlier nodes to the unused cube side.
•	The UI toggle should support switching between the “T-SNE” projection mode view and new “Cube” mode view.

## Prompt 2
As the application switches between the “T-SNE” view and the “Cube” view, please animate the movement of each of the nodes between layout modes, such that the nodes move from the “T-SNE” layout to the “Cube” layout, also maintain the node connections as the nodes move from one position to the next, such that the edges will stretch and contract as the nodes move. In the "Cube" layout view, please distribute the nodes across the full side of the cube that they have been projected onto. Please maintain the relative position of each node to each other, simply spread the node out.
Do not change the current dataset, and do not change any other functionality.

## Prompt 3
Ok, now I would like to add an additional Layout mode choice called “Flat”. In Flat mode move all the nodes of each cluster should move to be projected onto a series of 2D planes, keep the connections between the nodes and maintain the Force-Directed Graph Layout as a cluster (not a uniform layout).
Do not change the current dataset and do not change any other functionality. 

## Prompt 4
Ok, now I would like to add an additional Layout mode choice called “Sphere”. In sphere mode move all the nodes of each cluster should move to be projected onto a 3D sphere, keep the connections between the nodes and maintain the Force-Directed Graph Layout as a cluster (not a uniform layout).
Do not change the current dataset and do not change any other functionality.

## Prompt 5 (Performance)
With the addition of the display modes, the application and overall browser interactions have become very sluggish. Please review all the code and identify options to improve performance and responsiveness
