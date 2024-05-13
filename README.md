<h2>Custom entities extraction: lexicon-based approach vs GPT-4</h2>

This repository contains the Python Notebooks and the data used for a project aimed to demonstrate that GPT-4 outperforms traditional lexicon-based knowledge extraction approaches.

We consider the case of extracting customer needs and user categories from software reviews, collected on Play Store and App Store. The needs are identified through System Quality Attributes. The scripts are Python Notebooks.
The first utilizes lexicons to extract needs and users from a test set of 1050 software reviews. Then, GPT-4 is employed through OpenAI's APIs and few-shot prompting, to perform the same task. The testset has been manually
annotate by the authors. In the evaluation notebook, the results obtained with the two approaches are evaluated by comparing the identified entities with the manual labeling and calculating the following metrics:
BERTScore (Precision, Recall, F-1), ROUGE-1, ROUGE-2, ROUGE-L, and BLEW. The comparative analysis shows that GPT-4 outperforms the lexicon approach in both needs (the BERTScore F-1 is 0.73 for GPT-4 against 0.45 of lexicon)
and user extraction (0.25 against 0.04).
