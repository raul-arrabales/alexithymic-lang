# The Alexithymic Language Project
## A Psicobōtica Labs research project on discovering patterns in alexithymic discourse.
Raúl Arrabales Moreno (raul@psicobotica.com) / Sept. 2020 / Psicobōtica Labs.

**Abstract:**
1. We asked adult participants to describe what they see in several, rather ambiguous, visual stimuli. 
2. We estimated the degree of alexithymia (difficulty to identify emotions) of the same participants using a standarized test. 
3. In this project, we analyse the narratives provided by the participants, looking for specific patterns in those with the highest degree of alexithymia. 

<hr>

Most of the code is **also designed to serve as educational resource for junior data scientists**, and it's being used at different introductory courses on Natural Language Processing (NLP) and Natural Language Understanding (NLU). 

<hr>

**Context information:**
- [What is alexithymia](https://www.psicobotica.com/en/2020/06/08/alexithymia-when-i-dont-realize-how-i-feel/).
- [Data collection via citizen science projects](https://www.psicobotica.com/en/2020/06/11/get-involved-in-our-research-projects/).
- [Prolexitim NLP](https://psicobotica.com/prolexitim/nlp/index.html). The tool used to present the visual stimuli. 
- [Prolexitim TAS-20](https://psicobotica.com/prolexitim/tas-20-spain/). The tool used to measure the level of alexithymia. 
<hr>

### NLP/NLU Analytics Pipeline
This project is intended to contain a fairly complete end to end pipeline, representing some of the most popular techniques applied when dealing with natural language in written form. Here is a summary of the main tasks that we perform using the python code included in this project: 

- 0. Research design and problem modeling. 
- 1. Loading dataset and exploratory analysis. 
- 2. Variables transformation according to the research design. 
- 3. NLP Pre-processing: Tokenization. 
- 4. NLP Pre-processing: Stemming. 
- 5. NLP Pre-processing: PoS (Part of Speech) Tagging. 
- 6. NLP Pre-processing: NER (Named Entity Recognition) Tagging. 
- 7. NLP Pre-processing: DEP (syntactic Dependencies) Tagging.
- 8. NLP Frequency-Based Feature Engineering: frequencies, diversity scores.
- 9. NLP Bag of Words (BoW) Frequency Space Feature Engineering. 
- 10. NLP Latent Space Feature Engineering (embeddings): Word2Vec, Doc2Vec. 
- 11. NLP Processing: Topic Detection (LDA). 
- 12. NLP Processing: Sentiment Analysis (Lexicon-based, model-based). 
- 13. NLP Processing: 


<hr>

### Data folder
This folder contains the original dataset obtained from the Prolexitim project as well as newly generated datasets with additional processing and features.

The main information provided by the original dataset consists of rows representing: 
- Anonymous code of participant. 
- Degree of alexithymia of that participant (measured using the TAS-20 instrument). 
- Identification of a visual stimulus (an ambiguous picture taken from the Thematic Apperception Test (TAT) card set). 
- The original Spanish text corresponding to the narrative reported by the participant when presented with the visual stimulus.

The specific description of the variables represented in the CSV files can be found in [data folder's readme](https://github.com/raul-arrabales/alexithymic-lang/blob/master/data/README.md).
Note that multiple features have been obtained from the original documents (original raw text field) and included as additional columns in tabular dataset files. 

### Lexicon folder
This folder contains Spanish lexicon datasets:
- Sentiment analysis lexicons.

### NLP folder
This folder contains the interactive notebooks (ipynb) used for data analysis: 
- **1-Preprocessing.ipynb**: prolexitim dataset exploration, class variable definition and standard NLP processing (tokenization, stemming, lemmatization, POS, NER, DEP, etc.). 
- **1b-SA-Lexicons.ipynb**: preparation of Sentiment Analysis lexicons in Spanish. 
- **2-Features.ipynb**: standard natural language feature engineering (counts, lengths, frequencies, diversity scores, etc.). 
- **Embeddings_USEM.ipynb**: latent space feature engineering (embeddings) using Google's [Universal Sentence Encoder - Multilingual L3](https://tfhub.dev/google/universal-sentence-encoder-multilingual-large/3).
- **Embeddings_S3B.ipynb**: latent space feature engineering (embeddings) using [Spanish 3B Word2Vec Embedding](https://github.com/aitoralmeida/spanish_word2vec).

### Models folder 
This folder contains both pre-trained models from third party contributors and models trained with our own data. 
- Stanford NER tagger model - Spanish. [Stanford Entity Recognizer](https://nlp.stanford.edu/software/CRF-NER.html).
- Stanford POS tagger model - Spanish. [Stanford POS Tagger](https://nlp.stanford.edu/software/tagger.shtml).
- Other Stanford CoreNLP models (Spanish). [Stanford CoreNLP](https://stanfordnlp.github.io/CoreNLP/).
- Word BoW Model. 
- Stem BoW Model. 


