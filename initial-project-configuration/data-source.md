# Data Source

## What is a data source?

{% hint style="info" %}
Resist the temptation to put all the data that you need to compute your indicators in a single data source.
By doing so your risk loosing most of what makes Monitool useful:

- Track the quality and progress of data collection
- Assign data collection tasks to identified users
- Highlight data that is missing

{% endhint %}

Data sources should represent a single source of data that is backed by actual data collection in the field.
It describe how and when data is collected to compute indicators.

As a general rule, a data source is a document or a system that contains data that is relevant to the project.

Any of the following can be a data source:

- Surveys from target population
- Reports from field staff
- Reports from a partner organization
- Health information systems
- Data from government agencies
- Data from accounting software

## Which data should I track?

It can be tempting to track all the data that you can think of, but remember that data collection is time-consuming, and is only a small part of the work that needs to be done to have reliable indicators (cleaning, analysis, etc.).

Start by tracking the **minimum amount** of data that you need to compute your indicators. If you find that you need more data, you can always add more at a later stage.

We recommend following the [recommended order](./recommended-order.md) for setting up a project in Monitool. It will help you to focus on the most important data first.

## Anatomy of a data source

A data-source is composed of a list of variables (or "measures"), which in turn can be composed of multiple disaggregations.

For example, a data source could be a report from field staff, with the following variables:

| Variable                                        | Disaggregations                     |
| ----------------------------------------------- | ----------------------------------- |
| Number of people reached                        | Service provided, gender, age group |
| Number of people who received a follow-up visit | Service provided                    |
| Number of people who received a referral        |                                     |

In this example, the data source has 3 variables, and variables 1 and 2 have disaggregations.

## Understanding the variable creation process

Creating a variable is a four-step process:

1. **Define the variable**: Give it a name
2. **Set the aggregation method**: Define [how the data will be aggregated](../advanced-concepts/aggregation-modes.md) in reports (e.g. sum, average, etc.)
3. **Define the disaggregations**: Define the different ways in which the data can be disaggregated
4. **Configure the data entry form**: Define how the data will be entered in the system

### Aggregation methods

The aggregation method defines how the data will be aggregated in reports. For example, if you are tracking the number of people reached, you will most likely want to sum the data in reports.

A specific page is dedicated to [aggregation methods](../advanced-concepts/aggregation-modes.md).

### Disaggregations

Disaggregations are a simple concept: it represent the different ways in which the data can be broken down. For example, if you are tracking the number of people reached, you might want to break it down by gender, age group, etc.

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

### Data entry form configuration

The data entry form configuration is only needed when you use disaggregations: it defines the layout of the table that will be used to enter the data.

It is done in two steps:

- Chosing the structure of the table (e.g. do you want a table with 2 columns and 3 rows, or 2 columns and 3 rows?)
- Chosing which disaggregations will be columns and which will be rows
