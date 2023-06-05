# TipShare

The TipShare spreadsheet is a tool designed to distribute cash tips to employees based on their hours worked. It utilizes Excel's functions and cell referencing to calculate and allocate cash tips in a swift and precise way.

## Business Use Case

In the service industry, distributing cash tips to employees can be a time-consuming and error-prone task. The TipShare spreadsheet streamlines this process by automating the calculation and allocation of tips, saving valuable time for managers. It eliminates the need for manual calculations using paper, pencil, and calculators, reducing the chances of errors and ensuring fairness in distributing tips.

## Why Implement TipShare?

**Time Savings**: With TipShare, the time required to complete tip calculations and distribution is significantly reduced, allowing managers to focus on other important tasks. Our tests revealed time savings of nearly 78% compared to manual calculations.

**Efficiency**: By minimizing the number of button taps and potential errors, TipShare improves the efficiency of tip distribution by approximately 69% compared to manual calculations.

**Compatibility**: TipShare is designed to be compatible with a wide range of technology systems commonly used in the food service industry, making it accessible and adaptable for various establishments.

## How to Use

![tipshare interface](/tipshare.png)

1. **Enter Hours Worked**: Enter the hours worked by each employee from the Timeclock. Enter the respective values in the `Hours Worked` column.

2. **Enter Total Cash Tips**: Enter the total cash tips collected in the single blue cell in the `Cash Tips` column.

3. **Distribute Cash Tips**: The amounts shown in the series of green cells of the `Cash Tips` column will be automatically calculated and allocated to each employee.

Please note the following:

- **Blue Cells**: The blue cells are designated for user input, specifically the `Hours Worked` and `Total Cash Tips`.

- **Green Cells**: The green cells are calculated fields based on user input. These include the `Team Total Hours` and `Cash Tips`.

## TipShare Formula

The TipShare formula is as follows:

```
(Employee Hours Worked) / (Team Total Hours) × Total Cash Tips = Employee Cash Tips
```

## How It Works

The TipShare Excel spreadsheet utilizes the SUM function and cell referencing to calculate the total cash tips for each employee. The SUM function adds the hours for each employee and displays a cumulative total. Cell referencing allows the value in one cell to be referenced in another cell, enabling chaining of functions.

The Tipshare formula is applied to the `Cash Tips` column (C2:C9). Each employee's `Total Hours Worked` for that week (B2:B9) is divided by the `Team Total Hours` (B11). The intermediate result is multiplied by the `Total Cash Tips` for the week (C11). Each employee's `Cash Tips` are displayed in the `Cash Tips` column (C2:C9).

The `TipShare.xlsx` file has Worksheet Protection applied to the `Team Total Hours` and `Cash Tips` cells to prevent accidental breaking or overwriting the formulas. Worksheet Protection can be overridden or disabled at any time using the password: `password`. 

## Adding More Employee Names to TipShare

If you need to add more employee names to the TipShare spreadsheet, follow these steps:

1. Locate the last row that contains employee data. This row should be just above the row with the "Cash Tips" column.

2. Right-click on the row number of the last row and select "Insert" from the context menu. A new row will be inserted below the current row.

3. In the newly inserted row, enter the name of the new employee in the "Employee Name" column.

4. To fill the rest of the cells in the row with the necessary formulas and formatting, use the fill handle:

   - Hover your mouse cursor over the bottom-right corner of the cell in the last row of the "Hours Worked" column. The cursor should change to a small crosshair.
   - Click and drag the fill handle down to the newly inserted row. Excel will automatically fill the cells with the appropriate formulas and formatting based on the existing rows.

5. Double-check that the formulas and formatting have been applied correctly to the new row.

6. Update the "Team Total Hours" and "Cash Tips" cells if necessary to reflect the new employee's information in the calculations.

By inserting a new row and using the fill handle, you can easily add more employee names to the TipShare spreadsheet while ensuring that the formulas and formatting are applied consistently. This allows you to accommodate a growing team without disrupting the functionality of the spreadsheet.

Remember to adjust the protected range, if applicable, to include the newly inserted row to avoid any issues with the worksheet protection.
