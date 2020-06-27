# DNA Sequencing Classifier
Here is a classification model that can predict a gene's function based on the DNA sequence of the coding sequence alone.

Treating DNA sequence as a language known as k-mer counting.
A challenge that remains is that none of these above methods results in vectors of uniform length which is a requirement for feeding data to a classification or regression algorithm.
So with the above methods you have to resort to things like truncating sequences or padding with "n" or "0" to get vectors of uniform length.

Take the long biological sequence and break it down into k-mer length overlapping “words”. 
In genomics, we refer to these types of manipulations as "k-mer counting", or counting the occurances of each possible k-mer sequence. 
so, we will convert this sequence or say string k-mer words.
For example,"words" of length 6 (hexamers), “ATGCATGCA” becomes: ‘ATGCAT’, ‘TGCATG’, ‘GCATGC’, ‘CATGCA’. 
Hence our example sequence is broken down into 4 hexamer words.
