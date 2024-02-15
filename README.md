# Dynamic CSV Generator

## Description
You can dynamically generate CSVs for a table name on a SQL database. Pass in the table name and a CSV will be generated with the data contained in the table. This sample solution shows how you can dynamically create SQL queries with Linx, how you can create a CSV file for any table and you can then use that generated file for any purpose such as distribution, data migration or automation. Some enhancements might include allowing the process to build files based on a view. 

## Installation
Add your MS SQL Server Database Connection string to the Database_ConnectionString setting. 

This solution will only work for MS SQL databases - you can modify the solution to work with another database however, queries will have to be altered. Alter the queries in the following string components (expressions):
- GenerateCSV_FromTable > String_SQLQuery_Columns
- GenerateCSV_FromTable > String_SQLQuery_Data

## Usage

The GenerateCSV_FromTable function requires two parameters to be entered:
- Filelocation: Location of where the file will be generated
- Table: Table name from where the data must be pulled

Please note that the queries are dynamically created by Linx expressions and then executed int he ExecuteSQL components. You can alter these queries by altering expressions in the following components:
- GenerateCSV_FromTable > String_SQLQuery_Columns
- GenerateCSV_FromTable > String_SQLQuery_Data

## Contributing

For questions please ask the [Linx community](https://linx/software/community) or use the [Slack channel](https://linxsoftware.slack.com/archives/C01FLBC1XNX). 

## License

[MIT](https://github.com/linx-software/template-repo/blob/main/LICENSE.txt)
