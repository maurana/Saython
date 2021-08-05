![GitHub Logo](/logo.png)
<p align="center">
<a href="https://www.nuget.org/packages/SaythonMQ"><img src="https://img.shields.io/badge/creator-%40thisismaulanaa-blueviolet" alt="Creator"></a>
<a href="https://www.nuget.org/packages/SaythonMQ"><img src="https://img.shields.io/badge/made-indonesia-important" alt="Country"></a>
<a href="https://www.nuget.org/packages/SaythonMQ"><img src="https://img.shields.io/badge/licence-MIT-yellowgreen" alt="License"></a>
</p>

# Saython
The [Saython Technology](https://github.com/maurana/Saython) Karya Anak Bangsa created by Maulana Hasanudin

*Saython name was inspired by the Ta'Awudz sentence, namely أَعُوْذُ بِاللَّهِ مِنَ الشَّيْطَانِ الرَّجِيمِِْ*

*Which means "I seek refuge in Allah from the accursed Satan (Syaithan)". With the intention of Saython Technology can protect your code from the accursed Satan (Syaithan)*

> Technology List of Saython
* `Saython Framework` [Available v1.0.0](https://www.nuget.org/packages/SaythonFramework)
* `Saython Library`   [Available v1.0.0](https://www.nuget.org/packages/SaythonLibrary)
* `Saython Science`   **Coming Soon !** 
* `Saython Socket`    **Coming Soon !** 
* `Saython AI`        **Coming Soon !** 
* `Saython MQ`        [Available v1.0.0](https://www.nuget.org/packages/SaythonMQ)
* `Saython QL`        **Coming Soon !** 
* `Saython ML`        **Coming Soon !** 



## Saython Framework & Saython Library
A very cool Database Framework for all kinds of databases on .NET Core & .NET Framework technology
<p align="left">
<a href="https://www.nuget.org/packages/SaythonMQ"><img src="https://img.shields.io/badge/netcore-v3.1.0-brightgreen" alt="Tech"></a>
<a href="https://www.nuget.org/packages/SaythonMQ"><img src="https://img.shields.io/badge/netframework-v4.6.0-blueviolet" alt="Tech"></a>
<a href="https://www.nuget.org/packages/SaythonMQ"><img src="https://www.fuget.org/packages/SaythonMQ/badge.svg" alt="Build Status"></a>
<a href="https://www.nuget.org/packages/SaythonMQ"><img src="https://img.shields.io/nuget/v/SaythonMQ" alt="Latest Stable Version"></a>
<a href="https://www.nuget.org/packages/SaythonMQ"><img src="https://img.shields.io/nuget/dt/SaythonMQ?color=red&style=flat-square" alt="Total Downloads"></a>
</p>

> Supported DBMS SQL and NO SQL for now
- MySQL
- PostgreSQL
- SQL Server
- ODBC
- SQL Lite **Coming Soon !**
- MongoDB **Coming Soon !**

> Installation

Package Reference
```xml
<PackageReference Include="SaythonFramework" Version="1.0.0" />
<PackageReference Include="SaythonLibrary" Version="1.0.0" />
```
Package Manager
```bash
PM> Install-Package SaythonFramework -Version 1.0.0
PM> Install-Package SaythonLibrary -Version 1.0.0
```
.NET CLI
```bash
> dotnet add package SaythonFramework --version 1.0.0
> dotnet add package SaythonLibrary --version 1.0.0
```
Paket CLI
```bash
> paket add SaythonFramework --version 1.0.0
> paket add SaythonLibrary --version 1.0.0
```
Script & Interactive
```bash
> #r "nuget: SaythonFramework, 1.0.0"
> #r "nuget: SaythonLibrary, 1.0.0"
```
Cake Addin
```bash
#addin nuget:?package=SaythonFramework&version=1.0.0
#addin nuget:?package=SaythonLibrary&version=1.0.0
```
Cake Tool
```bash
#tool nuget:?package=SaythonFramework&version=1.0.0
#tool nuget:?package=SaythonLibrary&version=1.0.0
``` 
> Settings for use

Add the connection string according to the database used in *appsettings.json*

- **MySQL connection Example**
```json
{
  ...
  "ConnectionStrings": {
     "connstr": "server=localhost; port=3306; database=example; user=root; password=password"
  }
}
```

Set connection on Startup in *Startup.cs*
```c#
namespace Application
{
    public class Startup
    {
        // Add static property declaration
        public static string connStr
        {
            get;
            private set;
        }

        public void Configure(IApplicationBuilder app, IWebHostEnvironment env)
        {
            ...
            // Add initialize property
            connStr = Configuration.GetConnectionString("connstr");
        }
    }
}
```
