# Participatory Budgeting Design for the RealWorld

## Data description
The experiment data is structured in single xlsx file with 6 sheets.

### Experiments: 
Details about each instance

**fields**

EXP_ID - experiment ID

PARTICIPANT_ID - participant ID

CURTIME - When the experiment started

TUTORIAL_TIME - how long the tutorial stage took (seconds)

QUIZ_TIME - how long the quiz stage took (seconds)

RESPONSE_TIME - how long the voting stage took (seconds)

ISCONSISTENT - which of the consistency questions were answered correctly

FEEDBACK_EASE - survery feedback

FEEDBACK_INTERFACE - survery feedback

FEEDBACK_CAPTURE - survery feedback

FEEDBACK_MAP - survery feedback

FEEDBACK_CATEGORIES - survery feedback

FEEDBACK_MAP_ACCESS - survery feedback

INPUT_FORMAT - input format shown to the user

ELECTION_NUM - which election was shown (all types can be seen in Elections sheet)

CONSISTENCY_TIME - how long the consistency stage took (seconds)

TOTAL_TIME - how long the entire experiment took (seconds)

TOKEN - token given to the user when finishing the experiment

LOCATION_MAP - the coordinates of the user on the map


### Valid_experiments:
Similar to Experiments, showing only "valid" experiments, i.e. removing experiments from tests and such.

### Participants:
List of participants and their demographic information.

**fields**

PARTICIPANT_ID - participant ID

AGE - age

EDUCATION - level of education

GENDER - gender


### Experiment items:
The vote for each experiment

**fields**

EXP_ID - experiment ID

ITEM_ID - project ID (corresponds to items sheet)

VALUE - 0/1 for approval, 0-100 for points, rank location for ranking

RANK_BEFORE (for rankings only) -  rank of the project as shown to the user

RANK_AFTER(for rankings only) -  rank of the project after the user changed it


### Items
List of possible projects

**fields**

ITEM_ID - item ID

ITEM_NAME - name of the project

VALUE - cost of the project

DESCRIPTION - description of the project

GROUP_NAME - type of project (5 types)

SINGULAR - multiple location or one


### Elections:
List of possible elections (in the experiment 3,6,7 and 8 were used)

**fields**

Election - election ID

ITEM_ID - project ID (corresponds to items sheet)

COORDS - coordinates of the project on the map


## Citation

If you find this code useful for your research, please use the following BibTeX entry.

```bibtex
@inproceedings{fairstein2023participatory,
  title={Participatory Budgeting Design for the Real World},
  author={Fairstein, Roy and Benad, Gerdus and Gal, Kobi},
  booktitle={Proceedings of the 37t AAAI Conference on Artificial Intelligence},
  year={2023}
}
```
