---
title: Firebird
redirect_from:
  - /Firebird_Interbase/
---

Mono versions up to Mono 2.6 shipped a provider for the Firebird database. As of Mono 2.8, this provider is no longer distributed by Mono since the code in Mono's source tree was never updated by the Firebird maintainers.

Recent versions of Firebird bundle an up-to-date version of the database provider, and we strongly recommend developers to use that provider instead of using the bundled provider, even on versions 2.4 and 2.6 of Mono.

Info
----

-   Fully Managed ADO.NET Data Provider for Firebird database

-   The [Firebird Relational Database](http://firebirdsql.org) is is an independent project which uses source code based on the Interbase source code released by Borland under the Interbase Public License

-   Both the Firebird Relational Database and the Firebird .NET Data Provider can be downloaded from [here](http://sourceforge.net/projects/firebird/)

-   Does not require an unmanaged client library to use.

Support
-------

-   You can get support from the mailing list [firebird-net-provider](http://lists.sourceforge.net/lists/listinfo/firebird-net-provider). Please use this list for any questions that you may have about the provider

Using
-----

**Prerequisites**

-   Need a working mono and mcs

-   Need access to a Firebird Relational Database or you can download it from [here](http://firebirdsql.org/en/downloads/)

-   Get the Firebird .NET data provider from here as [firebird-net-provider](http://www.firebirdsql.org/en/additional-downloads/). Make sure the Firebird .NET data provider binary assembly FirebirdSql.Data.Firebird.dll is installed in the same place as the mono class libraries.

-   Connection String format:

<!-- -->

``` text
Database=databasefile.gdb;User=user;Password=pass;Dialect=3;Server=hostname
```

-   Connection String Parameters:

|Parameter Definition|Description|Example|
|:-------------------|:----------|:------|
|Server|hostname or network address of the Firebird SQL server|Server=localhost|
|Database|name of Firebird database file in which to connect|Database=C:\\PROGRAM FILES\\FIREBIRD\\EXAMPLES\\EMPLOYEE.GDB;|
|User|name of Firebird database user|User=SYSDBA|
|Password|password for Firebird database user|Password=masterkey|
|Dialect|Not sure. See Firebird net provider docs.|Dialect=3|

**C# Example**

``` csharp
using System;
using System.Data;
using FirebirdSql.Data.Firebird;
 
public class Test {
    public static void Main(string[] args) {
        string connectionString =
            "Database=C:\\PROGRAM FILES\\FIREBIRD\\EXAMPLES\\EMPLOYEE.GDB;" +
            "User=SYSDBA;" + "Password=masterkey;" +
            "Dialect=3;" + "Server=localhost";
 
        IDbConnection dbcon = new FbConnection(connectionString);
        dbcon.Open();
        IDbCommand dbcmd = dbcon.CreateCommand();
        string sql = "SELECT * FROM employee";
        dbcmd.CommandText = sql;
        IDataReader reader = dbcmd.ExecuteReader();
        while(reader.Read()) {
            object dataValue = reader.GetValue(0);
            string sValue = dataValue.ToString();
            Console.WriteLine("Value: " + sValue);
        }
 
        // clean up
        reader.Close();
        reader = null;
        dbcmd.Dispose();
        dbcmd = null;
        dbcon.Close();
        dbcon = null;
    }
}
```

-   Building C# Example:

-   Save the example to a file, such as, TestExample.cs

-   Build using Mono C# compiler:

<!-- -->

``` bash
mcs TestExample.cs -r System.Data.dll -r FirebirdSql.Data.Firebird.dll
```

-   Running the Example:

<!-- -->

``` bash
mono TestExample.exe
```

