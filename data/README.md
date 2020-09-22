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



**Language Feature Engineering Variables:**
- **sdfs**: sdfsdf.

**Latent Space (embeddings) Variables:**
- **dfs**: sdfsd.




