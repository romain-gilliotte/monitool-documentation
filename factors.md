Monitool is not alone in the world of data collection and analysis tools. There are many other tools that can be used for similar purposes, and some of them are even open-source. However, Monitool has some unique features.

## Tolerance to human error

The interface is designed to be tolerant to human error. No action from the interface can result in data loss, and all actions are logged and reversible ("who, what, when").

When modifying data that has already been entered, the system is actually creating a new version of the data, and the old version is kept for reference, so you can always go back to it.

# Tolerant to change

The structure of projects can be modified at any time even after data has been entered.

This is an extremely common situation in the field: the structure of the project is defined at the beginning, but as the project evolves, the structure needs to be modified.

When changing the structure of a project:

- Changes are tracked and reversible
- The new structure is applied to new data, and the old structure is kept for old data
- Data from both the old and new structures is used in reports, by shaping the old data to fit the new structure in predictable ways

# Data interpolation

Indicators derived from data collected over different time periods can be automatically interpolated to match the time periods of the indicator. All interpolated data is marked as such, so you can easily see where and how Monitool filled in the gaps.

This is useful when you have data collected at different frequencies (e.g. daily, weekly, monthly) and you want to mix and match them in the same indicator, which is a common situation when relying on national data sources.

## Absence of personal data

{% hint style="info" %}

We're not lawyers, but we believe that Monitool, when used as intended, should not be covered by data protection regulations such as GDPR, PIPEDA, or others and can be used without requesting consent from involved parties.

{% endhint %}

Disaggregated data, such as individual patient records, are not supported.

This ensures that you can't accidentally expose personal data, but also frees you from the burden of managing personal data in your monitoring system and having to comply with data protection regulations for yet another system.

Keep the individual patient records in a secure place, and only upload the aggregated data in Monitool.
