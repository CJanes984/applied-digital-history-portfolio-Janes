**1.	Report one result you independently validated and explain how you validated it.**
I validated that the code was not trying to overwrite or edit the original data when being uploaded to the HTML address on a search engine. 
After glancing over the code and having the LLM give me a rundown on what specific parts of the code do, I was able to be sure it was safe for use.

**2.	Identify one missing-data pattern in the book dataset.**
In the original book-sample.csv file, the edition_id value of 76584 is missing both the author, the language, and the format. 
This could cause problems depending on how the code is produced.

**3.	Describe one way you improved a prompt after seeing code or output.**
When seeing the output of the code, I realized there were minor mistakes regarding the names of the columns. 
These fixes were fairly easy to spot and extremely easy to fix. 
Thankfully, it didn’t take much time to fix these small errors, and any major ones were able to be fixed with help from the LLM.

**4.	Describe one error or questionable assumption and how you diagnosed it.**
When I was trying to make the HTML files run in a web browser. 
Every time I used TextEdit to export the HTML file and I tried to open it I would only see the source code. 
After roughly half an hour, I got help from the LLM, and it fixed the code for me. 
The error occurred because some of the function code was mistyped. Rather than being a function, at times it was written fvnction.

**5.	What does it mean to supervise generated code rather than merely accept it?**
Supervising generated code is ensuring that the code the LLM produces is safe to run, 
doesn’t edit the existing dataset or files, and follows the exact outlines prompted to it. 
The LLM is not to be used to replace the worker, but rather to aid the worker. 
Though it often gets abused as a simple replacement for the workforce.

**6.	What parts of this workflow should remain the historian's responsibility even if the code executes correctly?**
Ensuring the data sets are correct and aren’t being hallucinated, overwritten, or destroyed in any way. 
The historian is responsible for keeping the data accurate and in a simple, organized format.
