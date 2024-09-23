Annotated Datasets for Transformer-based Scholarly Information Extraction and Linguistic Linked Data Generation

The folder contains a manually curated and annotated, multidisciplinary datasets from research articles (abstract and main text), each associated with the corresponding article's metadata. Each dataset is in jsonl format where each line consists of a dictionary with the following structure:

{"text": the text of each sentence, 
 "meta": dictionary containing all the metadata piblication information of the corresponding article from which the sentence was derived,
 "answer": classification of the quality of the annotation/sentence based on Prodigy annotation style. For datasets regarding relation extraction this field denotes whether the relation holds or not for the cooresponding relation span,
 "spans": list of annotation spans, each containing information regarding character and token based pointers and the annoation label,
 "tokens": list of the tokens of the sentence
 }
 
The datasets can be used as a source for linguistic linked data by them selfs, or for fine tunning transformer-based classifiers that extract from scholarly publications the cooresponding annoated entity /relation types.

The datasets were created with Prodigy annotation software. 




