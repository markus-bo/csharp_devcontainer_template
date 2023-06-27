# csharp_devcontainer_template
**Template devcontainer for C# asp.net core developement**

Runs on: *ubuntu 22.04*

Contains: *asp.net core 7.0*, *C# extension*, *C# dev kit*, *Git*

## Usage
### Locally with Visual Studio Code
- Prerequisites
    - Docker installed
    - VS code with extensions "Dev Containers" installed
- Open VS code
    - Select "reopen in container"
    - Takes a couple of minutes to pull image and build container

### Create projects
#### Create new console application
- run in terminal `dotnet new console -o your_project_name`

#### Create new asp.net core web API project
- run in terminal `dotnet new webapi -o your_project_name`
- accept dev certificate (Windows host only) `dotnet dev-certs https --trust` (for Linux see https://learn.microsoft.com/de-de/aspnet/core/security/enforcing-ssl?view=aspnetcore-7.0&tabs=visual-studio%2Clinux-ubuntu#ssl-linux)
- Run project template and check https://localhost:{port}/weatherforecast for JSON output


#### Create new Xunit test project
- run in terminal `dotnet new xunit -o PrimeService.Tests`

## Remark
Tested on Windows 10 with VS Code 1.79.2