# SQLite Encryption Using EFCore
This is real life example which demostrates how to use SQLite encrypted database using Entity Framework Core (EFCore). Example is using .Net Core 2.2 with EFCore 2.2.

SQLLite is small, fast file based database. It is built into all mobile phones and most computers. Although it is widely used in mobile devices, it can be used in websites with low to moderate workload.

One of the common requirement for SQLite is encryption. There are various options available for encryption and SQLCipher is one of them. 
This example is using SQLCipher. Encryption is applied to the database using [DBBrowser](https://sqlitebrowser.org/) for SQLite. DBBrowser for SQLite is free and open source tool to edit the SQLite files. 

Steps for using Encrypted SQLite database in your .Net application with EFCore. 

1  Add the reference of Microsoft.EntityFrameworkCore.Design in your project.

2  Add the reference of Microsoft.EntityFrameworkCore.Sqlite.Core. This is really important step. Don't add the reference of Microsoft.EntityFrameworkCore.Sqlite. Otherwise it will not work.

3  Add the reference of SQLitePCLRaw.bundle_sqlcipher. For encryption it is required.

4  Add the following line 
   <PackageReference Include="SQLitePCLRaw.bundle_green" Version="1.1.14" ExcludeAssets="All" />
   ExcludeAssets="All" is important otherwise it will not work. 



