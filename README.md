# DatingApp

## Introduction
This repo is for my work as I follow the Udemy course "[Build an app with ASPNET Core and Angular from scratch](https://www.udemy.com/course/build-an-app-with-aspnet-core-and-angular-from-scratch/)" created by [Neil Cummings](https://www.udemy.com/user/neil-cummings-2/)

### Sections

- [Software](#Software)
- [VSCode Extensions](#VSCode-Extensions)
- [DotNet commands](#DotNet-commands)
- [Entity Framework commands](#Entity-Framework-commands)
- [Node Commands](#Node-Commands)
- [Angular CLI commands](#Angular-CLI-commands)

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
6. [Angular Language Service](https://marketplace.visualstudio.com/items?itemName=Angular.ng-template) v11.2.9
7. [Angular Snippets (Version 11)](https://marketplace.visualstudio.com/items?itemName=johnpapa.Angular2) v11.0.0
8. [Bracket Pair Colorizer 2](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer-2) v0.2.0

## DotNet commands

Create a Solution based on the current directory
```
PS E:\DatingApp> dotnet new sln
```

Create a Web API under a new "api" sub-directory
```
PS E:\DatingApp> dotnet new webapi --output api
```

Add the Web API to the Solution
```
PS E:\DatingApp> dotnet sln add api
```

Allow sef-signed Dev certificates to be trusted
```
PS E:\DatingApp> dotnet dev-certs https --trust
```

Run the Web API (CTRL+C to exit)
```
PS E:\DatingApp> dotnet run --project api
```

## Entity Framework commands

NB: The following commands must be run from "api" sub-directory

Initial Create
```
PS E:\DatingApp\api> dotnet ef migrations add InitialCreate --output Data/Migration
dotnet ef database update
```
List migrations
```
PS E:\DatingApp\api> dotnet ef migrations list
```

Delete the database
```
dotnet ef database drop
```

## Node commands

Pre-Flight version check for Node.js and NPM
```
PS E:\DatingApp> node --version
PS E:\DatingApp> npm --version
```

Install the latest Angular CLI
```
PS E:\DatingApp> npm install -g @angular/cli
```

Replace Angular CLI with a specific version
```
PS E:\DatingApp> npm uninstall -g @angular/cli
PS E:\DatingApp> npm cache clean
PS E:\DatingApp> npm install -g @angular/cli@10.2.3
```

NB: Angular CLI options selected - Yes (to routing), CSS (for styling)

Install Font Awesome
```
PS E:\DatingApp\client> npm install font-awesome
```

## Angular CLI commands

Create the Angular client
```
PS E:\DatingApp> ng new client
```

Run the client (CTRL+C to exit)
```
PS E:\DatingApp\client> ng serve
```

Install Bootstrap
```
PS E:\DatingApp\client> ng add ngx-bootstrap
```

Create the Nav component
```
PS E:\DatingApp\client> ng g component nav --skip-tests
```

Create a Service
```
PS E:\DatingApp\client\src\app\_services> ng g service account --skip-tests
```

Create a Home component
```
PS E:\DatingApp\client\src\app> ng g component home --skip-tests
```