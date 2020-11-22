[![.NET Core Logo](https://dotnet.microsoft.com/static/images/redesign/downloads-dot-net-core.svg?v=U_8I9gzFF2Cqi5zUNx-kHJuou_BWNurkhN_kSm3mCmo)](http://meanjs.org/)

This project is as start point with .NET framework.

# Prerequisites
Make sure you have installed all of the following prerequisites on your development machine:
* Visual Studio Community 2019 (https://visualstudio.microsoft.com/fr/downloads/)
* .NET Core 3.1 SDK (https://dotnet.microsoft.com/download/)

## Check you version of dotnet CLI
```batch
dotnet --info
```
You should have 3.1 .NET Core SDK installed.

# Quick Start
## Clone the GitHub repository and move to the created directory
```bat
git clone https://github.com/bosseludovic/students-union.git && cd students-union
```
## Create new solution
The solution is the projects container. [Solutions and projects in Visual Studio](https://docs.microsoft.com/en-us/visualstudio/ide/solutions-and-projects-in-visual-studio?view=vs-2019)
```batch
dotnet new sln -n cesi-students-union
```
## Create new web API project and add it to the solution
```batch
dotnet new sln -n cesi-students-union
dotnet new webAPI -o cesi-students-union -n cesi-students-union
dotnet sln add ./cesi-students-union/cesi-students-union.csproj
cd cesi-students-union
```
## Run the API
```batch
dotnet run
```
You can now browse to your first route
https://localhost:5001/weatherforecast

## Want to run all in once?
```batch
git clone https://github.com/bosseludovic/students-union.git && cd students-union
dotnet new sln -n cesi-students-union
dotnet new webAPI -o cesi-students-union -n cesi-students-union
dotnet sln add ./cesi-students-union/cesi-students-union.csproj
cd cesi-students-union
dotnet run
```

# Start Coding
## Unit tests
https://docs.microsoft.com/fr-fr/dotnet/core/testing/unit-testing-with-dotnet-test
### Create a unit test project and add it to the solution
Make sure you're in the root directory
```batch
cd ..
```
```batch
dotnet new xunit -o cesi-students-union.Tests -n cesi-students-union.Tests
dotnet add ./cesi-students-union.Tests/cesi-students-union.Tests.csproj reference ./cesi-students-union/cesi-students-union.csproj
dotnet sln add ./cesi-students-union.Tests/cesi-students-union.Tests.csproj
```

## Visual Studio
It's time to lauch Visual Studio! You can either run Visual Studio exe and then open you solution file (.sln) or directly run the solution file (.sln) with associated program.

## Nuget
It's the .NET package manager: https://docs.microsoft.com/fr-fr/nuget/quickstart/install-and-use-a-package-in-visual-studio .
You can even add package with the nuget package manager or the package manager console.

### Add NLog
https://github.com/NLog/NLog/wiki/Getting-started-with-ASP.NET-Core-3
#### Add NLog dependency
```batch
Install-Package NLog.Web.AspNetCore
```
#### Configure logs
https://github.com/nlog/NLog/wiki/Configuration-file    

## Swagger
### Swashbuckle
https://docs.microsoft.com/fr-fr/aspnet/core/tutorials/getting-started-with-swashbuckle?view=aspnetcore-3.1&tabs=visual-studio

```batch
Install-Package Swashbuckle.AspNetCore -Version 5.5.0
```

## Persistence
```batch
Install-Package Microsoft.EntityFrameworkCore.SqlServer
Install-Package Microsoft.EntityFrameworkCore.InMemory
```

Open the SQL server objects (View > SQL Server Object Explorer)
Create a new database.

Work with EF Core:
https://docs.microsoft.com/fr-fr/ef/core/

Create Models:
https://docs.microsoft.com/fr-fr/aspnet/core/data/ef-rp/intro?view=aspnetcore-5.0&tabs=visual-studio


### DbContext
https://github.com/rowanmiller/UnicornStore/blob/master/UnicornStore/src/UnicornStore/Models/UnicornStore/UnicornStoreContext.cs

## LINQ

## Dockerfile
https://docs.docker.com/engine/examples/dotnetcore/

echo. 2>Dockerfile
echo. 2>.dockerignore

## License
[The MIT License](LICENSE.md)
