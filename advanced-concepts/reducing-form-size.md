The difficulty with disaggregations is that there are trade-offs to be made:

- Between the precision of the data and the time it takes to collect it
- Between having few variables with many disaggregations, or many variables with few disaggregations

Remember that because Monitool [does not support disaggregated data](../limits.md), the size of the form grows exponentially with the number of disaggregations.

Usually, those forms are not meant to be filled by hand, but rather to be filled using the [Excel data entry method](../data-entry/excel-data-entry.md), it is still important to keep them manageable. Consider forms with more than 50 fields as a warning flag and a certainty for a lot of data entry errors.

| # of disaggregations | # of elements in each disaggregation | # of fields in the form for that variable |
| -------------------- | ------------------------------------ | ----------------------------------------- |
| 0                    | -                                    | 1                                         |
| 1                    | 3                                    | 3                                         |
| 2                    | 3                                    | 9 (3 x 3)                                 |
| 3                    | 3                                    | 27 (3 x 3 x 3)                            |
| 4                    | 3                                    | 81!!! (3 x 3 x 3 x 3)                     |
