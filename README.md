# ASP.NET MVC 5 Reference Material

This is personal reference material collated for creating a ASP.NET web application using MVC architecture.


All documentation can be found in the [wiki](https://github.com/Tolvic/dotnet-mvc-csharp-asp.net/wiki).

## To Do



* Deployment 
    * Application
    * Database
    * Connecting the two
    * CI
    * CD
* Testing
    * How to run tests section of writing nunit tests with nunit
    * Test Coverage Metric 
    * Mocking and stubbing unit tests using Moq framework
    * Test database for unit tests
    * Function Testing using Selenium: https://www.c-sharpcorner.com/article/selenium-automation-test-cases-for-the-net-web-application/
* Controller
    * Full restful routing
    * Best Practice
    * How to use HTTP type other than get and post
    * Difference between IActionResult and ActionResult
* Views
    * Layout components
* Events - Asynchronous responses rather than having to take the user through redirect chainn
* Work through core concepts: https://docs.microsoft.com/en-us/aspnet/core/fundamentals/?view=aspnetcore-2.1


## Research Notes from Instagram code challenge
This site appears to be a fantastic resources for ASP.net, MVC, c#:
* http://www.tutorialsteacher.com

Step by step documentation has been created for setting up an ASP.net MVC 5 app, setting up unit tests using NUnit and setting up a databases. This can be found in a seperate repository [here](https://github.com/Tolvic/dotnet-mvc-csharp-asp.net/wiki).

### Generics
Angle brackets indicates that the class in question is generic and the underlying type will be defined later. Ergo, any time you see angle brackets in documentation, you must specify the type that will be passed to the class's methods in order to call them.

* Increases the reusability of the code.
* Generic are type safe. You get compile time errors if you try to use a different type of data than the one specified in the definition.
* Generic has a performance advantage because it removes the possibilities of boxing and unboxing.


More info can be found here:
* http://www.tutorialsteacher.com/csharp/csharp-generics

### interfaces
An interface in C# contains only the declaration of the methods, properties, and events, but not the implementation.

Lets say you have class. This class has a method that is defined as requiring a 32-bit integer parameter. This method works as expected. One day the requirements of this method changes and you would like to pass it a larger integer. Changing the method to expect a 64-bit integer would break all of the code written previously that uses this method.

An interface is like a contract stating what the class method will require and return and prevents the class from being changed in a way that breaks code that calls upon the method. If the class is changed in a way that not set in the interface, it will not compile.

Interfaces make your code easier to reuse, maintain, and extend.

Explanation of what an interface is and why they exist:
https://docs.microsoft.com/en-us/previous-versions/visualstudio/visual-studio-6.0/aa260635(v=vs.60)

Implementation:
http://www.tutorialsteacher.com/csharp/csharp-interface

### Test Environment
Documentation on using multiple environments in ASP.net:
https://docs.microsoft.com/en-us/aspnet/core/fundamentals/environments?view=aspnetcore-2.1

Truncating tables between each test:
https://stackoverflow.com/questions/3925783/jpa-how-to-truncate-tables-between-unit-tests
https://stackoverflow.com/questions/35655688/nunit-global-method-executed-before-each-test
