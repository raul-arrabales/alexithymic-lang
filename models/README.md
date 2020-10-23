## Alexithymic Language Project 
### Trained models

**BoW Models:**
- **Prolexitim_v2_Standard_BoW.csv**: Word-based Bag of Words vectors. 
- **Prolexitim_v2_Stem_BoW.csv**: Stem-based Bag of Words vectors. 

**TF/IDF Models:**
- **Prolexitim_v2_TFIDF.csv**: Term-Frequency / Inversed Document Frequency vectors. 

**N-Gram based Models:**
- **Prolexitim_v2_CharNGram_Alex.json**: Char-based N-Gram model for alexithymic discourse (n=6). 
- **Prolexitim_v2_CharNGram_NoAlex.json**: Char-based N-Gram model for non-alexithymic discourse (n=6). 
- **Prolexitim_v2_WordNGram_Alex.json**: Word-based N-Gram model for alexithymic discourse (n=3). 
- **Prolexitim_v2_WordNGram_NoAlex.json**: Word-based N-Gram model for non-alexithymic discourse (n=3).

**Stanford pre-trained models:**
- **spanish-postagger.tagger**: Stanford Part-of-Speech Tagger for Spanish. 
- **stanford-ner.jar**: Stanford Spanish Named Entity Recognition model. 
- **spanish.ancora.distsim.s512.crf.ser.gz**: Spanish data from the AnCora corpus.

**Word2Vec models (trained with our dataset):**
- **Word2Vex_CBOW_Prolex_v2**: Word2Vec embeddings trained using CBoW (bin and model formats). 
- **Word2Vex_SGram_Prolex_v2**: Word2Vec embeddings trained using Skip Gram (bin and model formats). 

**Latent Space (embeddings) Variables (Prolexitim_v2_features-embed-XXX.csv):**
- **Embed_USEM**: 512 dimensions embedding calculated with Google Universal Sentence Enconder - Multilingual Large 3.
- **Embed_3B_Mean**: 400 dimensions embedding calculated as the mean of all word vectors (Spanish 3B).
