# Prompt: 3D t-SNE Explorer (Part 3)
version: v1
status: experimental
model: gemini

## Purpose
Add an Alternative Layouts to the experimental Interactive Data  Visualisation 3D t-SNE Explorer

## Prompt 1
Add a new Toggle UI menu with options for “T-SNE” and “Cluster”.
The “T-SNE” Option should activate the current node layout, this T-SNE layout should be remembered for later display.
Selecting the “Cluster” option should activate an alternative network display layout, as specified by:
•	Move all the nodes associated with each cluster to one of the sides of the display cube, keeping the connections between the nodes and maintain the Force-Directed Graph Layout as a cluster (not a uniform layout), position any connections between cluster on the inside of the cube. move the outliers to the unused cube side.
•	The UI toggle should support switching between the “T-SNE” projection mode view and new “Cluster” mode view.

## Prompt 2
As the application switches between the “T-SNE” view and the “Cluster” view, please animate the movement of each of the nodes between layout modes, such that the nodes move from the “T-SNE” layout to the “Cluster” layout, also maintain the node connections as the nodes move from one position to the next, such that the edges will stretch and contract as the nodes move. .
Do not change the current dataset, and do not change any other functionality.

## Prompt 3
Ok, now I would like to add an additional Layout mode choice called “Flat”. In Flat mode move all the nodes of each cluster should move to be projected onto a series of 2D planes, keep the connections between the nodes and maintain the Force-Directed Graph Layout as a cluster (not a uniform layout).
Do not change the current dataset and do not change any other functionality.

## Prompt 4
With the addition of the display modes the application and overall browser interactions have become very sluggish. Please review all the code and identify options to improve performance and responsiveness
