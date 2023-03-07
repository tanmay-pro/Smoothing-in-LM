### Smoothing in Language Modelling

## File Structure

- Run the file "kn.ipyb" for creating a language model while performing Kneser-ney Smoothing.
- Run the file "wb.ipyb" for creating a language model while performing Witten-Bell Smoothing.
- The corpus directory contains two different corpora (Difference in terms of size).

## Key Points

- Unknown words have been handled by adding <unk> tags in the language models. Incase a word appears less than a value (some aprticular frequency threshold which can be changed in the files) in the training set, it has been replaced by the <unk> token. Similarly, while calculating the perplexities on the test sets, if a word has not appeared before, it has been replaced by an <unk> token. This solves the issue of having an Open Vocabulary.

- <SOS> and <EOS> tags have been added to take into account a 4-gram model. Not using these tokens would lead to a loss in the amount of information extracted from a sentence.

- NLTK has not been used for tokenization, instead, a custom function has been written for the same.

