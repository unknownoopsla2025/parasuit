# ParaSuit - Data

This directory stores information about previously tested programs.
In this directory, five types of data are collected for each target program:

+ candidates              Store the used values during trials in the Extraction stage
+ covered_branches        Store the branch log covered when each candidate value is used
+ init_values             Store the initial value of each selected parameter for value sampling
+ min_parameters          Store the minimal parameter set required for KLEE to run for each program
+ param_scores            Store the score of each parameter from the most recent iteration

For target programs without existing data, ParaSuit automatically stores the five types of data in their respective directories after testing is complete.
By default, we include data for the following 12 target programs:

| Benchmark | version | Benchmark | version | Benchmark | version |
|:------:|:------------|:------:|:------------|:------:|:------------|
| combine   | 0.4.0 | gawk      | 5.1.0  | nano         | 4.9   |
| diff      | 3.7   | gcal      | 4.1    | sed          | 4.8   |
| du        | 8.32  | grep      | 3.4    | trueprint    | 5.4   |
| enscript  | 1.6.6 | ls        | 8.32   | xorriso     | 1.5.2 |
