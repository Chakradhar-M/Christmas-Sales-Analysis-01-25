
## 🎄  Power Query Transformations Documentation


#### 1️⃣ **`xmas_data` (Main Sales Data Table)**  
**Source**: Excel file – `Xmas Sales & Trends_C22.xlsx` → Sheet: `MasterData`

**Applied Steps:**
- **Data Type Conversion**: Changed column data types to appropriate types (e.g., dates, integers, logical).
- **Column Renaming**: Swapped `"Longitude"` and `"Latitude"` headers for accuracy.
- **Text Conversion for Flags**: Converted logical (True/False) flags (`Online Order Flag`, `Promotion Applied`, `Gift Wrap`, `Return Flag`) to **Yes/No** values.
- **Text Cleaning**: Replaced underscores (`_`) in `Product Name` with spaces.
- **Final Price Calculation**: Created a new column:  
  `Final Price = [Total Price] - [Discount Amount]`
- **Channel & Feature Labeling**:
  - `Online Order Flag`: Yes → **Online**, No → **In-Store**
  - `Gift Wrap`: Yes → **Wrapped**, No → **Unwrapped**
  - `Promotion Applied`: Yes → **Applied**, No → **Not Applied**
  - `Return Flag`: Yes → **Returned**, No → **Not Returned**
- **Event Column Cleaning**:
  - `Christmas Market` → **Christmas**
  - `None` → **Regular**

---

#### 2️⃣ **`candian_flags` (Flag Image Table)**  
**Source**: CSV file – `canadian_flags.csv`

**Applied Steps:**
- **Data Type Conversion**: Ensured columns are in text format.
- **Header Promotion**: Promoted the first row to headers.
- **Final Column Types**:  
  - `Location`: text  
  - `flag_link`: text (URL to flag image)

---

#### 3️⃣ **`toggle_table` (Event Toggles Table)**  
**Source**: JSON/Encoded table for toggling visual filters(Created in Power BI using `Enter Data`)

**Applied Steps:**
- **Decoding & Decompression**: Converted a compressed JSON string to table format.
- **Data Type Conversion**:  
  - `Event`: text  
  - `Toggle ON`: text  
  - `Toggle OFF`: text  

---

#### 4️⃣ **`kpi_parameter` (Parameter Table for Dynamic KPIs)**  
**Definition**:  
A manually created list table for switching between key metrics dynamically.

**Structure**:  
- `Label` (Display Name)  
- `MeasureName` (Reference to measure in model)  
- `Index` (Sorting or selection logic)

**Values**:
```
("Transactions", NAMEOF('measures_table'[Transactions]), 0),
("Sales Volume", NAMEOF('measures_table'[Sales Volume]), 1),
("Sales ($)", NAMEOF('measures_table'[Sales ($)]), 2)
```

---

#### 5️⃣ **`datetable` (Date Dimension Table)**  
**Definition**: Calculated table using DAX.

```dax
DateTable = 
ADDCOLUMNS(
    CALENDAR(DATE(2018, 1, 1), DATE(2023, 12, 31)),
    "Year", YEAR([Date]),
    "Month", MONTH([Date]),
    "Month Name", FORMAT([Date], "MMM"),
    "Quarter", "Q" & FORMAT([Date], "Q"),
    "Day Name", FORMAT([Date], "ddd"),
    "Day Order", WEEKDAY([Date], 2)
)
```

**Purpose**: To support time intelligence in reporting, including Year-Month breakdowns, Quarter filtering, weekday trends, and proper date sorting.


