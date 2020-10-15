## Datasets 

**Prolexitim Original Dataset V2 (Prolexitim_v2.csv):**

- **Code:** Anonymous unique code of each user. 
- **TAS20:** TAS-20 global score.
- **F1:** F1 factor of TAS-20: Difficulty identifying feelings.
- **F2:** F2 factor of TAS-20: Difficulty describing feelings.
- **F3:** F3 factor of TAS-20: Externally orientated style of thinking.
- **Gender:** Participant's gender. 
- **Age:** Participant's age. 
- **Card:** TAT card used as visual stimulus for the narrative. 
- **Text:** Raw text in Spanish as inputed by the user (form instructions removed).

**Class/Target Variables (Prolexitim_v2_processed.csv):**

- **Alex_A:** Dichotomous variable (0/1) indicating the presence of alexithymia according to criterion A (TAS-20 >= 61). 
- **Alex_B:** Dichotomous variable (0/1) indicating the presence of alexithymia according to criterion A (TAS-20 >= 56). 

**Manually Annotated Variables (Prolexitim_v2_tagged.csv):**
- **T_Metaphors:** Use of metaphorical language. 
- **T_ToM:** Signs of Theory of Mind. 
- **T_FP:** First-Person narrative.
- **T_Interpret:** Imaginative interpretation of the situation.
- **T_Desc:** Objective description of the situation without any interpretation.
- **T_Confussion:** Express confussion or disorientation.

**Text Preprocessing Dataset Variables (Prolexitim_v2_processed.csv):**
- **Words:** Number of words in the Text.
- **Sentences:** Number of sentences in the Text (dot separated).
- **Tokens:** List of tokens extracted from the Text (RegexpTokenizer(r'\w+')).
- **Tokens_Stop:** List of tokens without the Spanish stop words.
- **Tokens_Stem:** List of word stems, extracted from Tokens_Stop.
- **POS:** Part of Speech (POS) tagging (list of pairs (word, POS tag)).
- **NER:** Named Entity Recognition (NER) tagging (list of pairs (word, NER tag)).
- **DEP:** Lexical and dependency parsing tags (list of tuples ((word, POS tag), DEP tag, (word, POS tag))).

**Language Feature Engineering Variables (Prolexitim_v2_features-2.csv):**
- **Chars**: Number of characters in the Text.
- **avgWL**: Average word length in the Text.
- **avgSL**: Average sentence length in the Text.
- **Pun_Count**: Number of punctuation signs in the Text.
- **Stop_Count**: Number of stop words in the Text.
- **Tittle_Count**: Number of words starting with a capital letter in the Text.
- **Upper_Count**: Number of capitalized chars in the Text.
- **VERB_Count**: Number of verbs in the Text.
- **NOUN_Count**: Number of nouns in the Text.
- **SYM_Count**: Number of symbols in the Text.
- **ADV_Count**: Number of adverbs in the Text.
- **PUNCT_Count**: Number of punctuation in the Text.
- **INTJ_Count**: Number of interjections in the Text.
- **CCONJ_Count**: Number of coordination conjunctions in the Text.
- **ADJ_Count**: Number of adjectives in the Text.
- **AUX_Count**: Number of auxiliaries in the Text.
- **DET_Count**: Number of determiners in the Text.
- **SCONJ_Count**: Number of subordinating conjunctions in the Text.
- **PRON_Count**: Number of pronouns in the Text.
- **NUM_Count**: Number of numerals in the Text.
- **PROPN_Count**: Number of propper nouns in the Text.
- **ADP_Count**: Number of adpositions in the Text.
- **VERB_Ratio**: Proportion of verbs in the Text.
- **NOUN_Ratio**: Proportion of nouns in the Text.
- **SYM_Ratio**: Proportion of symbols in the Text.
- **ADV_Ratio**:  Proportion of adverbs in the Text.
- **PUNCT_Ratio**: Proportion of punctuation in the Text.
- **INTJ_Ratio**: Proportion of interjections in the Text.
- **CCONJ_Ratio**: Proportion of coordination conjunctions in the Text.
- **ADJ_Ratio**: Proportion of adjectives in the Text.
- **AUX_Ratio**: Proportion of auxiliaries in the Text.
- **DET_Ratio**: Proportion of determiners in the Text.
- **SCONJ_Ratio**: Proportion of subordinating conjunctions in the Text.
- **PRON_Ratio**: Proportion of pronouns in the Text.
- **NUM_Ratio**: Proportion of numerals in the Text.
- **PROPN_Ratio**: Proportion of propper nouns in the Text.
- **ADP_Ratio**: Proportion of adpositions in the Text.
- **TTR**: Type Token Ratio. Total number of unique word types used in the text divided by the total number of words.
- **HTR**: Hapax legomena/Token ratio. The number of words that occur only once divided by the number of total words.

**Language Feature Engineering Variables - BoW (Bag of Words) (Prolexitim_v2_features-3.csv):**
- **BoW_PCA_1**: Principal Component 1 BoW Vector.
- **BoW_PCA_2**: Principal Component 2 BoW Vector.
- **BoW_PCA_3**: Principal Component 3 BoW Vector.
- **TFIDF_PCA_1**: Principal Component 1 TF/IDF Vector.
- **TFIDF_PCA_2**: Principal Component 2 TF/IDF Vector.
- **TFIDF_PCA_3**: Principal Component 3 TF/IDF Vector.

**Lexical Semantics Analysis (Prolexitim_v2_features-4.csv):**
- **Verb_List**: List of verbs in the text in order of appearance.
- **Noun_List**: List of nouns in the text in order of appearance.
- **Adjective_List**: List of adjectives in the text in order of appearance.
- **Subord_List**: List of subordinate conjunctions in the text in order of appearance.
- **Adverb_List**: List of adverbs in the text in order of appearance.
- **Aux_List**: List of auxiliary verbs in the text in order of appearance.



