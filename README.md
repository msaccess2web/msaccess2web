# msaccess2web

## Access Microsoft Access data on the Web. Windows only.

No database migration required. No code needed.

Web application created with **a single command in 1 second**:

scaffold.py --db **C:\Users\Downloads\access_database.accdb**


# How to run?

Download this repository. If MS Access is not installed, you'll need [Microsoft Access 2016 Runtime](https://www.microsoft.com/en-us/download/details.aspx?id=50040).

Open Windows "Command Prompt". Navigate to downloaded or unzipped folder. Run as above **IF** you have Python installed, plus installed dependencies with "pip install pyodbc textblob sqlparse inflect":

scaffold_msaccess.py --db **C:\Users\Downloads\access_database.accdb**


If Python is **not** installed, download scaffold_msaccess.exe from Releases on the right hand side, and run:

scaffold_msaccess.exe --db **C:\Users\Downloads\access_database.accdb**


scaffold_msaccess.exe is packaged application by Github actions with Python and above dependencies. It is safe to use since built with Github.


# Running result

The above command will show you the results. For example, for the below video, the result is:

```
📊 Grouped Inserted Tables by Meaning:

  • Account (1): Account
  • Asset (6): Asset, AssetProperity, AssetSubType, AssetTrx, AssetTrxType, AssetType
  • Audit (4): AuditAccount, AuditChart, AuditDevice, AuditUsers
  • Cash (1): CashCustomer
  • Chart (1): Chart
  • Check (2): CheckFollow, CheckFollowType
  • Company (1): Company
  • Component (1): Component
  • Contract (1): ContractType
  • Cost (1): CostCenter
  • Currency (1): Currency
  • Customer (2): Customer, CustomerType
  • Department (1): Department
  • Depreciation (3): Depreciation, DepreciationPeriod, DepreciationType
  • Detail (1): DetailJournaltype
  • Device (3): Device, DeviceHistory, DeviceType
  • Domain (1): Domain
  • Employe (4): Employe, EmployeHistory, EmployeHistoryDetail, EmployeLoanDistribution
  • Entry (2): Entry, EntryDetail
  • Fin (1): FinYear
  • Geo (1): GeoSector
  • Group (1): GroupItem
  • Inventory (4): InventoryTRX, InventoryTRXDetail, InventoryTRXDetailDistribution, InventoryTrxType
  • Item (5): Item, ItemDetail, ItemType, ItemUom, item_migrated
  • Location (1): LOCATION
  • Main (2): MainCode, MainJournalType
  • Nature (1): Nature
  • Order (2): Order, OrderDetail
  • Over (2): OverTimeDetail, OverTimeRate
  • Period (1): Period
  • Po (1): PosBatch
  • Product (1): Product
  • Project (2): Project, ProjectType
  • Properity (1): Properity
  • Resource (2): Resource, ResourceType
  • Salary (3): SalaryPeriod, SalaryTRX, SalaryTrxType
  • Sale (3): SalesMan, SalesOrder, SalesOrderDetail
  • Section (1): Section
  • Sheet (1): Sheet
  • Stock (3): StockReview, StockReviewDetail, StockReviewType
  • Store (2): Store, StoreLocation
  • Sub (5): SubCode, SubGroupItem, SubJournalType, SubLocation, SubStore
  • Supplier (1): Supplier
  • Survey (5): Survey, SurveyGrade, SurveyQuestion, SurveyResult, SurveyResultDetail
  • System (1): SystemParameter
  • T (4): TMPAuditAccount, TMPAuditChart, TMPAuditDevice, TMPAuditUsers
  • Trx (1): TrxType
  • User (2): USERS, Users1
  • Work (1): WorkType
```

The above is effectively the Web application which enables you a complete interaction with your data - Create, Update and Delete.

This particular application will show a Menu for Asset, Audit, etc - with corresponding  tables. There is no Menu for a single table.

If the result shows no tables, it is impossible to show any data on the Web.


[![alt text](https://github.com/platipusica/msaccess2web/blob/main/output.gif?raw=true)](https://raw.githubusercontent.com/platipusica/msaccess2web/refs/heads/main/output.gif)




File size for this example:
```
C:\Users\dba\Downloads>dir access_database.accdb
 Volume in drive C has no label.
 Volume Serial Number is FEBB-5BF6

 Directory of C:\Users\dba\Downloads

08/06/2026  06:36 PM         8,388,608 access_database.accdb
               1 File(s)      8,388,608 bytes
               0 Dir(s)  40,732,401,664 bytes free
```

File type:
```
C:\Users\dba\Downloads>type access_database.accdb
Standard ACE DB...
```




## Features

- Works on Windows only
- Preserves Access compatibility


## Commercial support

This project is maintained for enterprise MS Access modernization projects.

Contact if:
- you are stuck on Access
- cannot migrate easily
- fear rewriting everything
- need MS Access data on the Web


