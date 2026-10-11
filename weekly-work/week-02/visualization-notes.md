1. What does one row represent?

A row represents one book. The row itself has 11 columns, which, where possible, individually hold all the important data tied to the book.

2. Does a row describe a physical copy, an edition, or an aggregate?

A single row describes an edition of a book, rather than a physical copy or an aggregate. 

3. Which columns contain categories?

I believe these columns are categories: author, printer, place, year, language, country, and decade.

4. Which columns contain quantities?

I believe the only column that contains quantities is year_numeric.

5. Which columns are identifiers rather than quantities?

I believe the columns that are identifiers are edition_id, short_title, and format.

6. How are dates represented in year, year_numeric, and decade?

Year is represented as a string value. The decade is a string w/ blanks, and year_numeric is a number w/ blanks data type. For example, 1925 would be depicted as 1920s.
The year_numeric data is received by reading the first 4 numerical digits in the year value.
For example, 1924 (=1925) would be 1924 but stored as a numerical value. The decade is determined by the value of year_numeric.

8. How are missing values represented?

Missing values lack any data in the dedicated box. They can be easily spotted by simply looking at the chart and looking for the empty boxes.
Empty boxes do not automatically mean that the value is anonymous, rather, the data is just not known or identified.

9. Are any categories uncertain, inconsistent, or historically constructed?

I believe that when the date of production is uncertain, the year that is estimated to be the print year is surrounded by brackets []. 
