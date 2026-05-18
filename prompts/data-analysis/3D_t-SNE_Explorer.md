## Prompt: 3D t-SNE Explorer 
version: v2
status: experimental
model: gemini

## Purpose
Create an experimental Interactive Data  Visualisation 3D t-SNE Explorer

## Prompt 1
Task: I would like to create a simple interactive 3D data visualisation inspired by a t-SNE projection, where the x, y, z coordinates of each node in the visual are generated as part of a sample dataset as specified below.
Dataset Requirements:  Please generate a sample dataset with 500 data points, each with the following properties:
•	x: Number representing the first t-SNE dimension (range approximately -50 to +50).
•	y: Number representing the second t-SNE dimension (range approximately -50 to +50).
•	z: Number representing the third t-SNE dimension (range approximately -50 to +50).
•	label: Category assigned to the data point that represents clusters (randomly assigned from 5 categories: A, B, C, D, E).
•	id: Unique identifier for each data point.
•	Each node should be connected to 3–7 nearby nodes (based on 3D Euclidean proximity). Where each edge includes a source_id and target_id. Edges should be undirected and no duplicates.
•	Please add a small number of random edge connections between the clusters in the dataset. 
•	Add 5 randomly located nodes, outside the main clusters but still with the overall x, y, z range, and connect those nodes by edges to their nearest nodes.
Visualisation Requirements: Display the dataset as an interactive 3D cube scatter plot, where:
•	Each data point is shown as a small colored sphere or dot.
•	Use distinct colours for each category label (A–E).
•	Render the data within a cube-shaped bounding box.
•	Allow freeform 3D rotation of the cube on all three axes (X, Y, Z), using the Drag behaviour.
•	Enable zoom in/out functionality, using the mouse scroll or pinch gesture.
•	Include tooltips or small popups that show the id and label when hovering over each point.
Technology: The application should have the following properties:
•	Use a performant and smooth 3D rendering library such as three.js or Plotly.js (3D scatter), depending on the best compatibility with Vibe.
•	Ensure the overall experience is smooth, clean, and suitable for exploratory data analysis and presentation.
•	Apply an "Immersive UI" design theme to the app, and set the application with a light background. 
•	Include a selectable toggle between dark mode and light mode, and provide an option to hide the node colour legend.

## Prompt 2
Please make the edges of the network the same colour as the related cluster and make the edges slightly thicker to improve visibility.
Add a hover action on all nodes that causes the display of a Tooltip type display showing the attributes of the selected node.
Do not change any other functionality

## Prompt 3
Please modify the cluster legend so that if the user clicks on a cluster, only the nodes and edges in that cluster are highlighted, and all other nodes and edges are displayed as bright grey (#E8E9E8) with a transparency of 50%.
Do not change any other functionality

## Prompt 4

When a user clicks on a node, please highlight that node and all the related nodes for three degrees of connection, and the edges between the highlighted nodes. All other nodes and edges should display as bright grey (#E8E9E8) with a transparency of 50%.  Please add an animation that pulsates the selected node to 50% bigger and back continuously, then return it to its normal state when it is deselected
Also enabling a toggle behaviour for node selection, such that:
•	Click a node: Highlights it and all nodes within three degrees of connection.
•	Click the same node again: Clears the selection and returns to the default view.
•	Click anywhere else: The onPointerMissed handler clears the selection as well if the user clicks anywhere else inside or outside the cube area.

## Prompt 5
Please add a button that provides a CSV Download of the node and edge details of the currently highlighted nodes and edges.

