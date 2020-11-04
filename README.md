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
- 3. Pre-processing: Tokenization. 
- 4. Pre-processing: Stemming. 
- 5. Pre-processing: PoS (Part of Speech) Tagging. 
- 6. Pre-processing: NER (Named Entity Recognition) Tagging. 
- 7. Pre-processing: DEP (syntactic Dependencies) Tagging.
- 8. Frequency-Based Feature Engineering: frequencies, diversity scores.
- 9. Bag of Words (BoW) Vector Space Feature Engineering. 
- 10. TF/IDF Vector Space Feature Engineering. 
- 11. N-Grams models and text generation. 
- 12. PoS tokens counts. Most frequent verbs, nouns, adjectives, etc. per class.
- 13. Inferring personality traits, needs, values and preferences. 
- 14. Sentiment analysis (polarity, intensity, etc.).
- 15. Topic Detection with Latent Semantic Analysis (LSA). 
- 16. Topic Detection with Latent Dirichlet Allocation (LDA). 
- 17. Word2Vec embedding training using CBoW and Skip Gram. 
- 18. Doc2Vec generation using a pre-trained Word2Vec model (Spanish 3B). 
- 19. Doc2Vec using a pre-trained sentence encoder.


<hr>

### HTML folder
This folder contains HTML versions of the iPython notebooks (Jupyter exported) for quick inspection and visualization.


### Data folder
This folder contains the original dataset obtained from the Prolexitim project as well as newly generated datasets with additional processing and features.

The main information provided by the original dataset consists of rows representing: 
- Anonymous code of participant. 
- Degree of alexithymia of that participant (measured using the TAS-20 instrument). 
- Identification of a visual stimulus (an ambiguous picture taken from the Thematic Apperception Test (TAT) card set). 
- The original Spanish text corresponding to the narrative reported by the participant when presented with the visual stimulus.

The specific description of the variables represented in the CSV files can be found in [data folder's readme](https://github.com/raul-arrabales/alexithymic-lang/blob/master/data/README.md).
Note that multiple features have been obtained from the original documents (original raw text field) and included as additional columns in tabular dataset files. 

[Here is the description of all variables contained in generated datasets](https://github.com/raul-arrabales/alexithymic-lang/blob/master/data/README.md).

### Lexicon folder
This folder contains Spanish lexicon datasets:
- Sentiment analysis lexicons.

### NLP folder
This folder contains the interactive notebooks (ipynb) used for data analysis: 
- **1-Preprocessing.ipynb**: prolexitim dataset exploration, class variable definition and standard NLP processing (tokenization, stemming, lemmatization, POS, NER, DEP, etc.). 
- **1b_SA-Lexicons.ipynb**: preparation of Sentiment Analysis lexicons in Spanish. 
- **2_Features.ipynb**: standard natural language feature engineering (counts, lengths, frequencies, diversity scores, etc.). 
- **3_BoW.ipynb**: words and stems Bag of Word models. BoW Vector space model dimensionality reduction (PCA and t-SNE).
- **3b_TF-IDF.ipynb**: words and stems TF/IDF models. TF/IDF Vector space model dimensionality reduction (PCA and t-SNE).
- **3c_N-Grams.ipynb**: chars and words N-Gram models. N-Gram based text generation. 
- **4_Lexicosemantics.ipynb**: PoS frequency in different classes. Semantic analysis. 
- **5_Personality.ipynb**: Use of the Personality Insights API (IBM Cloud) to annotate text with personality variables. 
- **6_Sentiment.ipynb**: Sentiment analysis using different techniques (lexicon-based, third-party API, etc.). 
- **7_SemanticAnalysis.ipynb**: Latent Semantic Analysis LSA (topic detection). 
- **8_LatentDirichletAllocation.ipynb**: Latent Dirichlet Allocation LDA (topic detection). 
- **9_Word2Vec.ipynb**: Traning neural vector models with our dataset (CBoW and Skip Gram). 
- **9b_Word2Vec_S3B.ipynb**: Using a pre-trained neural vector model, build Doc2Vec and other embedding features. 
- **10_Embeddings_USEM.ipynb**: Doc2Vec using Google's Universal Sentence Encoder - Multilingual L3.

### Models folder 
This folder contains both pre-trained models from third party contributors and models trained with our own data. 
- Stanford NER tagger model - Spanish. [Stanford Entity Recognizer](https://nlp.stanford.edu/software/CRF-NER.html).
- Stanford POS tagger model - Spanish. [Stanford POS Tagger](https://nlp.stanford.edu/software/tagger.shtml).
- Other Stanford CoreNLP models (Spanish). [Stanford CoreNLP](https://stanfordnlp.github.io/CoreNLP/).
- Word BoW Model. 
- Stem BoW Model. 
- Char-Based N-Gram (n=6) models.
- Word-Based N-Gram (n=3, trigrams) models.
- Word2Vec models. 
- Doc2Vec models. 

[Here is the list of all models](https://github.com/raul-arrabales/alexithymic-lang/blob/master/models/README.md).



