
INDEXING STRUCTURE:

<pre>|-- bin <br/> 
|-- Index <br/>
|   |-- body <br/>
|   |   -- final.txt <br/>
|   |-- category <br>
|   |   -- final.txt <br>
|   |-- external_links <br>
|   |   -- final.txt <br>
|   |-- infobox <br>
|   |   -- final.txt <br>
|   |-- reference <br>
|   |   -- final.txt <br>
|   |-- title <br>
|       -- final.txt <br>
|-- README.txt <br>
|-- run.sh <br>
 -- src <br>
    |-- code.py <br>
    |-- stopwords.txt
</pre>
LIBRARIES : 

	PyStemmer - for stemming
	SAX Parser - for parsing

LAYOUT OR DESCRIPTION :

 - Used SAX Parser for XML Parsing. 
 - Divided into six categories - Body, Category, External Links, Info-box, Rerefences and title.
 - Parsed XML accordingly and all the categories were obtained.
 - Stopwords removal using stopwords.txt (src/stopwords.txt) in each category.
 - Stemming via inbuilt pystemmer in each category.
 - Maintained a dictionary for each category and a global for tfig.
 - Dictionary is wriiten into file after every 1000 documents. 
 - Separate files are maintained for every category.
 - After all the text files written (13 in the sample case), merge is perfomed in each category.
 - Merge is performed by Two-Way Merge Sort and  Min Heap + Stack used for optimization. 


