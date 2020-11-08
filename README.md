[![.NET Core Logo](https://dotnet.microsoft.com/static/images/redesign/downloads-dot-net-core.svg?v=U_8I9gzFF2Cqi5zUNx-kHJuou_BWNurkhN_kSm3mCmo)](http://meanjs.org/)

This project is as start point with .NET framework.

## Prerequisites
Make sure you have installed all of the following prerequisites on your development machine:
* Visual Studio Community 2019 (https://visualstudio.microsoft.com/fr/downloads/)
* .NET Core 3.1 SDK (https://dotnet.microsoft.com/download/)

## Quick Start
### Check you version of dotnet CLI
```bash
$ dotnet --info
```
You should have 3.1 .NET Core SDKs installed.
### Clone the GitHub Repository
```bash
$ git clone https://github.com/bosseludovic/students-union.git
```
### Move to project directory
```bash
$ cd students-union
```
### Create new web API project
```bash
$ dotnet new webAPI -o cesi-students-union -n cesi-students-union
```
```bash
$ cd cesi-students-union
```
### Run the API
```bash
$ dotnet run
```
You can now browse to your first route
https://localhost:5001/weatherforecast

## Unit tests
https://docs.microsoft.com/fr-fr/dotnet/core/testing/unit-testing-with-dotnet-test
### Create a unit test project
Make sure you're in the root directory
```bash
$ cd ..
$ dotnet new xunit -o cesi-students-union.Tests
```

## Nuget
### Add NLog
https://github.com/NLog/NLog/wiki/Getting-started-with-ASP.NET-Core-3
** Add NLog dependency
```bash
ps> Install-Package NLog.Web.AspNetCore
```
** Configure logs
https://github.com/nlog/NLog/wiki/Configuration-file    

## Swagger

### Swashbuckle

https://docs.microsoft.com/fr-fr/aspnet/core/tutorials/getting-started-with-swashbuckle?view=aspnetcore-3.1&tabs=visual-studio

```bash
ps> Install-Package Swashbuckle.AspNetCore -Version 5.5.0
```

## Persistence

ps> Install-Package Microsoft.EntityFrameworkCore.SqlServer
ps> Install-Package Microsoft.EntityFrameworkCore.InMemory

### DbContext
https://github.com/rowanmiller/UnicornStore/blob/master/UnicornStore/src/UnicornStore/Models/UnicornStore/UnicornStoreContext.cs

## LINQ

## Dockerfile
https://docs.docker.com/engine/examples/dotnetcore/

echo. 2>Dockerfile
echo. 2>.dockerignore

## License
[The MIT License](LICENSE.md)
