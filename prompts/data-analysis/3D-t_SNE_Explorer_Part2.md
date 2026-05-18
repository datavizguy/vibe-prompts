# Prompt: 3D t-SNE Explorer (Part 2) - Persona Use Case
version: v2
status: experimental
model: gemini

## Purpose
Add a Persona Use Case to the experimental Interactive Data  Visualisation 3D t-SNE Explorer. 

## Prompt 1
Please re-label all the notes and clusters (including the legend) to align with fictitious organisational communication patterns. For example: Boss (Network Leader), Lieutenant (Second-in-command), Enforcer (Operative), Money Mule (Financial Agent), Broker (Facilitator), Outlier (Unknown Actor). This will support analysis of financial transactions and other data to identify and disrupt criminal networks. 

## Prompt 2
Centrality Measures: Quantify the importance or influence of each node within the network (e.g., degree centrality, betweenness centrality), and add the top 4 scoring nodes to a separate section of the Legend and make those items on the legend selectable, like the clusters and nodes.

## Prompt 3
Include the Centrality Measures in both the Popup Tooltip and the CSV download. Do not change any other functionality.
