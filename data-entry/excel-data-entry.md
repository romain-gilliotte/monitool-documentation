# Excel data entry

Excel is the most common tool used to collect data in the field. It is well known, flexible, and can be used offline.

It works with Monitool in two main ways:

- Entering data from users which do not have access to the platform, or no internet connectivity
- Dealing with primary sources of data, such as tally sheets, individual patient records, or other raw data

# Using Excel as an offline data entry tool

Monitool can only be used online, this is a strong advantage: it enables having a single source of truth, and makes sure that you will never end up with conflicting versions of your data, even if you are working with a team.

However, we understand that sometimes you need to work offline, and that's why we support Excel as a data entry tool.

In this simple case, download the template from Monitool, fill it with your data without worrying about internet connectivity, and then upload it to Monitool when you are back online.

# Dealing with disaggregated data

Monitool is designed to work with aggregated data, such as the number of patients seen in a health center in a given day, or the number of children vaccinated in a given month. Arbitrary levels of aggregation are supported, from daily to yearly, spliting the data by any dimension you want (e.g. gender, age, location, etc.).

However, disaggregated data, such as individual patient records, are not navitely supported.

This ensures that you can't accidentally expose personal data, but also frees you from the burden of managing personal data in your monitoring system and needing to comply with data protection regulations: you can keep the individual patient records in a secure place, and only upload the aggregated data in Monitool.

But that creates a problem: how do go a tally sheet, containing one line per patient seen in a health center in a given day, into a format that Monitool can understand?

You are probably already using Excel for that, and that's why we recommend that you continue doing just that.

## Create your tally sheet in the Excel template

The steps are the following:

- Download the Excel template from Monitool
- Create a new sheet in your Excel file with the structure of your tally sheet
- Enter the necessary formulas to aggregate the data into the "Data Entry" sheet that Monitool created
- Save the file and keep it!

{% hint style="info" %}

You will probably use the following Excel formulas extensively:

- [COUNTIFS](https://support.microsoft.com/en-us/office/countifs-function-dda3dc6e-f74e-4aee-88bc-aa8c2a866842) Allows to count rows that meet multiple criteria
- [SUMIFS](https://support.microsoft.com/en-au/office/sumifs-9bdc9d30-4277-4888-b606-ae9927a650bb) Allows to sum fields from rows that meet multiple criteria

{% endhint %}

## Using your Excel file

When you are ready to enter the data in Monitool, you can either enter or copy-paste the data in the tabs that you created in the Excel file, and then upload the file in Monitool.
