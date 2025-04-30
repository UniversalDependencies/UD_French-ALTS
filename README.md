# Summary

ALTS (AUTOMATED Sixteenth-century corpus) is a treebank of sixteenth-century legal French. Currently in contains one text, trial accounts from Guernsey Greffe (register Crime I), transcribed directly from the manuscript and manually annotated in PoS, lemmata and syntactic functions. The text presents dialectal Norman features and forms.


# Introduction

This text of Guernsey Crime I  (1,269 sentences; 45,101 tokens) was first annotated in PoS, lemmatised and automatically parsed as part of the Franco-German [MICLE project](https://www.unicaen.fr/projet_de_recherche/micle/) (2021-2024) led by Professor Pierre Larrivée (University of Caen) and Professor Cecilia Poletto (University of Frankfurt). Earlier versions of the text, annotated with [HT-CRISCO workflow](https://github.com/Corpus-Diachroniques-CRISCO/HT-CRISCO) incorporating the use of [HOPS parser](https://github.com/hopsparser/hopsparser), can be consulted on [CRISCO Lab's TXM server](https://txm-crisco.huma-num.fr/txm/) and via the [website](https://criscoht.unicaen.fr/).  

As part of [AUTOMATED project](https://www.unicaen.fr/projet_de_recherche/automated/) the text was reannotated with [BertForDeprel](https://github.com/kirianguiller/BertForDeprel) parser and manually corrected using bootstrapping methodology ([Peng et al 2022](https://hal.science/hal-03846834v1)) on [ArboratorGrew](https://arborator.grew.fr/#/) software.

| Set               | Sentences| Tokens    |
| :---------------- | :------: | ----:     |
| Train             |   811    |   30,140  |
| Dev               |   111    |   4,575   |
| Test              |   347    |   10,386  |
| **Total**         | **1,269**| **45,101**|



# Acknowledgments

This work was made possible thanks to the generous support of the ANR-DFG Franco-German scheme ([MICLE project](https://www.unicaen.fr/projet_de_recherche/micle/) (2021-2024)) and of the Normandy region [AUTOMATED project](https://www.unicaen.fr/projet_de_recherche/automated/) (2023-2025).

We would like to thank the staff at the Guernsey Greffe archives and the Guernsey Museum & Art Gallery for giving us acces to the manuscript and digital images in 2021 and 2023. We are also grateful to former island archivist Daryl Ogier for his assistance and advice when working with the original source. We are grateful to the team of student transcribers (Agathe Aubert, Lucie Marie-Leblanc, Marie Picart and Valentin Simenel) who helped with the transcription in 2022. We thank Patrice Lajoye and Stéphane Laîné for their assistance with lemmatisation and dialectal features of the text and to Mattis Le Scaer who helped elucidate the historical context of the document.

Annotation was performed by Natasha Romanova, technical assistance by Rayan Ziane and Khensa Daoudi.

## References

* **(Ziane & Romanova 2024)** [Pistes pour l’optimisation de modèles de parsing syntaxique.](https://lift2-2024.sciencesconf.org/590561/document) LIFT 2 - 2024 : Journées de lancement, Nov 2024, Orléans, France. 


# Changelog

* 2025-05-15 v2.16
  * Initial release in Universal Dependencies.


<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.16
License: CC BY-SA 4.0
Includes text: yes
Genre: legal
Lemmas: manual native
UPOS: manual native
XPOS: not available
Features: manual native
Relations: manual native
Contributors: Romanova, Natasha
Contributing: here
Contact: natalia.romanova@unicaen.fr
===============================================================================
</pre>
