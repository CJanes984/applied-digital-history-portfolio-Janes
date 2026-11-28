Part 1. Understand the source table 
one letter for which the original text survives; Letter ID: L0040, Sender Name: Johannes Hartmann, Survival Status: text_surviving
one record with an uncertain date; Letter ID: L0029, Sender Name: Elisabeth Reuchlin, Survival Status: text_surviving
one letter involving the unidentified correspondent; Letter ID: L0301, Sender Name: Anna Keller, Survival Status: text_surviving
a pair of people for whom letters are recorded in both directions. Letter ID’s: L0008 and L0009, Sender Names: Anna Keller and Matthias Vogler, Survival Statuses: text_surviving and text_surviving.
Checkpoint 1: Explain what one row represents. Explain why 304 rows do not demonstrate that only 304 letters were historically exchanged among these people.
One row represents a processed letter. There are only 304 rows because not every letter produced by each of the individual senders was saved. Many of the letters each of these people created may have been destroyed or lost. 

Part 2. Define the network model
Checkpoint 2: In your notebook, state what a node, edge, and weight represent. Explain why the data preserves direction even though the first analysis will temporarily ignore it.
A node is the main identifier for one person. It maintains a small number of categories within it, including but not limited to ID, Label, Gender, and City. An edge is a representation of all catalogued letters sent by one person to another. Weight simply represents the count of records that have the same recipient and sender. Five letters from a fictional Jake to Julie would have a weight of 5, but if Julie had only sent 3 letters to Jake, the respective weight of those letters would be 3. The data preserves direction because the order in which the sending and receiving IDs are entered maintains the same sending -> receiving path. The data is organized so that the sender ID always comes before the receiver ID. This ensures that the data will be accurately read.

Part 3. Create the notebook and inspect the data
Checkpoint 3: The notebook has inspected the unmodified source table and found 304 unique letter records involving 41 distinct person identifiers.
√

Part 4. Generate and validate the node table
Checkpoint 4: correspondence_nodes.csv contains 41 unique people, including the unidentified correspondent.
√

Part 5. Generate and validate the edge table
the edge with the largest weight: P001 -> P002
an edge with Weight = 1: P036 -> P016
one direction of a reciprocal pair: P001 -> P002, weight 8. P002 -> P001, weight 4
Checkpoint 5: correspondence_edges.csv contains 82 unique directed pairs whose weights sum to all 304 source records. Three selected weights have been checked against the original letters.
√

Part 6. Create a GEXF network file
Checkpoint 6: All three files have been saved to your repository.
√

Part 7. Open and inspect the network in Gephi Lite
Checkpoint 7: Gephi Lite contains the same 41 nodes and 82 edges as the validated Python tables.
√

Part 8. Apply and compare layouts
Before changing the layout, export or capture an image (screenshot) of the initial network. Record whether the initial arrangement makes any structure easy to interpret.
The graph is somewhat readable, though it is messy and can be confusing or hard to follow.
Generated Values:
Gravity: 0.05
Scaling ratio: 10
Slow down: 4.713572066704308
Strong gravity mode: selected
Final Values:
Gravity: 0.01
Scaling ratio: 30
Slow down: 4.713572066704308
Strong gravity mode: selected
Keep labels hidden or small while adjusting the layout, then restore selected labels after the positions are stable. Note one cluster or intermediary node that becomes easier to see.
Node P038 -> P037 became easier to see.
the initial crowded graph; 
 ForceAtlas2 using Gephi Lite's generated settings;

the final version after increasing the scaling ratio and sizing nodes by degree. 
In your notes, identify one feature that became clearer and one impression that may result from the layout settings rather than the historical evidence.
The weight of the records became instantly distinguishable. Though knowing which records have the largest weight can be difficult. The impression that this graph may wrongfully promote is that one could perceive the larger nodes as important and disregard the smaller nodes.
Checkpoint 8: You used the generated ForceAtlas2 settings, adjusted the scaling ratio if necessary, sized nodes by degree, recorded the final values, and can explain why node position and node size represent different things.
√

Part 9. Encode attributes through appearance
Color is based on city.
Checkpoint 9: Node size represents degree, node color represents either city or gender, edge size represents weight, node labels show names, and edge labels show letter counts.
√

Part 10. Filter the network
Checkpoint 10: You exported full, degree-filtered, and ego-network views and compared ego-network depth and direction settings.
√

Part 11. Calculate and translate network metrics
*degree centrality = number of connected neighbors ÷ maximum possible neighbors*
*5 connected correspondents ÷ 40 possible correspondents = 0.125*
Then write a short paragraph identifying the strongest direct and intermediary positions, followed by one limitation and one claim that would require checking the letters.
The strongest direct and intermediary positions relate to Sabina Lorenz. One limitation is that not every cell is filled with guaranteed data, so the data could be misleading or overlooked. One claim that would require checking the letters would be to prove that the writers are the true writers. I am not sure exactly how one could do this, but looking into the signatures of the letters could indicate that a writer may not have been the true writer of these letters.
Checkpoint 11: You calculated the network summary and four centrality measures, used an LLM to translate rather than replace your interpretation, checked the translation against the tables, and wrote your own evidence-conscious summary.
√

Part 12. What changes when direction matters?
Three distinct senders have the most incoming volume. P028, P031, and P037. Seven rows have the same outgoing amount. The direction of sending depicts asymmetrical paths. The direction and size could be misleading because the letters that were lost may have amounted to large changes.
Checkpoint 12: You calculated the directed measures, used an LLM to translate them into accessible prose, checked its explanation, and can distinguish degree, in-degree, out-degree, reciprocity, weak connectivity, and strong connectivity.
√

Part 13. Check one edge against the letter records
Records: The catalogue contains seven letter records sent from Johannes Hartmann to Georg Auer.
Network: These records appear as one directed edge with weight eight.
Records: The catalogue contains six letter records sent from Georg Auer to Nikolaus Eber.
Network: These records appear as one directed edge with weight six.
Checkpoint 13: One edge weight matches its underlying letter records, and its limitation has been stated.
√

Part 14. Save and export the Gephi Lite project
√

Part 15. Interpret the network historically
This data graph implies that the most contacted people were Magdalena Frisch, Sabina Lorenz, and Sebastian Walther. Most likely these individuals played an important hand in the situations that they were tasked with. There are typically three individuals being contacted per country. There was widespread communication between these individuals even though they may have been quite a long distance from one another. It would be extremely helpful to have either physical access to these documents or to have digital scans to inspect.
