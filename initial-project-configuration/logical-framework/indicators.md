# Indicators

An indicator is a numeric value that is calculated from the data entered into the system. Indicators are used to measure the progress of a project or program.

In Monitool, indicators are always linked to one or more data sources. This means that the data entered into the system is used to calculate the indicators. You can't create an indicator completely from scratch, you need to have data sources that provide the data needed to calculate the indicator, nor can you create an indicators that depend on other indicators.

## How to create an indicator

{% embed url="https://app.arcade.software/share/3ooz37r23FyeMcSx2MVC" %}

If you are following the [recommended order](../recommended-order.md) all indicators always start their life as "non computable". This means that the indicator is created, but it is not yet linked to any data sources. You'll come back later to connect it.

To create an indicator, follow these steps:

- Click on `Add indicator` in a section of a logical framework (e.g. `Objectives`, `Results`, `Activities`), or in the `Extra indicators` page.
- Enter the name of the indicator.
- If relevant enter a baseline value and a target value. These values are used to calculate the progress of the indicator. Check the `Colorize` checkbox to colorize the progress of the indicator in reports.
- Click on `Apply changes`.
- Save the logical framework.

## Computation

An indicator is computed by applying a formula to the data sources. The formula can simply copy a value from a data source, or it can use a predefined formula to calculate the indicator.

If your indicator cannot be computed with one of the predefined formulas, you can use a custom formula.

### Predefined formulas

{% embed url="https://app.arcade.software/share/PA2MQ6kI6wJS1akEI6AZ" %}

There are only three predefined formulas:

- Copy a variable from a data source as is.
- Compute a percentage from two variables (in the same data source or not).
- Compute a permillage from two variables (in the same data source or not).

Select the formula that best fits your needs and link the data sources to the indicator.

### Custom formulas

{% embed url="https://app.arcade.software/share/1qNycwQtuxS8A6pSngTW" %}

The syntax for the formula is similar to a spreadsheet formula, with the difference that you can use any name (without the space character) to refer to a data source.

For example, if you have a variable named `Number of beneficiaries` you can refer to it in the formula as `numberofbeneficiaries` or `x` or `num_befs`. The name itself does not matter, as long as it is unique in the formula. Also note that the names are case sensitive, so `numberofbeneficiaries` is different from `NumberOfBeneficiaries`.

| Operator | Description    | Use for                                         | Example                                               |
| -------- | -------------- | ----------------------------------------------- | ----------------------------------------------------- |
| `+`      | Addition       | Sum counts from different data sources          | `mobile_consultations + clinic_consultations`         |
| `-`      | Subtraction    | Compute unique people                           | `total_patients - repeat_patients`                    |
| `*`      | Multiplication | Aggregate multiple scores into one with weights | `score_hygiene * 2 + score_satisfaction`              |
| `/`      | Division       | Compute percentages                             | `100 * consultations_attended / consultations_missed` |
| `\|\|`   | Default value  | Replace missing variables by provided number    | `(mobile_consultations \|\| 0)`                       |

## Using desaggregation in indicators

{% embed url="https://app.arcade.software/share/g5DNLgx8ew5T5GWlwkdv" %}

You may want to compute indicators which include only some age groups, gender, or other disaggregation elements.

This is done by selecting the appropriate values on the right side of the indicator creation form. You can select multiple values for each disaggregation element. You can also use the `All` option to include all values for a given disaggregation element.
