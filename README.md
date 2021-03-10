# ilearnium-Survey-Standard


### Main (SurveySkeleton)

default_style: ```String```

default_scaleLabel_zero: ```String``` (optional, default = ```"disagree"```)

default_scaleLabel_max:  ```String``` (optional, default = ```"agree"```)

default_defaultScore: ```Double``` (optional, default = ```0```)

questions: ```[Question]```

scores: ```[score]``` (formula for all other score of survey)

scoreFormula: ```String``` (optional, default = "grandAverage") (formula for the main score of the survey)

### Questions

text: ```String```

condition: ```String``` (optional, default = ```"1"```)

style: ```String``` (optional, default = ```"_DEFAULT"```, reference to **default_style**)

scaleLabel_zero: ```String``` (optional, default = ```"_DEFAULT"```, reference to **default_scaleLabel_zero**)

scaleLabel_max: ```String``` (optional, default = ```"_DEFAULT"```, reference to **default_scaleLabel_max**)

defaultScore: ```Double``` (optional, default = ```-1```, same as ```_DEFAULT```, reference to **default_defaultScore**)

### Score

name: ```String```

formula: ```String```
