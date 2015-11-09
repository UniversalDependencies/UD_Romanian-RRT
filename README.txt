Romanian UD treebank

The Romanian UD treebank (called RoRefTrees) is based on RACAI-RoTb (Irimia and BarbuBarbu Mititelu, 2015) and on UAIC-RoTb (Perez, 2014). In the latter, the texts were selected in order to have all syntactic functions represented in the treebank: the 35 relations used to annotate the 5800 sentences occur, altogether, 41210 times. The percent of each relation representation in the treebank vary from 14.48% (the most frequent, namely the complement of a preposition) to 0.02% (the least frequent, namely the adjunct expressing exception). RACAI-RoTb presents the advantage of having been created on the basis of a balanced corpus (Ion et al., 2012), from which 5000 sentences were selected so as to belong to all domains represented in the corpus, to respect frequency criteria for verbs, as well as to have various lengths. As a consequence, the texts in RoRefTrees belong to various styles (journalistic, belletristic, law, science) and are rather balanced (statistics will be offered in the final form of the paper). Thus, we can say that the resulted treebank features all possible syntactic relations for Romanian.
For this first release of Romanian UD trees, we semi-automatically mapped the two originar treebanks (RACAI-RoTb and UAIC-RoTb) to the UD annotation style by the team of the SSPR project (Verginica Mititelu, Elena Irimia, Cenel-Augusto Perez, Radu Ion and Radu Simionescu), with help from Catalina Maranduc.

DATA SPLITS

We split the treebank as follows:
Roughly, the test set (ro-ud-test.conllu) is 12.5% of the whole treebank, the development set
(ro-ud-dev.conllu) also 12.5%, while the rest of the treebank (75%) is the training set (ro-ud-train.conllu).
When splitting data, we aimed at having the same distribution of domains in all sets.

BASIC STATISTICS

Tree count:  633
Word count:  12094
Token count: 12094
Dep. relations: 49 of which 11 language specific
POS tags: 17
Category=value feature pairs: 53

ACKNOWLEDGEMENTS

This work was supported by a grant of the Romanian National Authority for Scientific Research and Innovation, CNCS - UEFISCDI, project number PN-II-RU-TE-2014-4-1362.

REFERENCES

R. Ion, E. Irimia, D. Ștefănescu, D. Tufiș. 2012. ROMBAC: The Romanian Balanced Annotated Corpus. Proceedings of LREC'12, Istanbul, Turkey.
E. Irimia, V. Barbu Mititelu. 2015. Building a Romanian Dependency Treebank. Corpus Linguistics 2015, Lancaster, UK, 21-24 July 2015.
C-A Perez. 2014. Resurse lingvistice pentru prelucrarea limbajului natural, PhD thesis, A.I. Cuza University of Iasi.


=== Machine-readable metadata =================================================
Documentation status: partial
Data source: semi-automatic
Data available since: UD v1.2
License: CC BY-SA 4.0
Genre: wiki legal news fiction medical nonfiction
Contributors: Mititelu, Verginica; Irimia, Elena; Perez, Cenel-Augusto; Ion, Radu; Simionescu, Radu; Mărănduc, Cătălina
===============================================================================
