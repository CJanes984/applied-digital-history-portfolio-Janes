What material did I work with?
I worked with OpenRefine. A data cleaning tool that helps to organize similar datapoints that are seperated due to small typographical differences.

What transformation did the tool perform?
The tool was used to fix minor typographical errors made when inputting data. The tool was able to do so by duplicating a column of data. 
Inputting given expressions would trim spaces or give the certainty of a data value. We also were able to use facets to easily visualize the number of data types that appear in the column.
Then we used the cluster feature to easily mass transfer data types to the correct values. Using the reconcile ability we were able to match location names to real world locations via Wikidata.

What decisisions did I make?
I decided whether a data type was a simple typographical error or if the data was referring to different concepts, i.e., A. ABOTT and A. Abott, most likely refer to the same person. 
Though without proof it is a risk to assess them as the same and consider it a simple error.

What failed, remained unclear, or produced an unexpected result?
I struggled to discern which column represented the historical object, which were suitable for a controlled vocabulary, and which described its archival/digital representation.

What does the output allow me to infer historically?
The output data after being put into RawGraphs displays a gap in records dates between 1900 to roughly 1903. 

What does the output allow me to infer?
The output allows me to more easily inspect and use data to assess gaps, missing data, or issues regarding the recording or documentation of the data.

Could this method contribute to my final project? Why or why not?
This could be used for my final project to help sort data that is similar but has minor text differences.

**Notes**

Part: 3
1. What does one row represent?
		One row represents an individual historical photograph.
2. Which columns describe the historical object?
		title_raw, subject_raw, creator_raw, date_raw, place_raw, object_type_raw, caption_language_raw, country_raw, notes_raw
3. Which columns describe its archival or digital representation?
		record_id, rights_raw, holding_institution_raw, box_folder_raw, filename_raw, 
4. Which columns appear suitable for a controlled vocabulary?
		holding_institution_raw, object_type_raw, caption_language_raw, subject_raw, country_raw
5. Which columns contain uncertainty that should not simply be deleted?
		date_raw, notes_raw, country_raw

Part: 4
Record two examples for each category:
* A difference that is probably typographical;
    * rights_raw, row 47: CCBY4
    * object_type_raw 62: photo;print
    * Denmark & Danmark: rows 28 & 78 are listed as country_raw -> Danmark
    * photograph & Photograph: appears a multitude of times in object_type_raw
* A difference that probably represents two labels for the same concept;
    * U.S. and United States in country_raw
    * Ger. and Germany in country_raw
* A difference that should not be resolved without more evidence.
    * Public Domain & Public domain? -> Changing the label on row 27 without knowing if it’s truly public domain would be bad.
    * What does UNK stand for in row 64? 

Part: 6
In your notes, record:
* Merged photo;print and photo print, merged photo and photograph
* The preferred value I selected was photograph and photo print
* I believe that merging photo and photograph is fine, but merging photo print with photograph gets rid of important distinctions between the two different photo types.

Part: 7
For every proposed cluster, ask:
1. Are these strings only typographical variants?
	Yes, every string is simply a typographical variant, other than B. Abbott.
2. Could they refer to different people?
	Most are pretty set referring to one person, but B. Abbott and B. ABBOTT could refer to two people, and so could Brassaï.
3. Is an initial sufficient evidence of identity?
	No, an initial is a good indicator, but you should find more evidence before merging the cells.
4. Which form should be retained, and why?
	Keeping the form of last name, first name should be retained because it is a professionally organized way of sorting names.

In your notes, record at least one cluster you rejected or left unresolved. Explain what additional evidence would be needed to merge it responsibly.
* I left B. Abbott unmerged because I cannot be sure that B. Abbott and B. ABBOTT are the same person.

Part: 8
Record the mapping in your notes:
Manually merged Wien, Vienne, and Vienna into Vienna.

Part: 9
Row 89: n.d. is considered exact, but I believe it should be uncertain.

Part: 10
When would a separate subject table be preferable to storing several subjects in one cell?
It would be preferable to separate the subject table in cases where you need to easily sort a record by a single piece of information in a cell.

Part: 11
Choose two duplicate candidates and record:
* the evidence suggesting duplication;
PHO-094 and PHO-073 -> These two records have identical duplicate_key info, and the notes_raw info states that PHO-094 may be a duplicate.
* the evidence against treating them as identical;
The record_id values are different, but other than those cells, all values appear the same.
* your provisional decision;
These records are identical and can be merged.
* what additional source or metadata would help resolve the case.
Being able to see the photo document itself would distinguish whether or not the record is a duplicate.

Part: 13
There is no record of undoing the seperation of fields, the application warned that going forward with the operations I did would remove that previous operation.

Part: 15
The graph shows a clear gap in records between 1900-(~1903)

-Evidence

1. Identify two forms of inconsistency that were directly visible in facets.
Names being incorrectly recorded, in the column object_type_raw row 62 the words photo print was recorded as photo;print, this distinguished it from the rest of the values and was easily caught in facets. Also, names being written in different formats such as Vienne, Wien, and Vienna, which are all correct, but the inconsistency in the use of one name became visible using facets.

2. Identify one field in which a blank value, unknown, and an uncertain statement should not automatically be treated as equivalent.
A photographer was recorded as B. Abott while another was documented as B. ABOTT, while these names appear to reference the same person, it is impossible to know without having the individual’s full first name. 

-Inference

3. Give one example of two values you inferred referred to the same person, place, or category. What evidence supported the merge?
In the place_norm column, I inferred that méxico city and Mexico City referred to the same place. Therefore, I merged them.

4. Give one example you chose not to merge. What evidence was missing?
There were multiple different spellings of the name Brassaï, but I wasn’t sure whether I could merge them without knowing more about who the person/persons are.

-Interpretation

5. Explain one way that normalizing place, creator, date, or subject values could change a later historical analysis.
If the data has already been analysed by someone previously, it could disrupt their organization of the data. Also, if the values being changed shouldn’t have been altered, removing or merging some of the data types could hide important data that could’ve been utilized. 

6. Why might a count of normalized place names differ from a count based on the raw metadata?
The variation in place name values could separate the counted value because places like Vienna could be named in multiple ways, including Vienne or Wien.

-Limits and uncertainty

7. What information in the dataset would be lost if date_raw were replaced by a single year?
If the non-normalized field were overwritten, the date_certainty column would be inaccurate or unable to exist whatsoever. The approximations for years would also be lost.

8. Why are repeated filenames, titles, or composite keys evidence of possible duplication rather than proof?
Without having visible proof of duplication or other clear signs of duplication, these values could be inaccurate to the true piece they’re supposed to be representing
