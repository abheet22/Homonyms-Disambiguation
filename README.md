# Homonyms-Disambiguation
A NLP based project which identifies the wrong homonyms used in the sentences and suggests the correct homonym.

**Problem Statement** : 

Sometimes we get confuse with some words which sound similar but have a totally different meaning (These words are known as homonyms). 
**Example** : 

ACCEPT VS EXCEPT

ACCEPT– to receive something
India ACCEPTED its defeat at the hands of Australia.

EXCEPT– to take or leave out
All the children were given a share in the property EXCEPT  Rohit Sharma.

Examples:

Mr Axar Patel ACCEPTED the award for being the best motivational speaker in India.

All were dressed in blue EXCEPT one.

#### This module identifies the wrong homonym used in the sentence and suggests the correct one.

**Approach** :

Step 1 : Get the list of all the possible homonyms present in english dictionary.

Step 2 : Find the possible homonym in the inputted sentence and extract the combination of all the homonyms.

Step 3 : Filter out all the Nouns, adjective and verb from the given sentence (They only provide some relevant information).

Step 4 : Train a **word2vec** (to get word embeddings) on wiki dump.

Step 5 : Find the similarity of each combination of homonym  with Step 3 keywords and get the most suitable homonym to be used in the sentence.

**Performance** :

This module performed well with an accuracy of around **80 percent**.

