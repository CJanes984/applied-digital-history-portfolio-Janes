Part 1:
Checkpoint 1: In your own words, explain the difference between NLP and an LLM. Give one historical question for which NLP could help, and identify one part of that question that a word count could not answer.
NLP - Natural Language Processing, a broad field utilizing computers to process, analyze, or generate human language. NLP includes models ranging from extremely simple to complex. Just as every square is a rectangle, every LLM is an NLP. Just as not every rectangle is a square, not every NLP is an LLM. 
An NLP could help to answer a question similar to, have common phrases shifted largely throughout the past 200 years of the most popular English literature? This question asks for a quantifiable answer. Using NLP to test for similarities and differences across texts can make someone more efficient at finding their answers when the question relates to a large dataset. The word count could not answer why there was a change in vocab over the period, only that there was a shift.

Part 2:
Checkpoint 2: Why would a historian need to return to individual passages after identifying a frequency pattern?
When the historian uses the NLP to examine the texts, the samples are being treated individually and become a single massive dataset. So, the historian needs to go back through the individual records and read them closely to get their truest meanings. The close reading is also needed to understand what a term is referring to. For example, a term like “the cars” appearing multiple times could be referring to different kinds of cars. 

Part 3:
Checkpoint 3: Confirm that the folder contains 57 documents covering 1789–2013. Record what one document represents and one reason the corpus should not be treated as a transparent record of American political language.
√ - Each document represents one speech from the inauguration of the United States President. The records should not be treated as a record of American political language because the speeches have been perfected and rewritten hundreds of times to make them come off as relatable and caring as possible. 
 Part 4:
Checkpoint 4: Explain why relative frequency may be preferable to raw frequency when comparing two speeches.
Raw frequency counts are useful when trying to inspect a document, but if someone is trying to inspect documents of differing lengths, it can become misleading. Relative frequency counts express the number in relation to the document’s length. Relative frequency counts can help when trying to compare two or more documents of differing lengths to one another. 

Part 5:
Checkpoint 5: Voyant reports 57 documents. Record its total word count and confirm that 2_washington_1793.txt is the shortest document and 14_harrison_1841.txt is the longest. If Voyant reports something different, inspect the corpus before continuing.
√

Part 6:
5  Most Prominent Words:
1)	Government (596 Occurrences)
2)	People (564 Occurrences)
3)	States (335 Occurrences)
4)	Great (334 Occurrences)
5)	Shall (312 Occurrences)
Word size represents the number of times the words appear in total across all the speeches. Common words like and, we, and the are not shown in the Cirrus.
1)	Record the raw counts of five frequent terms.
Government: 596 occurrences, People: 564 occurrences, States: 335 occurrences, Great: 334 occurrences, and Shall: 312 occurrences.
2)	Identify one word whose prominence might reflect the genre of inaugural addresses.
The term government having substantial occurrence indicates a relationship to inaugural addresses.
3)	Identify one word that could support a historical question.
The term occurring so often raises the question of when the term ‘people’ was used so often. Is the term still being used so frequently, or was it simply used so often in the past that it still tops the top five most used words?
#1
Evidence: In the processed corpus, the token ‘Government’ occurs 596 times and ranks among the #1 most frequent displayed terms.
Possible interpretation: This pattern might relate to the president's focus and effect on the government, but establishing that interpretation would require examining the text files individually and comparing them with other inaugural speeches.
#2
Evidence: In the processed corpus, the token ‘Constitution’  occurs 209 times and ranks among the 15 most frequent displayed terms.
Possible interpretation: This pattern might relate to the Constitution’s control over the functioning of the government, but establishing that interpretation would require examining each text file and comparing it with other speeches given by presidents.

Part 7:
## FINDING STOP WORDS SETTINGS
-	To find the stop words setting, you must click on the “Define options for this tool.” slider.
The stop word setting is currently set to “Auto-detect”. Meaning it will define what terms are stop words automatically.
5 Most Prominent Words:
1)	The (10044 Occurrences)
2)	Of (7074 Occurrences)
3)	And (5265 Occurrences)
4)	To (4506 Occurrences)
5)	In (2782 Occurrences)
When removing the auto-detect setting for stop words and setting it to “None”, the word cloud becomes clouded by filler words and connection words like ‘the’ and ‘of’. Terms like ‘government’ and ‘people’ get filtered out by the overwhelming amount of ‘the’ and ‘of’.
Word Removal: “People.” A historian could remove the term “People” to allow less frequent words to appear and show their quantifiable amount. This wouldn’t affect the data significantly and wouldn’t cause much confusion. However, if the historian is trying to cover the way presidents focus and what topics they sway towards. Removing a term as valuable as “People” could make the data misrepresent the truth and imply that they don’t focus on the “People” in their speeches.
Before the new stop word:
1)	Government (596 Occurrences)
2)	People (564 Occurrences)
3)	States (335 Occurrences)
4)	Great (334 Occurrences)
5)	Shall (312 Occurrences)
After the new stop word:
1)	Government (596 Occurrences)
2)	States (335 Occurrences)
3)	Great (334 Occurrences)
4)	Shall (312 Occurrences)
5)	World (308 Occurrences)
Answer:
-	Which output is the "correct" word cloud?
Neither output can be determined “correct.” Both outputs could be utilized depending on the intention for the word cloud.
-	What analytical purpose might justify each version?
Someone analyzing the word cloud could use it to identify how much certain issues or subjects have been focused on by previous presidents. Someone could also use the updated word cloud to identify what the top five most used words were and how those words could change their viewpoint of presidential speeches.
-	Why should a historian document the stop word list used?
If the historian doesn’t document what stop words they used for their data, it could confuse the viewers or present false data. This data needs to be easily reproducible as well, so if the stop words weren’t documented, it could become difficult to create the same conditions and get the same results.

Part 8:
How do selected inaugural addresses use vocabulary concerning political community, government, and national identity?
The inaugural speeches heavily focus on phrases regarding people, government, and states. These words are among the top five most common in the 57 documents recorded and input into Voyant Tools. 
Values (Three Speeches)
1-	10_adams_john_quincy_1825
a.	Government (Relative: 0.0058199)
b.	People (Relative: 0.0023964)
c.	Nation (Relative: 0.0027388)

2-	39_roose_franklin_1941
a.	Government (Relative: 0.0028798)
b.	People (Relative: 0.0050396)
c.	Nation (Relative: 0.0079194)

3-	52_clinton_1997
a.	Government (Relative: 0.0074766)
b.	People (Relative: 0.0074766)
c.	Nation (Relative: 0.0060102)
In the raw frequencies, the speech by Polk appears most prominently. He mentioned government 47 times and states 36 times. When switching to relative frequencies, the charts change dramatically. Rather than using word counts, they switch to a count that somewhat mimics a percentage.
When resizing the Voyant Tools window on Safari, the page must be reloaded to fix the positions of the charts. 
-	In this corpus, the relative frequency of shall is higher in the 2_washington_1793 address than in the 40_roosevelt_franklin_1945 address. 
o	This could be the case because, due to the historical time, a word like ‘shall’ could be much more heavily depended on and a more common everyday phrase. Over time, the use of the word in different sentence structures could fade, leading to the much lower frequency of shall being used.
o	The trending use of ‘shall’ dropping so far could also reflect the government’s strength and belief in its prosperity. At the time Washington was using it, the nation was extremely young and would’ve needed a lot of effort to push through the struggles of an emerging nation, while when Roosevelt was giving his inaugural speech, the U.S. had already existed for quite a while. 
What additional texts would be needed to determine whether this is (choose two):
•	a difference between individual speeches; *X*
•	a difference between presidents;
•	a response to a particular political crisis; *X*
•	a broader chronological change;
•	a feature of changing inaugural rhetoric?
As I stated previously, it could be a difference in the response to the political climate they were in at the time. With a young nation and an older nation experiencing struggles in vastly different ways. It could also simply be a difference in their individual speeches, but to find out which is true, we would need to sample some other speeches given by both Washington and Roosevelt aside from their inaugural speeches.
Checkpoint 7: You have compared raw and relative frequency, recorded a change or stability, and identified evidence needed to explain the pattern.
√
Part 9:
1)	‘Government’ - 10_adams_john_quincy_1825
a.	Quote: “…the whole action of the Government instituted by it should be invariably and sacredly devoted--to form a more perfect union, establish justice, ensure domestic tranquility, provide for the common defense, promote the general welfare, and secure the blessings of liberty…”
b.	The term appears to refer to the U.S. government and its duties. 
c.	Words like ‘union’, ‘justice’, and ‘welfare’ appear to help define the government’s role in the speech.
d.	The speech is making a positive statement regarding the duties of the government and how it will uphold them.

2)	‘Government’ - 24_garfield_1881
a.	Quote: “We cannot overestimate the fervent love of liberty, the intelligent courage, and the sum of common sense with which our fathers made the great experiment of self-government.”
b.	The term appears to refer to the creation of a nation that was supposed to be governed by the people.
c.	Words like ‘intelligent’, ‘courage’, and ‘great’ appear to help define the value of the experimental role of a new governing system in the speech.
d.	The speech is making a positive statement regarding the value of self-governance.

3)	‘Government’ - 57_obama_2013
a.	Quote: “Through it all, we have never relinquished our skepticism of central authority nor have we succumbed to the fiction that all society's ills can be cured through government alone.”
b.	The term appears to refer to the struggles that trying to aid the world through governmental processes can bring.
c.	Words like ‘fiction’, ‘ills’, and ‘alone’ appear to help define the difficulties of trying to help the citizens in a nation through slow-moving governmental efforts.
d.	The speech is making an almost negative statement regarding the slow process of governmental progressiveness.
Checkpoint 8: You have examined at least three occurrences of one term in different speeches and recorded what the term appears to refer to, the nearby words that qualify it, and how it functions in each passage.
√
Part 10:
How do references to conflict—such as war, peace, or enemy—vary across speeches?
I was unable to think of a question to ask, so I used one of the five given questions to use. My chosen question was: “How do references to conflict, such as war, peace, or enemy, vary across speeches?” The relative frequency chart shows that the terms ‘peace’, ‘war’, and ‘enemy’ have been used somewhat rarely. Though the most often used of the three of them is war, followed by peace, and finally by enemy. In the speech titled “45_Johnson_1965”, the speaker refers to the enemy as a waste of resources. In the speech titled “7_madison_1813”, the speaker refers to the enemy as one who has restrained United States soldiers. Over the roughly 150 years after Madison gave his speech, Johnson describes the enemy as an economic problem. Finally, in the speech titled “56_obama_2009”, Obama speaks of the creation of the government and how difficult it was to persevere through. It appears that over time the term enemy began shifting as to what it referred to. In the earliest speech I documented here, it was referring to the enemy as a foreign nation that took soldiers prisoner during wartime. By the time Johnson spoke, he referred to the enemy as a waste of resources. The ‘enemy’ has been ever-changing since the first speeches. The main limitation is that we are unable to know why this term has been changing or what’s been the main cause of it. Also, we are unaware of why it appeared so frequently throughout each of the speeches.

Part 11:
How could you use text analysis with Voyant in a research project? Briefly describe the corpus you might use, the question you would investigate, and one limitation you would need to consider.
Text analysis could be extremely helpful for research because it could allow someone to easily look at the word counts and how often they occur. Also, it can visualize the text into different kinds of graphs and give an idea of how speech has changed over different time periods. Using the relative frequency, raw frequency, and the Cirrus could provide invaluable amounts of information at a quick glance. Rather than having the historian read through each document individually. These tools exponentially speed up the historian’s work process. The main limitation that must always be noted is that these results do not give an idea of why the patterns appear as they do. The tools only show the correlation, rather than the reasoning.

