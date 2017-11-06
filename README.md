# Summary

The Romanian UD treebank (called RoRefTrees) (Barbu Mititelu et al., 2016) is the reference treebank in UD format for standard Romanian.

# Introduction

It is based on RACAI-RoTb (Irimia and Barbu Mititelu, 2015) and on UAIC-RoTb (Perez, 2014). The distribution of text genres in RoRefTrees is not balanced: literature - 1818 sentences, law - 1606 sentences, medical - 1210 sentences, FrameNet translations - 1092 sentences, academic writing - 950 sentences, news - 933 sentences, science - 362 sentences, wikipedia - 251 sentences, miscellanea - 1301 sentences. These genres can be told apart by the sentences id.

# DATA SPLITS

We split the treebank as follows: the test set (ro-ud-test.conllu) is 12.5% of the whole treebank, the development set (ro-ud-dev.conllu) also 12.5%, while the rest of the treebank (75%) is the training set (ro-ud-train.conllu). The data was split in a random fashion.

# BASIC STATISTICS

Tree count:  9523
Word count:  218511
Token count: 218511
Dep. relations: 50 of which 11 language specific
POS tags: 17
Category=value feature pairs: 57

# Acknowledgments

This work was supported by a grant of the Romanian National Authority for Scientific Research and Innovation, CNCS - UEFISCDI, project number PN-II-RU-TE-2014-4-1362.

# REFERENCES

V. Barbu Mititelu, R. Ion, R. Simionescu, E. Irimia, C-A Perez. 2016. The Romanian Treebank Annotated According to Universal Dependencies. Proceedings of HrTAL2016, Dubrovnik, Croatia, 29 September - 1 October 2016.
R. Ion, E. Irimia, D. Ștefănescu, D. Tufiș. 2012. ROMBAC: The Romanian Balanced Annotated Corpus. Proceedings of LREC'12, Istanbul, Turkey.
E. Irimia, V. Barbu Mititelu. 2015. Building a Romanian Dependency Treebank. Corpus Linguistics 2015, Lancaster, UK, 21-24 July 2015.
C-A Perez. 2014. Resurse lingvistice pentru prelucrarea limbajului natural, PhD thesis, A.I. Cuza University of Iasi.


# CHANGELOG

UD 1.2 --> 1.3
- the number of trees was considerably increased.
UD 1.3 --> 1.4
- increase the treebank size to 9523 sentences;
- identical sentences (disregarding punctuation and numbers) at word form level have been removed;
- added a scientific (Physics, Mathematics and Computer Science) sub-corpus to make up for the loss;
- removed all words with underscores;
- removed most of the errors reported by the content validation tool;
- extensive POS-tagging and lemmatization corrections;
- ensuring more consistent data at the lexical, morphological and syntactic levels.
UD 1.4 --> 2.0
- manual improvements of the annotation, concerning POS-tagging, syntactic labeling, one sentence split.
- automatic conversion to UDv2 guidelines using Udapi (http://udapi.github.io/) ud.Convert1to2
- automatic reconstruction of original texts (ud.ro.SetSpaceAfter), pseudo-documents marked with newdoc markup
- re-split: train=185,113 (84.7%) tokens, dev=17,074 (7.8%) tokens, dev=16,324 (7.5%) tokens. Each pseudo-document equally distributed into train/dev/test.
- test set omitted from the UDv2.0 official release because of CoNLL 2017 shared task.
UD 2.0 --> 2.1
- no modifications to the previous version.


=== Machine-readable metadata =================================================
Data available since: UD v1.2
License: CC BY-SA 4.0
Includes text: yes
Genre: wiki legal news fiction medical nonfiction science
Lemmas: automatic
UPOS: converted with corrections
XPOS: automatic
Features: converted with corrections
Relations: manual native
Contributors: Barbu Mititelu, Verginica; Irimia, Elena; Perez, Cenel-Augusto; Ion, Radu; Simionescu, Radu; Popel, Martin
Contributing: elsewhere
Contact: vergi@racai.ro
===============================================================================
