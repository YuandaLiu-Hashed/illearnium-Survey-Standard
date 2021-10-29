# illearnium-Survey-Standard


### Main (SurveySkeleton)

default_style: ```String```

default_scaleLabel_zero: ```String``` (optional, default = ```"disagree"```)

default_scaleLabel_max:  ```String``` (optional, default = ```"agree"```)

default_defaultScore: ```Double``` (optional, default = ```0```)

questions: ```[Question]```

scores: ```[score]``` (formula for all other score of survey)

scoreFormula: ```String``` (optional, default = "$average") (formula for the main score of the survey)

### Questions

text: ```String```

condition: ```String``` (optional, default = ```"1"```)

style: ```String``` (optional, default = ```"_DEFAULT"```, reference to **default_style**)

scaleLabel_zero: ```String``` (optional, default = ```"_DEFAULT"```, reference to **default_scaleLabel_zero**)

scaleLabel_max: ```String``` (optional, default = ```"_DEFAULT"```, reference to **default_scaleLabel_max**)

defaultScore: ```Double``` (optional, default = ```-1```, same as ```_DEFAULT```, reference to **default_defaultScore**)
#### All Acceptable Replacement in Condition Formula:
1. **$q#** where # is question number (example: $q1), index start at zero

### Score
name: ```String```

formula: ```String```

#### All Acceptable Replacement in Score Formula:
1. **$q#** (where # is question number, index start at zero) - Answer of said question, scale always from 0 to 1. (example: $q1)
2. $average - average of all questions. (ones with a false condition substitues its default value)
3. $min and $max - min or max of all questions. (ones with a false condition substitues its default value)
