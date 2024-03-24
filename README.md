# 1. ASPNET CORE MVC PROJECT SETUP

## Create the project

First at all we need to install de dotnet CLI to create a new MVC project with the auth template.

```bash
dotnet new mvc --auth Individual -o proyecto
```

## Set HTTPS in development environment

```bash
dotnet dev-certs https --trust
```

## Visual Studio options

In case of use visual studio to create the aspnet core project, you can set up the same options:

![](./docs/img/1.1_vs_project-creation-auth.png)

![](./docs/img/1.2_vs_project-creation-https.png)


## Run Project

To run the project

```bash
dotnet run
```
![](./docs/img/1.3_first_execution.png)

## SET the database

https://learn.microsoft.com/en-us/ef/core/get-started/overview/install

To add EF Core to an application, install the NuGet package for the database provider you want to use.

In this case SQL SERVER:
```bash
dotnet add package Microsoft.EntityFrameworkCore.SqlServer
```

### GET ENTITY FRAMEWORK CORE TOOLS

```bash
dotnet tool install --global dotnet-ef

dotnet tool install --global dotnet-ef --version 7.0.17
```

```bash
dotnet add package Microsoft.EntityFrameworkCore.Design
```