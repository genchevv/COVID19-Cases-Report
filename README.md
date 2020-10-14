# COVID19-Cases-Report 
This is a short Python 3.8 script that I wrote which helps my colleague export data from a weekly text report on the number of new COVID-19 cases in seven municipalities into an .xls file. It uses key phrases to assign categories to text. 

The logic of the script is that the report follows a fairly predictable structure from week to week - the paragraphs in a defined part of the text must all go into the "Prevention" category while other paragraphs are classified based on a repetitive textual pattern.

The task is to organize text from the report into seven categories. The script uses the Python NLTK and Panda libraries to first tokenize the text into sentences.
It then builds lists of paragraphs based on the appearance of key words. Each paragraph is assigned a unique ID.

The script then builds a dictionary where three of the categories (Date, Geo. Area, Ref.) are assigned to each entry. The rest of the categories remain the same for all entries.  

I have provided sample names for the entries used to locate paragraphs. We normally use the names of the municipalities. 
