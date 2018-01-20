﻿### 2.1 Release Note

### Changes

- Update packages
	- NHibernate 5.0.3
	- Npgsql 3.2.6
	- MySqlConnector 0.34.2
	- Dapper 1.50.4
	- ZKWeb.System.Drawing 4.0.1
	- MongoDB.Driver 2.5.0
	- Microsoft.EntityFrameworkCore 2.0.1
	- Microsoft.EntityFrameworkCore.Design 2.0.1
	- Microsoft.EntityFrameworkCore.InMemory 2.0.1
	- Microsoft.EntityFrameworkCore.Sqlite 2.0.1
	- Microsoft.EntityFrameworkCore.SqlServer 2.0.1
	- Npgsql.EntityFrameworkCore.PostgreSQL 2.0.1
	- Pomelo.EntityFrameworkCore.MySql 2.0.1
	- System.Security.Cryptography.Algorithms 4.3.1
	- Microsoft.CodeAnalysis.CSharp 2.4.0
	- Microsoft.DiaSymReader.Native 1.7.0
	- Microsoft.DiaSymReader.PortablePdb 1.4.0
	- Microsoft.CSharp 4.4.1
	- Microsoft.Extensions.DependencyModel 2.0.4
	- Microsoft.CodeAnalysis.CSharp 2.6.1
	- Microsoft.AspNetCore.Hosting.Abstractions 2.0.1
	- Microsoft.AspNetCore.Http.Abstractions 2.0.1
	- MySql.Data 6.10.5
- Bug fixes
	- Fix state didn't reset during EFCore dbcontext reusing
- Improve plugin system
	- Support disable automatic plugin relodaing
	- Provide a method to decide which plugin to load
- Improve ORM
	- Change dapper's mysql provider to MySqlConnector (previous is Pomelo.Data.MySql)
	- Support command logger (see IDatabaseContext.CommandLogger)
		- Dapper: Log insert, update, delete and select
		- EFCore: Log insert, update, delete and select
		- InMemory: No logging
		- MongoDB: TBD
		- NHibernate: TBD