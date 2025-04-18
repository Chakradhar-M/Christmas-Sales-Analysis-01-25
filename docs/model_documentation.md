
## Data Model Documentation

The data model integrates multiple dimension and fact tables to enable dynamic analysis of Holiday sales trends. Relationships are established to support accurate filtering, time intelligence, and data enrichment in reports.

|  Table Name      |  Related To   |  Relationship Type | Key Column         |
|-------------------|----------------|-----------------------|--------------------------|
| `DateTable`       | `xmas_data`    | One-to-Many           | `Date`                  |
| `canadian_flags`  | `xmas_data`    | One-to-Many           | `Location`              |
| `toggle_table`    | `xmas_data`    | One-to-Many           | `Event`                 |
| `measures_table`  | None           | No direct relationship| N/A                     |
| `kpi_parameter`   | None           | No direct relationship| N/A                     |

### Holiday Sales Data Model Screenshot
![Data Model img](https://github.com/Chakradhar-M/Christmas-Sales-Analysis-01-25/blob/main/resources/Holiday%20Sales%20Data%20Model.png?raw=true)
