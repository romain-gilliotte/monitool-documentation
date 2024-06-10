# Advanced aggregation modes

The aggregation method defines how the data will be aggregated in reports.

It needs to be defined twice: once for aggregating by location, and once for aggregating by time.

The reason why you need to define an aggregation method is that Monitool can be used to collect data that is different in nature. For example, you might want to sum the number of people reached, but average the satisfaction score.

## What are the possible aggregation methods?

The following aggregation methods are available:

- **Sum**: The data will be summed in reports
- **Average**: The data will be averaged in reports
- **Minimum**: The minimum value will be displayed in reports
- **Maximum**: The maximum value will be displayed in reports
- **It's not possible to compute this**: The data will not be aggregated in reports

Note that when [interpolating data](./data-interpolation.md), the aggregation method will be used in reverse:

- If you set the aggregation method to "Sum", the data will be distributed evenly over the period
- If you set the aggregation method to "Average", the data will be duplicated over the period

## When do I need this?

You will need to set the aggregation method at two different levels:

- For location: how the data will be aggregated by location
- For time: how the data will be aggregated by time
- When you add disaggregations: how the data will be aggregated by disaggregation

## Examples

### Example 1: Monthly number of medical consultations

When you track something that is countable you will most likely want to sum the data in reports.

In this case, you would set the aggregation method to "Sum" for both location and time.

| Number of medical consultations | January | February | March | Total |
| ------------------------------- | ------- | -------- | ----- | ----- |
| Clinic A                        | 10      | 15       | 20    | 45    |
| Clinic B                        | 5       | 10       | 15    | 30    |
| Total                           | 15      | 25       | 35    | 75    |

### Example 2: Number of unique beneficiaries

Unique beneficiaries are more complex to aggregate, as you don't want to count the same person twice.

Assuming that your collection sites are far enough from each other that you can consider that a person only goes to one site, you can sum the data by location, but you may not be able to assume that a person does not go to the same clinic in different months.

In this case, you would set the aggregation method to "Sum" for location, and "It's not possible to compute this" for time.

This would give you the following table in reports:

| Number of unique beneficiaries | January | February | March | Total |
| ------------------------------ | ------- | -------- | ----- | ----- |
| Clinic A                       | 10      | 15       | 20    | ?     |
| Clinic B                       | 5       | 10       | 15    | ?     |
| Total                          | 15      | 25       | 35    | ?     |

Note that the total is not computed: you will be able to see totals by month for the whole project, but not by location.

### Example 3: Satisfaction score

When you track a satisfaction score, you will most likely want to average the data in reports.

| Satisfaction score | January | February | March | Total |
| ------------------ | ------- | -------- | ----- | ----- |
| Clinic A           | 70      | 80       | 90    | 80    |
| Clinic B           | 45      | 50       | 55    | 50    |
| Total              | 57.5    | 65       | 72.5  | 65    |
