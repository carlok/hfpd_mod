# Heart Failure Prediction Dataset modified version

This dataset is a modified version of the famous [Heart Failure Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction).

The changes are:

* binary features are turned to {0, 1} labels:
    * Sex => {'M' 'F'} => {0, 1}
    * ExerciseAngina => {'N' 'Y'} => {0, 1}
* multi-class features are turned into new binary features using [hot encoding](https://en.wikipedia.org/wiki/One-hot#Machine_learning_and_statistics):
    * ChestPainType
    * RestingECG
    * ST_Slope
* labels are shortened:
    * Age => A
    * RestingBP => RBP
    * Cholesterol => C
    * FastingBS => FBS
    * MaxHR => MHR
    * Oldpeak => OP
    * HeartDisease => HD
    * Sex => S
    * ExerciseAngina => EA
    * ChestPainType
        * CPT_ASY
        * CPT_ATA
        * CPT_NAP
        * CPT_TA
    * RestingECG
        * RECG_LVH
        * RECG_N (Normal)
        * RECG_ST
    * ST_Slope
        * STS_D (Down)
        * STS_F (Flat)
        * STS_U (Up)
