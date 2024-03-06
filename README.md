# Dynamic CSV Generator

## Description
Generate a CSV file for a MS SQL Server table. The solution contains a single function that given a connection string, table name, and file path, will create a CSV file containing the contents of the table.

It uses Linx's capabilities to run dynamic queries and write to text files. 

## Usage

#### Try it out
Select the GenerateCSVFromTable function, click Debug, supply values for ConnectionString, TableName, and FilePath parameters, and click Start.

#### Use it in your own Linx solution
Copy GenerateCSVFromTable to your solution and call it from anywhere.

## Limitations
#### Only works with MS SQL Server
To use it with other databases, change the connection type and SQL properties in the GetCSVHeader and GetCSVData functions.
#### Does not escape the delimiter and line feeds in source data
If the source data contains the delimiter and/or line feeds, the CSV file will be invalid. The function can be extended to cater for these scenarios.

## Contributing

For questions please ask the [Linx community](https://linx/software/community). 

## License

[MIT](https://github.com/linx-software/template-repo/blob/main/LICENSE.txt)
