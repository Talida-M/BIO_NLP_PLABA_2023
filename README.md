# BIO_NLP_PLABA_2023
https://bionlp.nlm.nih.gov/plaba2023/#
## Task
The task is to adapt biomedical abstracts to for the general public using plain language. Given a set of abstracts (the source), your system will provide output for each sentence of the source. When adapting, source sentences may be split, in which case the output for one source sentence will be multiple target sentences, or omitted, in which case the output for a source sentence will be blank. However, source sentences may not be merged, and the output for a given source sentence should not contain information from other source sentences. Both source and output will be in English. Source abstracts have been retrieved to answer consumer questions asked on MedlinePlus. These questions will be used for to guide manual evaluation (see Evaluation). Teams will have access to the questions and may provide Systems with them desired.

- For each of 40 consumer questions:
    - Input: A text file containing the consumer question used to retrieve abstracts, on one line
    - For each of 10 abstracts retrieved to answer the consumer question:
        - Input: A text file with one line per sentence of the abstract
        - Output: A text file with one line per source sentence. These lines may be blank (to omit the source sentence) or contain multiple sentences (to split the source sentence)

## Data
https://bionlp.nlm.nih.gov/plaba2023/#data\
Training data are the publicly available PLABA dataset (Attal 2023), which comprises 750 abstracts, each manually adapted to plain language by at least one annotator, for a total of 7,643 sentence pairs.
Notable guidelines include:
Split complex sentences. Each source sentence can have any number of target sentences.
Substitute medical jargon with common alternatives, e.g. orthoses with braces.
Explain terms with no substitutes when introduced, e.g. "Duloxetine (a common antidepressant)."


@Emil: research on related work (SOTA), report 

@Andrei: finetune-mistral research

@Andreiana: presentation

@Talida: prompting/summarization, 

Up for grabs: preparing dataset for finetuning, metrics (SARI, BLEU, ROUGE)
