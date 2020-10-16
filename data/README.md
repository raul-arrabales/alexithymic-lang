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

**Personality Analysis (Prolexitim_v2_features-5.csv):**
- **IBM Personality Insights variables**: 95 variables related to personality traits, needs, values and preferences:
- 'big5_openness'
-- 'facet_adventurousness'
-- 'facet_artistic_interests'
-- 'facet_emotionality'
-- 'facet_imagination'
-- 'facet_intellect'
-- 'facet_liberalism'
- 'big5_conscientiousness'
-- 'facet_achievement_striving'
-- 'facet_cautiousness'
-- 'facet_dutifulness'
-- 'facet_orderliness'
-- 'facet_self_discipline'
-- 'facet_self_efficacy'
- 'big5_extraversion'
-- 'facet_activity_level'
-- 'facet_assertiveness'
-- 'facet_cheerfulness'
-- 'facet_excitement_seeking'
-- 'facet_friendliness'
-- 'facet_gregariousness'
- 'big5_agreeableness'
-- 'facet_altruism',
-- 'facet_cooperation'
-- 'facet_modesty'
-- 'facet_morality'
-- 'facet_sympathy'
-- 'facet_trust'
- 'big5_neuroticism'
-- 'facet_anger'
-- 'facet_anxiety'
-- 'facet_depression'
-- 'facet_immoderation'
-- 'facet_self_consciousness'
-- 'facet_vulnerability'
- Needs:
-- 'need_challenge'
-- 'need_closeness'
-- 'need_curiosity'
-- 'need_excitement'
-- 'need_harmony'
-- 'need_ideal'
-- 'need_liberty'
-- 'need_love'
-- 'need_practicality'
-- 'need_self_expression'
-- 'need_stability'
-- 'need_structure',
- Values:
-- 'value_conservation'
-- 'value_openness_to_change'
-- 'value_hedonism'
-- 'value_self_enhancement'
-- 'value_self_transcendence'
- Consumption preferences:
-- 'consumption_preferences_automobile_ownership_cost'
-- 'consumption_preferences_automobile_safety'
-- 'consumption_preferences_clothes_quality'
-- 'consumption_preferences_clothes_style'
-- 'consumption_preferences_clothes_comfort'
-- 'consumption_preferences_influence_brand_name'
-- 'consumption_preferences_influence_utility'
-- 'consumption_preferences_influence_online_ads'
-- 'consumption_preferences_influence_social_media'
-- 'consumption_preferences_influence_family_members'
-- 'consumption_preferences_spur_of_moment'
-- 'consumption_preferences_credit_card_payment'
-- 'consumption_preferences_health_and_activity'
-- 'consumption_preferences_eat_out'
-- 'consumption_preferences_gym_membership'
-- 'consumption_preferences_outdoor'
-- 'consumption_preferences_concerned_environment'
-- 'consumption_preferences_start_business'
-- 'consumption_preferences_movie_romance'
-- 'consumption_preferences_movie_adventure'
-- 'consumption_preferences_movie_horror'
-- 'consumption_preferences_movie_musical'
-- 'consumption_preferences_movie_historical'
-- 'consumption_preferences_movie_science_fiction'
-- 'consumption_preferences_movie_war'
-- 'consumption_preferences_movie_drama'
-- 'consumption_preferences_movie_action'
-- 'consumption_preferences_movie_documentary'
-- 'consumption_preferences_music_rap'
-- 'consumption_preferences_music_country'
-- 'consumption_preferences_music_r_b'
-- 'consumption_preferences_music_hip_hop'
-- 'consumption_preferences_music_live_event'
-- 'consumption_preferences_music_playing'
-- 'consumption_preferences_music_latin'
-- 'consumption_preferences_music_rock'
-- 'consumption_preferences_music_classical'
-- 'consumption_preferences_read_frequency'
-- 'consumption_preferences_books_entertainment_magazines'
-- 'consumption_preferences_books_non_fiction'
-- 'consumption_preferences_books_financial_investing'
-- 'consumption_preferences_books_autobiographies'
-- 'consumption_preferences_volunteer'

**Sentiment Analysis (Prolexitim_v2_features-6.csv):**
- **MSP_Words**: Multilingual Sentiment Project - Lexicon-based pos/neg words sentiment score.
- **MSP_Stems**: Multilingual Sentiment Project - Lexicon-based pos/neg snowball stems sentiment score.
- **AFINN_Words_Pol**: AFINN-ES - Lexicon-based words polarity score.
- **AFINN_Stems_Pol**: AFINN-ES - Lexicon-based snowball stems polarity score.
- **AFINN_Words_Int**: AFINN-ES - Lexicon-based words mean intensity score.
- **AFINN_Stems_Int**: AFINN-ES - Lexicon-based snowball stems mean intensity score.
- **AFINN_Words_Max**: AFINN-ES - Lexicon-based words max intensity score.
- **AFINN_Stems_Max**: AFINN-ES - Lexicon-based snowball stems max intensity score.
- **Watson_Sent**: IBM Watson Natural Language Understanding API - sentiment score.


