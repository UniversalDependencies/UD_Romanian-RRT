Romanian UD treebank

*** Update Jan 17th, 2017: train == dev == test, doing bug fixing.

The Romanian UD treebank (called RoRefTrees) (Barbu Mititelu et al., 2016) is based on RACAI-RoTb (Irimia and Barbu Mititelu, 2015) and on UAIC-RoTb (Perez, 2014). The distribution of text genres in RoRefTrees is not balanced: literature - 1818 sentences, law - 1606 sentences, medical - 1210 sentences, FrameNet translations - 1092 sentences, academic writing - 950 sentences, news - 933 sentences, science - 362 sentences, wikipedia - 251 sentences, miscellanea - 1301 sentences. The most frequent relation in RoRefTrees is nmod (14.97% relative frequency) and the least frequent is reparandum (only 1 occurrence in the whole treebank).

For the third release of Romanian UD trees, the team of the SSPR project (Verginica Mititelu, Elena Irimia, Cenel-Augusto Perez, Radu Ion and Radu Simionescu) focused both on the size increase of the treebank and on the morphologic and syntactic annotation consistency of the treebank.

DATA SPLITS

We split the treebank as follows: the test set (ro-ud-test.conllu) is 12.5% of the whole treebank, the development set (ro-ud-dev.conllu) also 12.5%, while the rest of the treebank (75%) is the training set (ro-ud-train.conllu). The data was split in a random fashion.

BASIC STATISTICS

Tree count:  9523
Word count:  218511
Token count: 218511
Dep. relations: 50 of which 11 language specific
POS tags: 17
Category=value feature pairs: 57

ACKNOWLEDGEMENTS

This work was supported by a grant of the Romanian National Authority for Scientific Research and Innovation, CNCS - UEFISCDI, project number PN-II-RU-TE-2014-4-1362.

REFERENCES

V. Barbu Mititelu, R. Ion, R. Simionescu, E. Irimia, C-A Perez. 2016. The Romanian Treebank Annotated According to Universal Dependencies. Proceedings of HrTAL2016, Dubrovnik, Croatia, 29 September - 1 October 2016.
R. Ion, E. Irimia, D. Ștefănescu, D. Tufiș. 2012. ROMBAC: The Romanian Balanced Annotated Corpus. Proceedings of LREC'12, Istanbul, Turkey.
E. Irimia, V. Barbu Mititelu. 2015. Building a Romanian Dependency Treebank. Corpus Linguistics 2015, Lancaster, UK, 21-24 July 2015.
C-A Perez. 2014. Resurse lingvistice pentru prelucrarea limbajului natural, PhD thesis, A.I. Cuza University of Iasi.


CHANGELOG

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


=== Machine-readable metadata =================================================
Documentation status: partial
Data source: semi-automatic
Data available since: UD v1.2
License: CC BY-SA 4.0
Genre: wiki legal news fiction medical nonfiction scientific
Contributors: Mititelu, Verginica; Irimia, Elena; Perez, Cenel-Augusto; Ion, Radu; Simionescu, Radu; Mărănduc, Cătălina
Contact: Verginica Mititelu (vergi@racai.ro)
===============================================================================
