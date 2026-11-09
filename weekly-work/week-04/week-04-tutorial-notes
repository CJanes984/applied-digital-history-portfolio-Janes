Checkpoint 1: In your own words, explain the difference between Python, a notebook, Colab, and an LLM.
•	Python is a scripting language with incredibly versatile uses. Python does not make decisions. Instead, the individual, or, in some cases, a computer generating the source code, makes the decisions. The Python script defines what happens to the CSV files. A notebook is a file or document that contains executable code, text, and output. The notebook gives an order to the work that shows small, inspectable steps. Google Colab is an online service that Google provides for Jupyter notebooks. It allows a user to run the notebook without having a local Python installation. An LLM is a giant mathematical codebase that generates text through hundreds of thousands of complicated mathematical operations to create text and plausible code. It can be used to help draft, explain, and revise code. It does not and should never be used as a replacement for a human’s review or correction. An LLM is simply a text generator, so it cannot execute its generated code within the interface.
The generated code failed on execution, so I took a break from the work. When I returned and tried to execute the code once more, it had lost the files, and I was unable to figure out how to get them back into Colab. So, I started a new project and restarted. After resetting, ChatGPT refused to take my prompt. Every time I’d try to send it through, it would reappear in my input box. I switched to Google Gemini, and it gave me no issues. The code generated properly and gave a correct output.
Checkpoint 3: Your notebook displays the expected dimensions and missing-value counts, and your text cell distinguishes file-level evidence from historical inference.
The output was exactly as it should be. No values were incorrect, and the code displayed everything correctly.
How can uncertain and ranged date statements be represented in separate, machine-readable fields without replacing the original evidence? 
Uncertain or ranged data statements can be represented in separate, machine-readable fields without replacing the original evidence by using a simple, organized list of data fields to represent the missing information. Something simple that indicates why something is missing or uncertain would work perfectly. Though certain distinctions would have to be coded to jump over or treated specially. Such as the values beginning with “c.”. 
Checkpoint 4: You have downloaded both CSV files, confirmed that the record-level file still has 100 rows, confirmed that the six aggregated counts sum to 100, and created the RAWGraphs bar chart from date_certainty_counts_for_rawgraphs.csv.
√
Checkpoint 5: Your chart has been validated against the aggregated table, its counts total 500, and its wording identifies the data as a teaching sample.
√
Part 10:
I struggled to open the html file as the desired output on my MacBook. Each time I’d try to open it the source code would simply be shown in the web browser. It took me roughly half an hour to find the simple solution to fix it. All I had to do was make the text in the text editor a plain text file rather than a rich text file. This worked and allowed the page to open correctly. Though uploading a file was not working, after prompting Google Gemini with the problem. It quickly gave me a solution and started working perfectly.
Part 11:
The same thing that occurred in part 10 happened in part 11 as well. The same fix occurred and the files worked perfectly afterward.

Part 12:
Create an interactive visualization:
I prompted Gemini to create an extremely simple html file that allows the user to search across all fields to find a data cell they’re looking for. This can be incredibly helpful if someone needs to find a piece of data, but doesn’t know what column it could be in.

Code Prompts for the AI:
step 1:
I am a digital humanities student with no previous Python experience working in [Google Colab]. Write one self-contained Python code cell using pandas to inspect a CSV named "book-sample.csv".

Each row represents one recorded edition in a teaching sample. The columns are: edition_id, short_title, author, printer, place, year, language, format, country, year_numeric, decade.

Here is a short excerpt from the beginning of the file:
[paste the first 5 rows here]

The code must:
1. load the CSV without changing it;
2. print the number of rows and columns;
3. display the first five rows;
4. print every column name and data type;
5. print the number and percentage of missing values in every column;
6. calculate minimum, median, mean, and maximum of year_numeric;
7. count records by decade, country, language, and format, including missing categories;
8. check whether edition_id is unique;
9. use clear labels so a beginner can interpret each output.
Do not drop, fill, or overwrite any values. After the code, explain it in plain language and identify what these statistics cannot establish historically.

step 7:
I am a digital humanities student with no previous Python experience working in [Google Colab]. Write one self-contained Python code cell using pandas and Python's standard re module to transform "historic_photographs_sample_dataset.csv" for later use in RAWGraphs.

Each input row represents one photograph metadata record. The input has 100 rows and these columns:
record_id, title_raw, creator_raw, date_raw, place_raw, country_raw, subject_raw, object_type_raw, caption_language_raw, holding_institution_raw, rights_raw, box_folder_raw, filename_raw, notes_raw, creator_authority_uri, place_wikidata_qid, lcsh_subjects.

Requirements:
- Preserve all original columns and all 100 rows.
- Do not overwrite, fill, or delete raw values.
- Add year_start: the first four-digit year in date_raw, stored as a nullable integer.
- Add year_end: the second four-digit year when present; otherwise use year_start, stored as a nullable integer.
- Add date_certainty using this explicit precedence: "uncertain" if date_raw contains ?, otherwise "approximate" if it begins with c. after trimming and lowercasing, otherwise "supplied/inferred" if it begins with [, otherwise "range" if it contains two four-digit years, otherwise "exact" if it contains one four-digit year, otherwise "unparsed".
- Add place_trimmed by removing leading and trailing whitespace from place_raw. Do not translate or otherwise standardize place names.
- Print input and output row counts, the number of unique record_id values, missing counts for every newly created column, and a table containing date_raw plus the three derived date columns for at least ten representative rows.
- Assert that the output has 100 rows, that record_id remains unique, and that no original column has been removed.
- Save the record-level transformed table as "photographs_for_rawgraphs.csv" with UTF-8 encoding and without a pandas index.
- Create a second DataFrame that groups the transformed records by date_certainty and counts the number of records in each category. It must have exactly two columns named date_certainty and record_count, with one row per date_certainty category. Include every category, including "unparsed".
- Print this aggregated table and assert that record_count sums to 100.
- Save the aggregated table as "date_certainty_counts_for_rawgraphs.csv" with UTF-8 encoding and without a pandas index.
- Do not use Google Drive mounting or any library other than pandas and Python's standard library.
After the code, explain every transformation, explain how aggregation changes the unit of observation, and identify cases that the rules might handle incorrectly.

If an error occurs with the AI code a simple prompting asking how to fix that will allow the AI to generate new code with the html errors corrected.

step 8:
I am a digital humanities student with no previous Python experience working in [Google Colab]. Write one self-contained Python code cell using pandas and matplotlib to create a bar chart from "book-sample.csv".

Each row represents one recorded edition in a selected teaching sample. Use the existing decade column to count rows by decade.

Requirements:
- Keep missing categories visible if any exist.
- Sort decade labels chronologically rather than alphabetically.
- Print the aggregated decade-and-count table before plotting it.
- Assert that the sum of all bar counts equals the number of input rows.
- Use an honest title that refers to "recorded editions in the teaching sample", not book production or readership.
- Label both axes and begin the numerical axis at zero.
- Make the chart legible but do not use a decorative style or 3D effects.
- Save it as "book-records-by-decade.png" at 300 dpi with a tight bounding box, then display it.
- Do not modify or overwrite the input CSV.

After the code, explain how the aggregation changes the unit of observation and why this chart cannot demonstrate total historical book production.

step 10:
I am a digital humanities student with no previous Python experience working in [Google Colab]. Write one self-contained Python code cell using pandas and matplotlib to create a bar chart from "book-sample.csv".

Each row represents one recorded edition in a selected teaching sample. Use the existing decade column to count rows by decade.

Requirements:
- Keep missing categories visible if any exist.
- Sort decade labels chronologically rather than alphabetically.
- Print the aggregated decade-and-count table before plotting it.
- Assert that the sum of all bar counts equals the number of input rows.
- Use an honest title that refers to "recorded editions in the teaching sample", not book production or readership.
- Label both axes and begin the numerical axis at zero.
- Make the chart legible but do not use a decorative style or 3D effects.
- Save it as "book-records-by-decade.png" at 300 dpi with a tight bounding box, then display it.
- Do not modify or overwrite the input CSV.

After the code, explain how the aggregation changes the unit of observation and why this chart cannot demonstrate total historical book production.

step 11:
Create one standalone HTML file that lets a user choose a local CSV file and then displays it as a searchable, filterable table. Design it for "historic_photographs_sample_dataset.csv".

Here is an excerpt of the first rows:
[paste first 5 rows]

Requirements:
- Use HTML, CSS, and vanilla JavaScript in one file.
- Do not require Python, a web server, npm, or a build step.
- Do not upload the CSV anywhere.
- Provide a keyword search across all displayed fields.
- Provide dropdown filters for country_raw and object_type_raw.
- Display the number of visible records and the total number of records.
- Allow sorting by clicking column headers.
- Preserve the original cell text; do not normalize values silently.
- Treat cell contents as text, not executable HTML, to reduce script-injection risk.
- Handle quoted commas and UTF-8 characters correctly.
- Show useful messages if the expected columns are absent.
- Make the table keyboard-accessible and usable on a narrow screen.
- Add comments and explain how to save, open, and test the file.

step 12:
I am a digital humanities student with no previous HTML experience.
Input: book-sample.csv. Each row represents one recorded edition in a teaching sample. The relevant columns are edition_id, short_title, author, printer, place, year, language, format, country, year_numeric, decade.
Requirements:
Use Python with pandas and matplotlib if needed.
Do not overwrite the input file or silently delete rows.
Preserve original values and put derived values in new columns.
Make missing values visible.
Print validation checks, including row counts and relevant missing-value counts.
Save the result as book-analysis-summary.csv, if applicable.
Give me one self-contained code cell, followed by a plain-language explanation of every major step and any assumptions.
