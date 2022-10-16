## Evaluation Metrics for Object Detection
This repository presents the results corresponding to the ICRA 2023 Submission on Evaluation Metrics for Object Detection for Autonomous Systems by Apurva Badithela, Tichakorn Wongpiromsarn, and Richard M. Murray. The paper presents two types of evaluation metrics -- class-labeled and proposition-labeled  -- -- distance parametrized confusion matrices. A variation of each of these metrics that accounts for distance from ego is also accounted for.

### Class-labeled distance parameterized confusion matrix
Class-labeled Confusion matrix for distance $0 < d <= 10.0$
```
-----------------------------------------------------------------------
                 |   ('pedestrian',) |   ('obstacle',) |   ('empty',) |
-----------------------------------------------------------------------
 ('pedestrian',) |                31 |               0 |            0 |
 ('obstacle',)   |                 0 |             191 |            0 |
 ('empty',)      |               127 |             734 |         3227 |
-----------------------------------------------------------------------
```
Class-labeled Confusion matrix for distance $10 < d <= 20.0$
```
-----------------------------------------------------------------------
                 |   ('pedestrian',) |   ('obstacle',) |   ('empty',) |
-----------------------------------------------------------------------
 ('pedestrian',) |               158 |               2 |            0 |
 ('obstacle',)   |                 1 |             998 |            0 |
 ('empty',)      |               873 |            3526 |         1969 |
-----------------------------------------------------------------------
 ```
 
Class-labeled Confusion matrix for distance $20.0 < d <= 30.0$
 ```
-----------------------------------------------------------------------
                 |   ('pedestrian',) |   ('obstacle',) |   ('empty',) |
-----------------------------------------------------------------------
 ('pedestrian',) |               291 |               4 |            0 |
 ('obstacle',)   |                 0 |            1052 |            0 |
 ('empty',)      |              1794 |            4689 |         1387 |
-----------------------------------------------------------------------
```

Class-labeled Confusion matrix for distance $30.0 < d <= 40.0$
```

-----------------------------------------------------------------------
                 |   ('pedestrian',) |   ('obstacle',) |   ('empty',) |
-----------------------------------------------------------------------
 ('pedestrian',) |               183 |               5 |            0 |
 ('obstacle',)   |                 0 |             983 |            0 |
 ('empty',)      |              1913 |            4132 |         1474 |
-----------------------------------------------------------------------
 ```

Class-labeled Confusion matrix for distance $40.0 <= d <= 50.0$
```
-----------------------------------------------------------------------
                 |   ('pedestrian',) |   ('obstacle',) |   ('empty',) |
-----------------------------------------------------------------------
 ('pedestrian',) |                30 |               3 |            0 |
 ('obstacle',)   |                 0 |             759 |            0 |
 ('empty',)      |              1396 |            3093 |         1733 |
-----------------------------------------------------------------------
 ```
 
Class-labeled confusion matrix for distance $50.0 <= d <= 60.0$
```
-----------------------------------------------------------------------
                 |   ('pedestrian',) |   ('obstacle',) |   ('empty',) |
-----------------------------------------------------------------------
 ('pedestrian',) |                10 |               3 |            0 |
 ('obstacle',)   |                 0 |             409 |            0 |
 ('empty',)      |               848 |            2151 |         2188 |
-----------------------------------------------------------------------
```
 
Class-labeled Confusion matrix for distance $60.0 <= d <= 70.0$
```
-----------------------------------------------------------------------
                 |   ('pedestrian',) |   ('obstacle',) |   ('empty',) |
-----------------------------------------------------------------------
 ('pedestrian',) |                 5 |               3 |            0 |
 ('obstacle',)   |                 0 |             171 |            0 |
 ('empty',)      |               555 |            1167 |         2742 |
-----------------------------------------------------------------------
 ```
 
Class-labeled Confusion matrix from distance $70.0 <= d <= 80.0$
```
-----------------------------------------------------------------------
                 |   ('pedestrian',) |   ('obstacle',) |   ('empty',) |
-----------------------------------------------------------------------
 ('pedestrian',) |                 2 |               1 |            0 |
 ('obstacle',)   |                 0 |              85 |            0 |
 ('empty',)      |               281 |             761 |         3077 |
-----------------------------------------------------------------------
 ```
 
Class-labeled Confusion matrix from distance $80.0 <= d <= 90.0$
```
-----------------------------------------------------------------------
                 |   ('pedestrian',) |   ('obstacle',) |   ('empty',) |
-----------------------------------------------------------------------
 ('pedestrian',) |                 1 |               0 |            0 |
 ('obstacle',)   |                 0 |              36 |            0 |
 ('empty',)      |                88 |             409 |         3436 |
-----------------------------------------------------------------------
 ```
 
Class-labeled confusion matrix from distance $90.0 <= d <= 100.0$
```
-----------------------------------------------------------------------
                 |   ('pedestrian',) |   ('obstacle',) |   ('empty',) |
-----------------------------------------------------------------------
 ('pedestrian',) |                 0 |               0 |            0 |
 ('obstacle',)   |                 0 |              12 |            0 |
 ('empty',)      |                35 |             207 |         3651 |
-----------------------------------------------------------------------
```

### Proposition-labeled Distance Parametrized Confusion matrix

Proposition-labeled Confusion matrix for distance $0 < d <= 10.0$
```
-----------------------------------------------------------------------------------------------------------------
                            |   ('pedestrian',) |   ('obstacle',) |   ('pedestrian', 'obstacle') |   ('empty',) |
-----------------------------------------------------------------------------------------------------------------
 ('pedestrian',)            |                22 |               0 |                            5 |            0 |
 ('obstacle',)              |                 0 |             184 |                            4 |            0 |
 ('pedestrian', 'obstacle') |                 0 |               0 |                            0 |            0 |
 ('empty',)                 |                63 |             354 |                           13 |         3227 |
-----------------------------------------------------------------------------------------------------------------
```
Proposition-labeled Confusion matrix for distance $10 < d <= 20.0$
```
-----------------------------------------------------------------------------------------------------------------
                            |   ('pedestrian',) |   ('obstacle',) |   ('pedestrian', 'obstacle') |   ('empty',) |
-----------------------------------------------------------------------------------------------------------------
 ('pedestrian',)            |                52 |               2 |                           39 |            0 |
 ('obstacle',)              |                 0 |             714 |                           92 |            0 |
 ('pedestrian', 'obstacle') |                 0 |               0 |                           28 |            0 |
 ('empty',)                 |               180 |             662 |                          134 |         1969 |
-----------------------------------------------------------------------------------------------------------------
 ```
 
Proposition-labeled Confusion matrix for distance $20.0 < d <= 30.0$
 ```
-----------------------------------------------------------------------------------------------------------------
                            |   ('pedestrian',) |   ('obstacle',) |   ('pedestrian', 'obstacle') |   ('empty',) |
-----------------------------------------------------------------------------------------------------------------
 ('pedestrian',)            |               117 |               4 |                           43 |            0 |
 ('obstacle',)              |                 0 |             678 |                          178 |            0 |
 ('pedestrian', 'obstacle') |                 0 |               0 |                           40 |            0 |
 ('empty',)                 |               311 |             883 |                          231 |         1387 |
-----------------------------------------------------------------------------------------------------------------
```

Proposition-labeled Confusion matrix for distance $30.0 < d <= 40.0$
```
-----------------------------------------------------------------------------------------------------------------
                            |   ('pedestrian',) |   ('obstacle',) |   ('pedestrian', 'obstacle') |   ('empty',) |
-----------------------------------------------------------------------------------------------------------------
 ('pedestrian',)            |                47 |               5 |                           52 |            0 |
 ('obstacle',)              |                 0 |             602 |                          193 |            0 |
 ('pedestrian', 'obstacle') |                 0 |               0 |                           36 |            0 |
 ('empty',)                 |               321 |             878 |                          264 |         1474 |
-----------------------------------------------------------------------------------------------------------------
 ```

Proposition-labeled confusion matrix for distance $40.0 <= d <= 50.0$
```
-----------------------------------------------------------------------------------------------------------------
                            |   ('pedestrian',) |   ('obstacle',) |   ('pedestrian', 'obstacle') |   ('empty',) |
-----------------------------------------------------------------------------------------------------------------
 ('pedestrian',)            |                21 |               3 |                            7 |            0 |
 ('obstacle',)              |                 0 |             515 |                          142 |            0 |
 ('pedestrian', 'obstacle') |                 0 |               0 |                            1 |            0 |
 ('empty',)                 |               302 |             907 |                          241 |         1733 |
-----------------------------------------------------------------------------------------------------------------
 ```
 
Proposition-labeled confusion matrix for distance $50.0 <= d <= 60.0$
```
-----------------------------------------------------------------------------------------------------------------
                            |   ('pedestrian',) |   ('obstacle',) |   ('pedestrian', 'obstacle') |   ('empty',) |
-----------------------------------------------------------------------------------------------------------------
 ('pedestrian',)            |                 8 |               3 |                            2 |            0 |
 ('obstacle',)              |                 0 |             332 |                           53 |            0 |
 ('pedestrian', 'obstacle') |                 0 |               0 |                            0 |            0 |
 ('empty',)                 |               251 |             838 |                          197 |         2188 |
-----------------------------------------------------------------------------------------------------------------
```
 
Proposition-labeled Confusion matrix for distance $60.0 <= d <= 70.0$
```
-----------------------------------------------------------------------------------------------------------------
                            |   ('pedestrian',) |   ('obstacle',) |   ('pedestrian', 'obstacle') |   ('empty',) |
-----------------------------------------------------------------------------------------------------------------
 ('pedestrian',)            |                 4 |               3 |                            0 |            0 |
 ('obstacle',)              |                 0 |             146 |                           15 |            0 |
 ('pedestrian', 'obstacle') |                 0 |               0 |                            0 |            0 |
 ('empty',)                 |               206 |             668 |                           88 |         2742 |
-----------------------------------------------------------------------------------------------------------------
 ```
 
Proposition-labeled Confusion matrix from distance $70.0 <= d <= 80.0$
```
-----------------------------------------------------------------------------------------------------------------
                            |   ('pedestrian',) |   ('obstacle',) |   ('pedestrian', 'obstacle') |   ('empty',) |
-----------------------------------------------------------------------------------------------------------------
 ('pedestrian',)            |                 2 |               1 |                            0 |            0 |
 ('obstacle',)              |                 0 |              79 |                            5 |            0 |
 ('pedestrian', 'obstacle') |                 0 |               0 |                            0 |            0 |
 ('empty',)                 |               136 |             541 |                           31 |         3077 |
-----------------------------------------------------------------------------------------------------------------
 ```
 
Proposition-labeled confusion matrix from distance $80.0 <= d <= 90.0$
```
-----------------------------------------------------------------------------------------------------------------
                            |   ('pedestrian',) |   ('obstacle',) |   ('pedestrian', 'obstacle') |   ('empty',) |
-----------------------------------------------------------------------------------------------------------------
 ('pedestrian',)            |                 1 |               0 |                            0 |            0 |
 ('obstacle',)              |                 0 |              34 |                            2 |            0 |
 ('pedestrian', 'obstacle') |                 0 |               0 |                            0 |            0 |
 ('empty',)                 |                51 |             337 |                           11 |         3436 |
-----------------------------------------------------------------------------------------------------------------
 ```
 
Proposition-labeled confusion matrix from distance $90.0 <= d <= 100.0$
```
-----------------------------------------------------------------------------------------------------------------
                            |   ('pedestrian',) |   ('obstacle',) |   ('pedestrian', 'obstacle') |   ('empty',) |
-----------------------------------------------------------------------------------------------------------------
 ('pedestrian',)            |                 0 |               0 |                            0 |            0 |
 ('obstacle',)              |                 0 |              12 |                            0 |            0 |
 ('pedestrian', 'obstacle') |                 0 |               0 |                            0 |            0 |
 ('empty',)                 |                23 |             180 |                            6 |         3651 |
-----------------------------------------------------------------------------------------------------------------
```