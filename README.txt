https://docs.microsoft.com/en-us/dotnet/framework/data/adonet/data-providers
.NET Framework Data Providers
A .NET Framework data provider is used for connecting to a database, executing commands, and retrieving results. Those results are either processed directly, placed in a DataSet in order to be exposed to the user as needed, combined with data from multiple sources, or remoted between tiers. .NET Framework data providers are lightweight, creating a minimal layer between the data source and code, increasing performance without sacrificing functionality.

The following table lists the data providers that are included in the .NET Framework.

.NET Framework data provider|	Description

.NET Framework Data Provider for SQL Server|	Provides data access for Microsoft SQL Server. Uses the System.Data.SqlClient namespace.
.NET Framework Data Provider for OLE DB|	For data sources exposed by using OLE DB. Uses the System.Data.OleDb namespace.
.NET Framework Data Provider for ODBC|	For data sources exposed by using ODBC. Uses the System.Data.Odbc namespace.
.NET Framework Data Provider for Oracle|	For Oracle data sources. The .NET Framework Data Provider for Oracle supports Oracle client software version 8.1.7 and later, and uses the System.Data.OracleClient namespace.
EntityClient Provider|	Provides data access for Entity Data Model (EDM) applications. Uses the System.Data.EntityClient namespace.
.NET Framework Data Provider for SQL Server Compact 4.0.|	Provides data access for Microsoft SQL Server Compact 4.0. Uses the System.Data.SqlServerCe namespace.


Core Objects of .NET Framework Data Providers

The following table outlines the four core objects that make up a .NET Framework data provider.
Object|	Description
Connection|	Establishes a connection to a specific data source. The base class for all Connection objects is the DbConnection class.
Command|	Executes a command against a data source. Exposes Parameters and can execute in the scope of a Transaction from a Connection. The base class for all Command objects is the DbCommand class.
DataReader|	Reads a forward-only, read-only stream of data from a data source. The base class for all DataReader objects is the DbDataReader class.
DataAdapter|	Populates a DataSet and resolves updates with the data source. The base class for all DataAdapter objects is the DbDataAdapter class.


In addition to the core classes listed in the table earlier in this document, a .NET Framework data provider also contains the classes listed in the following table.

Object| 	Description
Transaction| 	Enlists commands in transactions at the data source. The base class for all Transaction objects is the DbTransaction class. ADO.NET also provides support for transactions using classes in the System.Transactions namespace.
CommandBuilder|	A helper object that automatically generates command properties of a DataAdapter or derives parameter information from a stored procedure and populates the Parameters collection of a Command object. The base class for all CommandBuilder objects is the DbCommandBuilder class.
ConnectionStringBuilder|	A helper object that provides a simple way to create and manage the contents of connection strings used by the Connection objects. The base class for all ConnectionStringBuilder objects is the DbConnectionStringBuilder class.
Parameter|	Defines input, output, and return value parameters for commands and stored procedures. The base class for all Parameter objects is the DbParameter class.
Exception|	Returned when an error is encountered at the data source. For an error encountered at the client, .NET Framework data providers throw a .NET Framework exception. The base class for all Exception objects is the DbException class.
Error|	Exposes the information from a warning or error returned by a data source.
ClientPermission|	Provided for .NET Framework data provider code access security attributes. The base class for all ClientPermission objects is the DBDataPermission class.










