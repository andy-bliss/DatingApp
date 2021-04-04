# DatingApp

## Introduction
This repo is for my work as I follow the Udemy course "[Build an app with ASPNET Core and Angular from scratch](https://www.udemy.com/course/build-an-app-with-aspnet-core-and-angular-from-scratch/)" created by [Neil Cummings](https://www.udemy.com/user/neil-cummings-2/)

## Software

The following software has been installed to support the content of the course:
1. [Visual Studio Code](https://code.visualstudio.com/download#) v1.55.0 (system setup)
2. [.Net SDK](https://dotnet.microsoft.com/download/dotnet/5.0) v5.0.2 (includes .Net Runtime 5.0.4)
3. [Node.js](https://nodejs.org/en/) v14.16.0 LTS
4. [Postman](https://www.postman.com/downloads/) win64 v8.1.0

## VSCode Extensions

The following extensions have been added to VSCode:
1. [C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp) for Visual Studio Code (powered by OmniSharp) v1.23.9
2. [C# Extensions](https://marketplace.visualstudio.com/items?itemName=kreativ-software.csharpextensions) v1.3.6
3. [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme) v4.6.0
4. [NuGet Gallery](https://marketplace.visualstudio.com/items?itemName=patcx.vscode-nuget-gallery) v0.0.24
5. [SQLite](https://marketplace.visualstudio.com/items?itemName=alexcvzz.vscode-sqlite) v0.11.1

## Starting Dot Net commands

Create a Solution based on the current directory
```
dotnet new sln
```

Create a Web API under a new "api" sub-directory
```
dotnet new webapi --output api
```

Add the Web API to the Solution
```
dotnet sln add api
```

Allow sef-signed Dev certificates to be trusted
```
dotnet dev-certs https --trust
```

Run the Web API (CTRL+C to exit)
```
dotnet run --project api
```
