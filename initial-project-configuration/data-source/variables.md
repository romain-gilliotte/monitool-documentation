A data-source is composed of a list of variables (or "measures"), which in turn can be composed of multiple disaggregations.

For example, a data source could be a report from field staff, with the following variables:

| Variable                                        | Disaggregations                     |
| ----------------------------------------------- | ----------------------------------- |
| Number of people reached                        | Service provided, gender, age group |
| Number of people who received a follow-up visit | Service provided                    |
| Number of people who received a referral        |                                     |

In this example, the data source has 3 variables, and variables 1 and 2 have disaggregations.

# Creating a variable

Creating a variable is a four-step process:

1. **Define the variable**: Give it a name
2. **Set the aggregation method**: Define how the data will be aggregated in reports (e.g. sum, average, etc.)
3. **Define the disaggregations**: Define the different ways in which the data can be disaggregated
4. **Configure the data entry form**: Define how the data will be entered in the system

## Defining the variable

{% @arcade/embed flowId="fzo6j1xiitdyz9Kyt99G" url="https://app.arcade.software/share/fzo6j1xiitdyz9Kyt99G" %}

This is by far the quickest step: you only need to name them!

As those names will be used in reports and data entry forms, make sure they are concise.

## Aggregation methods

{% @arcade/embed flowId="KqSDNxrXl6r8eDPu6Vz8" url="https://app.arcade.software/share/KqSDNxrXl6r8eDPu6Vz8" %}

The aggregation method defines how the data will be aggregated in reports. For example, if you are tracking the number of people reached, you will most likely want to sum the data in reports.

A specific page is dedicated to [aggregation methods](./aggregation-modes.md).

## Disaggregations

{% @arcade/embed flowId="AtsADgwdwLwKUsNR2CmA" url="https://app.arcade.software/share/AtsADgwdwLwKUsNR2CmA" %}

Disaggregations are a simple concept: they represent the different ways in which the data can be broken down. For example, if you are tracking the number of people reached, you might want to break it down by gender, age group, etc.

Use them wisely: the more disaggregations you have, the more complex the data entry form will be!

When you define disaggregations, you can group their elements. This is useful for reports, as it allows you to group disaggregations together.

{% hint style="warning" %}

The number of fields in form grows exponentially with the number of disaggregations for any given variable.
Check out the [reducing form size](./reducing-form-size.md) guide.

{% endhint %}

## Data entry layout

{% @arcade/embed flowId="MXkjj4WzPFlF9Ltjq0ub" url="https://app.arcade.software/share/MXkjj4WzPFlF9Ltjq0ub" %}

The data entry layout fields are only displayed when you use disaggregations: they defines the layout of the table that will be used to enter the data.

- Choose the structure of the table (e.g. do you want a table with 2 columns and 3 rows, or 2 columns and 3 rows?)
- Choose which disaggregations will be columns and which will be rows
