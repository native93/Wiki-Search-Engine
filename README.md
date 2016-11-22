
INDEXING STRUCTURE:

<pre>|-- bin 
|-- Index 
|   |-- body 
|   |   -- final.txt 
|   |-- category
|   |   -- final.txt
|   |-- external_links
|   |   -- final.txt
|   |-- infobox
|   |   -- final.txt
|   |-- reference 
|   |   -- final.txt 
|   |-- title 
|       -- final.txt
|-- README.txt 
|-- run.sh 
 -- src 
    |-- code.py 
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


