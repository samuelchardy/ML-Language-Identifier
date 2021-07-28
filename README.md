# ML-Language-Identifier
Using machine learning to determine the source language of a piece of text. Text from three languages with character crossover are used.

To avoid using expensive computational methods that are (in this case) surplus to requirements, I developed preprocessing techniques that manipulate the data into a format that allows ease of analysis.

The format of the processed data is a multi-language bigram hash-map, which contains the observed bigrams of each language as the key. The value associated with each key is the frequency of said bigram. When these frequencies are filled in for a piece of text it is easy to determine the origin language using cosine similarity between the vector of frequencies in the test and train data sets.

See the report on this work here:
https://www.researchgate.net/publication/351482569_Natural_Language_Identification_Using_Cosine_Similarity
