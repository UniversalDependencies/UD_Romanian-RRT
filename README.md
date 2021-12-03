# Summary

The Romanian UD treebank (called RoRefTrees) (Barbu Mititelu et al., 2016) is the reference treebank in UD format for standard Romanian.

# Introduction

It is based on RACAI-RoTb (Irimia and Barbu Mititelu, 2015) and on UAIC-RoTb (Perez, 2014). The distribution of text genres in RoRefTrees is not balanced: literature - 1818 sentences, law - 1606 sentences, medical - 1210 sentences, FrameNet translations - 1092 sentences, academic writing - 950 sentences, news - 933 sentences, science - 362 sentences, wikipedia - 251 sentences, miscellanea - 1301 sentences. These genres can be told apart by the sentences id.

# DATA SPLITS

We split the treebank as follows: the test set (ro-ud-test.conllu) is 12.5% of the whole treebank, the development set (ro-ud-dev.conllu) also 12.5%, while the rest of the treebank (75%) is the training set (ro-ud-train.conllu). The data was split in a random fashion.

The corpus is split into documents corresponding to several genres:

**Legal**: document ids:
Acquis-b1-ttl,
Acquis-b2-ttl,
Acquis-b3-ttl,
JRC-b1,
JRC-b2,
JRC-noi-b1,
JRC-noi-b2,
JRC-noi-b3

**News**: document ids:
Agenda-1-300,
Agenda-b1,
Agenda-b2,
Agenda-b3

**Fiction**: document ids:
1984Orwell-b1-ttl,
1984Orwell-b2-ttl,
1984Orwell-b3-ttl,
1984Orwell-b4-ttl,
Literatura-1-300,
Literatura-b1,
Literatura-b2,
Literatura-noi-b1

**Medical**: document ids:
EMEA-b1,
EMEA-b2,
EMEA-b3,
EMEA-noi-b1,
Medical-1,
Medical-2

**Nonfiction**: document ids:
PhysicsCompSciMath

**Academic**: document ids:
DGLR-1-300,
DGLR-b1,
DGLR-b2,
DGLR-b3,
DGLR-noi-b1

**FrameNet**: document ids:
FrameNet-b1,
FrameNet-b2,
FrameNet-b3,
FrameNet-b4

**Wikipedia**: document ids:
Wikipedia-2-FirstUDRelease,
Wikipedia-b1,
Wikipedia-b2

**Miscellanea**: document ids:
DTLR-b1,
DTLR-b2,
DTLR-b3,
FirstUDRelease-ICIA,
FirstUDRelease-UAIC

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

Verginica Barbu Mititelu, “Modern Syntactic Analysis of Romanian”. In Ofelia Ichim, Luminiţa Botoşineanu, Daniela Butnaru, Marius-Radu Clim, Ofelia Ichim, Veronica Olariu (eds.), Clasic şi modern în cercetarea filologică românească actuală, Iaşi, Publishing House of "Alexandru Ioan Cuza" University, 2018, pp. 67-78.

For RACAI-RoTb:
Elena Irimia, Verginica Barbu Mititelu, RACAI-RoTb: nucleu de corpus de limbă română adnotat sintactic cu relaţii de dependenţă, Revista Română de Interacţiune Om-Calculator 8 (2) 2015, p. 101-120.

For UAIC-RoTb:
Cenel Augusto Perez. 2014. Linguistic Resources for Natural Language Processing. (PhD thesis). Faculty of Computer Science, Al. I. Cuza University, Iasi.


# CHANGELOG

- UD 1.2 --> 1.3: the number of trees was considerably increased.
- UD 1.3 --> 1.4:
- increase the treebank size to 9523 sentences;
- identical sentences (disregarding punctuation and numbers) at word form level have been removed;
- added a scientific (Physics, Mathematics and Computer Science) sub-corpus to make up for the loss;
- removed all words with underscores;
- removed most of the errors reported by the content validation tool;
- extensive POS-tagging and lemmatization corrections;
- ensuring more consistent data at the lexical, morphological and syntactic levels.
- UD 1.4 --> 2.0:
- manual improvements of the annotation, concerning POS-tagging, syntactic labeling, one sentence split.
- automatic conversion to UDv2 guidelines using Udapi (http://udapi.github.io/) ud.Convert1to2
- automatic reconstruction of original texts (ud.ro.SetSpaceAfter), pseudo-documents marked with newdoc markup
- re-split: train=185,113 (84.7%) tokens, dev=17,074 (7.8%) tokens, dev=16,324 (7.5%) tokens. Each pseudo-document equally distributed into train/dev/test.
- test set omitted from the UDv2.0 official release because of CoNLL 2017 shared task.
- UD 2.0 --> 2.1: no modifications to the previous version.
- UD 2.1 --> 2.2: repository renamed from UD_Romanian to UD_Romanian-RRT
- UD 2.6 --> 2.7: manual improvement of the annotations, concerning POS-tagging, syntactic labeling
- UD 2.7 --> 2.8: automatic (then manually checked) improved POS-tagging, mainly for numerals and auxiliaries; some automatic dependency relation corrections (`obl` for nouns headed by verbs, `nsubj:pass` for subjects of passive constructions).  Correction scripts are in GitHub at [ro-ud-autocorrect](https://github.com/racai-ai/ro-ud-autocorrect).
- UD 2.8 --> 2.9: solving the verbal homography between present and past simple, the pronominal homonymy between dativ singular and accusative plural, the nominal homonymy between singular oblique cases and all cases in the plural; consistent use of the obl and nmod relations according to the guidelines.

<pre>
=== Machine-readable metadata =================================================
Data available since: UD v1.2
License: CC BY-SA 4.0
Includes text: yes
Genre: wiki legal news fiction medical nonfiction academic
Lemmas: automatic
UPOS: converted with corrections
XPOS: automatic
Features: converted with corrections
Relations: manual native
Contributors: Barbu Mititelu, Verginica; Irimia, Elena; Perez, Cenel-Augusto; Ion, Radu; Simionescu, Radu; Popel, Martin
Contributing: elsewhere
Contact: vergi@racai.ro
===============================================================================
</pre>
