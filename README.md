# Mortgage Amortization
This repo holds a mortgage amortization sheet that was built in Google Sheets in CSV and Excel format.

You can copy the Google Sheet here: https://docs.google.com/spreadsheets/d/18EcN6qMgRPKmWy_2R3GsSoTc6Dt6s4kcxBn08wm40M8/

Note: Inputs highlighted yellow in the Google Sheet are inputs that the user can/should modify, and inputs that are not highlighted are calculated/updated automatically based on changes to the highlighted inputs.

## Preview

### Inputs 
These inputs are found at the top of the sheet. Inputs written in _italics_ are automically calculated based on changes to the other inputs. _There are no "Item" or "Value" columns, they are just here so that GitHub will display the input table correctly in markdown._

| **Item**                   | **Value**         |   | **Item**                 | **Value**         |
|----------------------------|-------------------|---|--------------------------|-------------------|
| Price of House             | $200,000.00      |   | _Loan Payment_             | $858.91           |
| Down Payment %             | 20.00%           |   | Property Tax             | $0.00             |
| _Down Payment $_             | $40,000.00       |   | HOA                      | $0.00             |
| _Loan Amount_                | $160,000.00      |   | Property Insurance       | $0.00             |
| Mortgage Rate              | 5.00%            |   | Mortgage Insurance       | $0.00             |
| _Monthly Mortgage Rate_      | 0.42%            |   | Other                    | $0.00             |
| Mortgage Term (Years)      | 30               |   | Extra Payment            | $0.00             |
|                            |                   |   | _Total Monthly Payment_    | $858.91           |

### Table 
These table values automatically update based on the inputs. (Note: if you use the CSV file these inputs will not change automatically.)

| Month | Beginning Balance | Monthly Interest | Monthly Payment | Extra Payment | Ending Balance | Principal Repayment | Total Principal Repayment | Homeowner Equity |
|-------|--------------------|------------------|-----------------|---------------|----------------|---------------------|--------------------------|------------------|
| 1     | $160,000.00       | $666.67          | $858.91         | $0.00         | $159,807.75    | $192.25             | $192.25                  | $40,000.00       |
| 2     | $159,807.75       | $665.87          | $858.91         | $0.00         | $159,614.70    | $193.05             | $385.30                  | $40,385.30       |
| 3     | $159,614.70       | $665.06          | $858.91         | $0.00         | $159,420.85    | $193.85             | $579.15                  | $40,579.15       |

### Calculated Outputs
These calculated output values automatically update based on the inputs. (Note: if you use the CSV file these inputs will not change automatically.)

| **Item**         | **Value**       |
|-------------------|-----------------|
| Total Payments    | $309,209.25    |
| Total Interest    | $149,209.25    |

![Mortgage Balance Chart](https://github.com/gumdropsteve/mortgage-amortization/blob/main/Beginning%20Balance%20vs.%20Month.png)
