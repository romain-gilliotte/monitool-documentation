{% embed url="https://app.arcade.software/share/1zQWNLHAiyFRifRKaUUl" %}

The calendar section of the form defines where and when the data is collected.

### Location

The location configuration is based on the [Collection Sites](./sites.md) that you have previously created. You can select individual sites, or groups of sites.

### Frequency

Depending on the context of your project, you can choose to collect data at different frequencies.

From the more frequent to the less frequent:

- Daily:
  - Seldomly used on a monitoring context (indicators are not tracked daily)
  - Can be useful when Monitool is used for data collection for field activities.
  - Beware of making data-entry in the platform too costly!
- Weekly, splitted by month:
  - When a week overlaps two months, two separate forms will need to be filled for the start and end of the week
  - This allows to have exact numbers when aggregating week data into months in reports
  - You can choose to start the weeks on Saturday, Sunday or Monday, [depending on the project's location](https://en.wikipedia.org/wiki/Week#/media/File:First_Day_of_Week_World_Map.svg).
- Weekly:
  - Same as previous, but without form duplication when a week overlaps two months
- Monthly, Quaterly and Year: for less frequent data.

Note that when using the weekly periodicity, and aggregating data by month, the data will be attached to the month where most days of the overlapping week are.
