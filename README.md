# TodoApi

Create a web API with ASP.NET Core
https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-3.1&tabs=visual-studio

The project template creates a WeatherForecast API

A model is a set of classes that represent the data that the app manages
The model for this app is a single TodoItem class.

The database context is the main class that coordinates Entity Framework functionality for a data model. 
This class is created by deriving from the Microsoft.EntityFrameworkCore.DbContext class.
NuGet Package - Microsoft.EntityFrameworkCore.SqlServer
NuGet Package - Microsoft.EntityFrameworkCore.InMemory

In ASP.NET Core, services such as the DB context must be registered with the dependency injection (DI) container. 
The container provides the service to controllers.
Registered "TodoContext" in Startup.cs

Install Postman
https://www.getpostman.com/downloads/

Prevent over-posting
Productions apps typically limit the data that's input and returned using a subset of the model.
The subset of a model is usually referred to as a Data Transfer Object (DTO), input model, or view model.
The secret field needs to be hidden from this app, but an administrative app could choose to expose it.

############################################################################################################

Call an ASP.NET Core web API with JavaScript
https://docs.microsoft.com/en-us/aspnet/core/tutorials/web-api-javascript?view=aspnetcore-3.1

HTML page containing forms for creating and managing to-do items
Event handlers are attached to elements on the page. 
The event handlers result in HTTP requests to the web API's action methods. 
The Fetch API's fetch function initiates each HTTP request.