# MiddelNER (Middelnederlandse named entity recognition)
This repository is the result of an internship at the University of Ghent. It is an attempt to perform Named Entity Recognition on Middle Dutch charters. The data used is adapted from the C14NL corpus of non-literary Middle Dutch texts (https://bouwstoffen.kantl.be/C14NL/). 155 charters of the linguistically enriched C14NL-PoS subcorpus were annotated for this project and can also be found in this repo. 

First experiments folder contains small tests with existing resources, including pietagger:
```
@inproceedings{manjavacas-etal-2019-improving,
    title = "Improving Lemmatization of Non-Standard Languages with Joint Learning",
    author = "Manjavacas, Enrique  and
      K{\'a}d{\'a}r, {\'A}kos  and
      Kestemont, Mike",
    booktitle = "Proceedings of the 2019 Conference of the North {A}merican Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers)",
    month = jun,
    year = "2019",
    address = "Minneapolis, Minnesota",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/N19-1153",
    doi = "10.18653/v1/N19-1153",
    pages = "1493--1503",
    abstract = "Lemmatization of standard languages is concerned with (i) abstracting over morphological differences and (ii) resolving token-lemma ambiguities of inflected words in order to map them to a dictionary headword. In the present paper we aim to improve lemmatization performance on a set of non-standard historical languages in which the difficulty is increased by an additional aspect (iii): spelling variation due to lacking orthographic standards. We approach lemmatization as a string-transduction task with an Encoder-Decoder architecture which we enrich with sentence information using a hierarchical sentence encoder. We show significant improvements over the state-of-the-art by fine-tuning the sentence encodings to jointly optimize a bidirectional language model loss. Crucially, our architecture does not require POS or morphological annotations, which are not always available for historical corpora. Additionally, we also test the proposed model on a set of typologically diverse standard languages showing results on par or better than a model without fine-tuned sentence representations and previous state-of-the-art systems. Finally, to encourage future work on processing of non-standard varieties, we release the dataset of non-standard languages underlying the present study, which is based on openly accessible sources.",
}
```
The repo also contains a colab notebook with three models. A simple Bi-LSTM, a model made with SpaCy and a BERT model based on BERTje.
```
@misc{devries2019bertje,
	title = {{BERTje}: {A} {Dutch} {BERT} {Model}},
	shorttitle = {{BERTje}},
	author = {de Vries, Wietse  and  van Cranenburgh, Andreas  and  Bisazza, Arianna  and  Caselli, Tommaso  and  Noord, Gertjan van  and  Nissim, Malvina},
	year = {2019},
	month = dec,
	howpublished = {arXiv:1912.09582},
	url = {http://arxiv.org/abs/1912.09582},
}
```
