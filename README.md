This project is part of my NLP Course. </br>

This project is inspired by 2 games - wordle and pimantle.</br>

In wordle, a user has to guess a 5-letter word within 6 tries. No information regarding the word is given other </br>
than which letters are correctly positioned or which are present in the chosen wod but not in the correct position. </br>

In pimantle, the user has to guess a word based on semantic similarity. The more closer one is to the chosen word, </br>
the greater the semantic similarity. </br>

In this game, the user must guess the word within 7 tries with only three hints provided. These hints </br>
are available only after the user has tried to guess the word atleast once. </br>

The dataset is made up of words available within the wordnet vocabulary. Preprocessing is done on the vocab </br>
to lowercase words, lemmatize, stem, remove special characters and remove numbers. Whatever words are left, </br>
their definitions are then taken and synonyms are taken and made into the remaining columns of the dataset. </br>

Next, the three hints are generated by three different methods - semantic similarity using coine similarity, keyphrase </br>
extraction from the word's definitions and clustering semantically similar words and choosing the closest word from </br>
a given cluster.

Word2Vec, FastText and Bert was used to embed the dataset fo hint 1 but BERT gave the best results. </br>
WordVec, FastText and KeyBert were used for hint 2 but KeyBert gave the best results.
Glove, FastText, BERT and DistilBert were used for hint 3, BERT and DistilBert gave the best results but we used </br>
DistilBert for diversity of models. </br>