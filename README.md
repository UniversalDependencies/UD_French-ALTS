# Summary

ALTS (AUTOMATED Sixteenth-century corpus) is a treebank of sixteenth-century legal French from Normandy and the Channel Islands.

Currently it contains two texts: 1) trial accounts from Guernsey Greffe (register _Crime I_), transcribed directly from the manuscript (**1563-1569_Guern**) and 2) an extract from Book 9 of Guillaume Terrien's _Commentaires du droict civil tant public que privé observé au pays et duché de Normandie_ digitised from the original printed book (**1578_Terrien**). The text of 1563-1569_Guern presents many dialectal Norman features and forms. The text of 1578_Terrien has some Latin words and expressions.


# Introduction


**1563-1569_Guern**

This text contains accounts of fifteen court cases on the island on Guernsey from 1563 to 1569 (witchcraft, piratry, infanticide etc). The text was transcribed in full from the original manuscript Guernsey Greffe _Crime I_, abbreviations were expanded. In the treebank, sentences from this text have the prefix 1563-1569_Guern.

**1578_Terrien**

This text contains passages authored by Guillaume Terrien himself (and not quotations from earlier legal texts) from Book 9 "Style de procédure"
from the sixteenth-century printed book Guillaume Terrien (1568). _Commentaires du droict civil tant public que privé observé au pays et duché de Normandie_, 2nd edition, Paris: Jacques du Puy, pp. 339-402. The spelling and word segmentation of the original, including abbreviated words (e.g. "glo." for "glose"), have been retained. Only abbreviations for "m" and "n" (eg. "o with a tilda" for "om" or "on" and "&" for "et" have been expanded. In the treebank, sentences from this text have the prefix 1578_Terrien.

Sentences written completely in Latin were excluded. If Latin words occur in French sentences, the token contains the tag Lang=la and is lemmatised with a Latin lemma.

**Sentence and token number per text**

| Text              | Sentences| Tokens    |
| :---------------- | :------: | ----:     |
| 1563-1569_Guern   |   1,269  |  45,101   |
| 1578_Terrien      |   757    |  25,113   |
| **Total**         | **2,026**| **70,114**|

**Annotation**

The texts were first annotated in PoS, lemmatised and automatically parsed as part of the Franco-German [MICLE project](https://www.unicaen.fr/projet_de_recherche/micle/) (2021-2024) led by Professor Pierre Larrivée (University of Caen) and Professor Cecilia Poletto (University of Frankfurt). Earlier versions of the texts, annotated with [HT-CRISCO workflow](https://github.com/Corpus-Diachroniques-CRISCO/HT-CRISCO) incorporating the use of [HOPS parser](https://github.com/hopsparser/hopsparser), can be consulted on [CRISCO Lab's TXM server](https://txm-crisco.huma-num.fr/txm/) and via the [website](https://criscoht.unicaen.fr/).

As part of [AUTOMATED project](https://www.unicaen.fr/projet_de_recherche/automated/) the texts were reannotated with [BertForDeprel](https://github.com/kirianguiller/BertForDeprel) parser and manually corrected using bootstrapping methodology ([Peng et al 2022](https://hal.science/hal-03846834v1)) on [ArboratorGrew](https://arborator.grew.fr/#/) software.

Verbs and auxiliaries are annotated in verb forms (VerbForm): Inf (infinitive), Fin (conjugated) and Part (participle). In 1568_Terrien, congujated verbs and auxiliaries are annotated in Person and Number.

Pronouns are annotated in type (PronType: Dem for demonstrative, Ind for indefinite, Int for interrogative, Prs for personal and Rel for relative). Reflexive and possessive pronouns are also tagged (Reflexive=Yes and Poss=Yes).

Determiners are annotated using PronType feature (Art for articles, Dem for demonstratives, Ind for indefinite). Possessive determiners have are annotated Poss=Yes.

The treebank is lemmatised using modern French lemmata and, wherever approriate, using lemmata from ([Dictionnaire du Moyen Français](http://zeus.atilf.fr/dmf/)).

**Train/Dev/Test split**

| Set               | Sentences| Tokens    |
| :---------------- | :------: | ----:     |
| Train             |   1202   |   43,389  |
| Dev               |   154    |   6,024   |
| Test              |   670    |   20,701  |
| **Total**         | **2,026**| **70,114**|


Please note that French-ALTS treebank is still under development and will be undergoing campains of correction. Annotation will be revised and expanded. Please do not hesitate to contact us is you have any questions, suggestions or comments.

# Acknowledgments

This work was made possible thanks to the generous support of the ANR-DFG Franco-German scheme ([MICLE project](https://www.unicaen.fr/projet_de_recherche/micle/) (2021-2024)) and of the Normandy region [AUTOMATED project](https://www.unicaen.fr/projet_de_recherche/automated/) (2023-2025).

**1563-1569_Guern**

We would like to thank the staff at the Guernsey Greffe archives and the Guernsey Museum & Art Gallery for giving us acces to the original manuscript and digital images in 2021 and 2023 which. We are also grateful to former island archivist Daryl Ogier for his assistance and advice when working with the original source. We are grateful to the team of student transcribers (Agathe Aubert, Lucie Marie-Leblanc, Marie Picart and Valentin Simenel) who helped with the transcription in 2022. We thank Patrice Lajoye and Stéphane Laîné for their assistance with lemmatisation and dialectal features of the text and to Mattis Le Squer who helped elucidate the historical context of the document. The annotation of 1563-1569_Guern has not been revised since UD 2.16 release. Annotation was performed by Natasha Romanova and Rayan Ziane, technical assistance by Khensa Daoudi.

**1578_Terrien**
The digitisation of Guillaume Terrien's _Commentaires du droict civil tant public que privé observé au pays et duché de Normandie_ was originally performed by Morgane Pica and Mathieu Goux as part of the [ConDE](https://mrsh.unicaen.fr/coutumiers/conde/accueil.html) project funded by Normandy region. PoS annotation and lemmatisation was performed by Natasha Romanova. Annotation in syntactic functions was done by Théo Brillet and Natasha Romanova. Théo Brillet annotated all the sentences with Latin tokens. Khensa Daoudi and Rayan Ziane provided technical assistance.


## References

* Ziane, Rayan & Romanova, Natasha, 2024. « Pistes pour l’optimisation de modèles de parsing syntaxique » _Proceedings of LIFT 2 - 2024 : Journées de lancement_. 14-15 Nov 2024, Orléans, France. https://lift2-2024.sciencesconf.org/590561/document (7 pp.)

See also:
* **Daoudi, Khensa, Dehouck, Mathieu, Romanova, Natasha & Ziane, Rayan, 2025. « Explicit Edge Length Coding to Improve Long Sentence Parsing Performance ». _Proceedings of the First Workshops on Advancing NLP for Low-Resource Languages_. 13 September 2025, Varna, Bulgaria. URL: https://acl-bg.org/proceedings/2025/LowResNLP%202025/index.html (pp. 102-110)

# Changelog

* 2025-05-15 v2.16
  * Initial release in Universal Dependencies.


<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.16
License: CC BY-SA 4.0
Includes text: yes
Parallel: no
Genre: legal
Lemmas: manual native
UPOS: manual native
XPOS: not available
Features: manual native
Relations: manual native
Contributors: Romanova, Natalia; Ziane, Rayan; Daoudi, Khensa
Contributing: here
Contact: natalia.romanova@unicaen.fr
===============================================================================
</pre>
