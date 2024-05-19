An Annotated Dataset for Transformer-based Scholarly Information Extraction and Linguistic Linked Data Generation

The file contains a manually curated and annotated, multidisciplinary dataset of 15,262 sentences from research articles (abstract and main text) each associated with the corresponding article's metadata. The dataset is in jsonl format where each line consists of a dictionary with the following structure:

{"text": the text of each sentence, 
 "meta": dictionary containing all the metadata piblication information of the corresponding article from which the sentence was derived,
 "answer": classification of the quality of the annotation/sentence based on Prodigy annotation style,
 "spans": list of annotation spans, each containing information regarding character and token based pointers and the annoation label,
 "tokens": list of the tokens of the sentence
 }
 
The dataset can be used as a source for linguistic linked data by it self, or for fine tunning transformer-based classifiers that extract from scholarly publications three types of entities:

1) Research methods, named entities of variable length.
2) Research goals, entities that appear as textual spans of variable length with mostly fixed lexico-syntactic-structure.
3) Research activities, entities that appear as textual spans of variable length with complex lexico-syntactic structure.

The dataset was created with Prodigy annotation software using the spans-manual recipie. 




