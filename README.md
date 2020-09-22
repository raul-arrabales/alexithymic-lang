# The Alexithymic Language Project
## A Psicobōtica Labs research project on discovering patterns in alexithymic discourse.
Raúl Arrabales Moreno (raul@psicobotica.com) / Sept. 2020 / Psicobōtica Labs.
<hr>
Most of the code is also designed to serve as educational resource for junior data scientists, and it's being used at different introductory courses on Natural Language Processing (NLP) and Natural Language Understanding (NLU). 
<hr>

**Context information:**
- [What is alexithymia](https://www.psicobotica.com/en/2020/06/08/alexithymia-when-i-dont-realize-how-i-feel/).
- [Data collection via citizen science projects](https://www.psicobotica.com/en/2020/06/11/get-involved-in-our-research-projects/).
- [Prolexitim NLP](https://psicobotica.com/prolexitim/nlp/index.html). The tool used to present the visual stimuli. 
- [Prolexitim TAS-20](https://psicobotica.com/prolexitim/tas-20-spain/). The tool used to measure the level of alexithymia. 
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

### NLP folder

### Models folder 
