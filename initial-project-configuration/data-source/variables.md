Creating a variable is a four-step process:

1. **Define the variable**: Give it a name
2. **Set the aggregation method**: Define how the data will be aggregated in reports (e.g. sum, average, etc.)
3. **Define the disaggregations**: Define the different ways in which the data can be disaggregated
4. **Configure the data entry form**: Define how the data will be entered in the system

### Defining the variable

{% embed url="https://app.arcade.software/share/fzo6j1xiitdyz9Kyt99G" %}

This is by far the quickest step: you only need to name them!

### Aggregation methods

{% embed url="https://app.arcade.software/share/KqSDNxrXl6r8eDPu6Vz8" %}

The aggregation method defines how the data will be aggregated in reports. For example, if you are tracking the number of people reached, you will most likely want to sum the data in reports.

A specific page is dedicated to [aggregation methods](./aggregation-modes.md).

### Disaggregations

Disaggregations are a simple concept: it represent the different ways in which the data can be broken down. For example, if you are tracking the number of people reached, you might want to break it down by gender, age group, etc.

{% hint style="warning" %}

The number of fields in form grows exponentially with the number of disaggregations for any given variable.
Check out the [reducing form size](./reducing-form-size.md) guide.

{% endhint %}

### Data entry layout

{% embed url="https://app.arcade.software/share/MXkjj4WzPFlF9Ltjq0ub" %}

The data entry layout fields are only displayed when you use disaggregations: they defines the layout of the table that will be used to enter the data.

- Choose the structure of the table (e.g. do you want a table with 2 columns and 3 rows, or 2 columns and 3 rows?)
- Choose which disaggregations will be columns and which will be rows
