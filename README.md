# Text-searcher
Implemented a Full-Text search application that will produce improved results using NLP features and techniques.It includes a keyword-based strategy and an improved strategy using NLP feature and techniques.

EXECUTION:

1. pdf.py(converts the pdf documents to txt files)
2. tf-idf.py(extracts the matched sentence from the corpus using tf-idf and cosine similarity technique)
3. whoosh.py(searches the indexed corpus by BM25F )
4. part1.py(performs the addition of data to solr)
5. part2.py(extracts the matched sentence from solr)
6. pysolr.py(modified version of pysolr.Containns an added method(disjunction_max()) of the solr object in order to add weights to the querry features)
7. rural.txt(corpus used for part1 and part2)
8. input.txt(input string for part1 and part2)
9. doc(corpus for others)

part1 takes corpus(rural.txt) as command line argument.
part2 takes corpus(rural.txt) and input(input.txt) as command line arguments.


tf-idf->)Used Python, NLTK, NLP techniques to make a search engine that ranks documents based on search keyword, based on TF-IDF weights and cosine similarity.The code will read a corpus and produce TF-IDF vectors for documents in the corpus. Then, given a query string, you code will return the query answer--the document with the highest cosine similarity score for the query.

whoosh->)Whoosh is a library of classes and functions for indexing text and then searching the index. It allows you to develop custom search engines for your content.It uses Fielded indexing and search,Fast indexing and retrieval,Pluggable scoring algorithm (default BM25F), text analysis, storage, posting format,etc.

part1 and part2->)Implement a shallow NLP pipeline to perform the following: a. Keyword search index creation  Segment the News articles into sentences  Tokenize the sentences into words  Index the word vector per sentence into search index such as Lucene or SOLR b. Natural language query parsing and search  Segment an user’s input natural language query into sentences  Tokenize the sentences into words  Run a search/match with the search query word vector against the sentence word vector (present in the Lucene/SOLR search index) created from the corpus c. Evaluate the results of at least 10 search queries for the top-10 returned sentence matches



