# NoReC_gender

This dataset is described in the paper ["*Gender and sentiment, critics and authors: a dataset of Norwegian book reviews*"](https://www.aclweb.org/anthology/2020.gebnlp-1.11/) by S. Touileb, E. Velldal, and L. Øvrelid, presented at the Second Workshop on Gender Bias in Natural Language Processing, COLING 2020.

NoReC_gender comprises the _book reviews_ of the Norwegian Review Corpus (NoReC), here expanded with annotations of _gender_ of both book authors and critics (review authors).

# Terms of use

NoReC_gender inherits the license of the underlying [NoReC](https://github.com/ltgoslo/norec) corpus, copied here for convenience:

The data is distributed under a Creative Commons Attribution-NonCommercial licence (CC BY-NC 4.0), access the full license text here: https://creativecommons.org/licenses/by-nc/4.0/

The licence is motivated by the need to block the possibility of third parties redistributing the orignal reviews for commercial purposes. Note that machine learned models, extracted lexicons, embeddings, and similar resources that are created on the basis of NoReC are not considered to contain the original data and so can be freely used also for commercial purposes despite the non-commercial condition.

# Format and pre-processing

The book reviews are distributed as *.txt* files, split into pre-defined train, dev, and test sets (again, inherited from NoReC). The files contain sentence and paragraph segmented texts, processed using UDPipe. 

The metadata for each review is provided as a JSON object, all listed in a single file, metadata_norec_gender.json, indexed on the document id (corresponding to the file names). The JSON objects record several properties as the numerical rating (an integer in the range 1–6), the thematic category or domain, the URL of the original document, the names of the critics and their genders, the names of the book authors and their genders. For more information about the metadata, data sources, etc. please see the [NoReC repo](https://github.com/ltgoslo/norec).

# Cite

If you use this dataset, please cite the following paper:

```
@inproceedings{touileb-etal-2020-gender,
    title = "Gender and sentiment, critics and authors: a dataset of {N}orwegian book reviews",
    author = "Touileb, Samia and {\O}vrelid, Lilja and Velldal, Erik",
    booktitle = "Proceedings of the Second Workshop on Gender Bias in Natural Language Processing",
    month = dec,
    year = "2020",
    address = "Barcelona, Spain (Online)",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/2020.gebnlp-1.11",
    pages = "125--138"
}
```
