# EvidenceOutcomes: a Dataset of Clinical Trial Publications with Clinically Meaningful Outcomes

## Purpose

The fundamental process of evidence extraction and synthesis in the practice of evidence-based medicine involves extracting PICO (Population, Intervention, Comparison, and Outcome) elements from biomedical literature. However, Outcomes, being the most complex elements, are often overlooked or neglected. To address this issue, we developed a robust annotation guideline for extracting clinically meaningful outcomes from text through iteration and discussion with clinicians and Natural Language Processing experts. 

Three independent annotators annotated the Results and Conclusions sections of a randomly selected sample of 500 PubMed abstracts and additional 140 PubMed abstracts from the existing EBM-NLP corpus. This resulted in a dataset, EvidenceOutcomes, with high-quality annotations of an inter-rater agreement of 0.76.


## Data

* A finalized annotation guideline for identifying outcome elements (O in PICO framework) in randomized controlled trial abstracts from PubMed ('Annotation Guideline Finalized.pdf') and 
* A corpus of 640 randomized controlled trial abstracts from two corpora (500 RCT abstracts randomly selected and 140 RCT abstracts selected from the existing EBM-NLP corpus (https://github.com/bepnye/EBM-NLP)) that have been annotated per the annotation guideline by one primary annotator and two secondary annotators. The primary annotator and a secondary annotator reached a consensus on annotation for each of the abstracts. 
  * A zipped consensus folder of all 640 abstract that contains both the abstract document (`*.txt`) and the outcome annotations using the platform Brat (http://brat.nlplab.org/) in `.ann` format ('consensus.tar.gz').
  * For ease of use, abstracts from the two corpora are provided in CoNLL format as well  (`500RCT-CoNLL.tsv` and `140EBMNLP-CoNLL.tsv`).

## Acknowledgment

This project was sponsored by the National Library of Medicine grant R01LM009886 and the National Center for Advancing Clinical and Translational Science award UL1TR001873.

## License

Copyright (c) 2023 Weng Lab at Columbia University

Distributed under the terms of the [MIT](https://github.com/bionlplab/medtext/blob/master/LICENSE) license, 
EvidenceOutcomes is free and open-source.
