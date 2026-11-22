Checkpoint 1: In your notes, explain the difference between place, place_norm, and place_interpreted. Classify Roma (=Basel) using one of the proposed place_relationship values and explain your decision.
The ‘place’ value is the original field that was documented. It holds a range of values that indicate where the book was published. The ‘place_norm’ column is an updated list based on the value of ‘place’. This column refines the existing data into more uniform and standard fields. Rather than having a column filled with several different input styles, it creates a uniform list that can be easily read by a machine. The ‘place_interpreted’ column represents the geographic location selected for the record. The input data, Roma (=Basel), indicates that the book was inaccurately described as being published in Rome, but was truly created in Basel. The ‘place_relationship’ would be set as ‘false_imprint_attributed_to’ because the book wasn’t truly made in Rome.

Step 1: √

Step 2:
•	Non-empty place strings: 31
•	One Straightforward Value: Köln
•	One Bracketed Value: [Basel]
•	One Malformed Value: Basel]
•	One Value Containing An Attributed Alternative Place: Erfurt (=Homberg)
Checkpoint 2: OpenRefine contains 500 rows and approximately 31 distinct non-empty place strings. If your totals differ, inspect the import settings and blank values before continuing.
√

Step 3:
•	One Accepted Normalization: Tübingen]  Tübingen
•	One Proposed Normalization Rejected: Buyten Strasbourg (=Emden)
•	One Requiring Historical Interpretation, Not String Cleaning: Basel (Genève
I struggled to find an easy way to clear the column when creating a column in OpenRefine. After guessing and trying value.clear(), I got a pop-up notification saying the argument was invalid. After trying to find a manual that could teach me how to easily add a new column, I gave up and tried another guess. After inputting value.empty I noticed that all the rows stated they were ‘null’. This input worked and emptied the rows in this column. Then I actually continued reading and saw that the solution was already input in the tutorial, and all I had to do was type null. This was awkward.

Checkpoint 3: The original place column is unchanged. You have separate place_norm and place_interpreted columns, and at least three documented decisions.
√

Step 4:
Checkpoint 4: Every distinct place has been reviewed. At least one candidate decision is documented, and ambiguous or unmatched cases have not been silently discarded.
√

Step 5:
Checkpoint 5: Your exported CSV contains all original columns, place_norm, place_interpreted, match_status, wikidata_id, and coordinate information. The original CSV remains unchanged.
√

Step 6: √

Step 7:
The Colab session wouldn’t allow me to upload my file through the prompt. Therefore manually uploading the data was the only simple solution I was able to come to. 

Checkpoint 6: The notebook reports 500 input rows and 500 unique edition_id values. You have inspected the actual coordinate representation.
√

Step 8:
Checkpoint 7: The row count and edition identifiers are unchanged. Invalid or missing coordinates are reported rather than silently deleted, and at least a few representative cases have been checked. 
√

Step 9:
Checkpoint 8: You can explain what one row represents in the original table and what one row represents in the aggregated table.
√

Step 10:
Choose at least five markers and compare their displayed counts with printing_places_aggregated.csv. Include the largest place and at least one place with a small count.
1)	Basel: 135 Editions √
2)	Antwerp: 1 Edition √
3)	Strasbourg: 56 Editions √
4)	Regensburg: 1 Edition √
5)	Augsburg: 37 Editions √

Checkpoint 9: The interactive map opens, marker counts match the aggregated CSV, and marker area—not radius—is intended to represent the count.
√

Step 11:
The map indicates that most of the books processed were in Central Europe. If the texts that were processed represent all the available data, it demonstrates that most of the publication of texts was in Central Europe. The amount of data sets declines drastically as the map moves from west to east. Basel was almost certainly a controlling factor during this time because it is credited with producing 135 of the documented editions.

