# AN-AUTOMATED-SYSTEM-FOR-LEXICAL-NORMALIZATION-OF-NOISY-TEXT-WITH-NAMED-ENTITY-RECOGNITION
The objective of the project is to create a model to convert noisy text into non-noisy and then tagging every word present in comic books using lexical analysis.

MODULES:
  Here we will be passing threecomic storiesas the dataset. We have implemented the first module completely and the second module partially.
  
MODULE I-PREPROCESSING
  •Segmentation: The data present in comic book (dataset) are split into sentences.
  •Punctuation removal:Removing punctuation mark from each sentenceafter segmentation.
  •Tokenization: Tokenization is the process of breaking down the given text in natural language processing into the smallest unit in a sentence called a token. In this technique, we will be splitting each sentence in the book into words.
  INPUT: Comic story(text)
  OUTPUT: Tokens 
  
MODULE II-POS TAGGING
  Here we have passed the output of the first module and then we have divided the tokens into noisy and non-noisy text. The non-noisy text will undergo POS tagging.
  INPUT:Tokens
  OUTPUT:POS tagged non-noisy text
 
MODULE III-REMAINING NOISY TO NON-NOISY WORDS
  Herethe remaining noisy words from module 2 is converted into non-noisy form. Same as above POS tagging is done for those words. And the noun alone will be saved in a separate file for NER tagging.
  INPUT: Noisy text
  OUTPUT: Words POS tagged as nouns
  
MODULE IV-NER TAGGING
  The NER (Named Entity Recognition) tagging will be done for the words which are POS tagged as nouns.  Here the noun.txt is the input file.
  INPUT:Words POS tagged as nouns
  OUTPUT:NER tagged words
