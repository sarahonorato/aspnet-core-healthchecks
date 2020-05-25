# ASP.NET Core 3.1 Health Checks 
This is a demo for adding health checks for an API and a database (SQL Server).
The health check endpoint is created at /health. In this sample, no specific health checks are registered, if the app is capable of responding at the health endpoint URL, then it is healthy.
For the database, the health check is testing the connection.
And we also can see that is possible to have the body of the response customized!

## Prerequisites
- The [Microsoft.AspNetCore.Diagnostics.HealthChecks](https://www.nuget.org/packages/Microsoft.AspNetCore.Diagnostics.HealthChecks) package is referenced implicitly for ASP.NET Core apps;
- Creates a database and provides its connection string in the appsettings.json file;
- Has the following package references in its project file: [AspNetCore.HealthChecks.SqlServer](https://www.nuget.org/packages/AspNetCore.HealthChecks.SqlServer/);

## Examples on Postman
- Healthy api and healthy database
![HealthyStatus](https://github.com/sarahonorato/aspnet-core-healthchecks/blob/master/ExpectedResultsImages/Postman_Healthy.PNG)
- Healthy api and unhealthy database
![HealthyStatus](https://github.com/sarahonorato/aspnet-core-healthchecks/blob/master/ExpectedResultsImages/Postman_Unhealthy.PNG)

## Reference
[Microsoft Tutorial](https://docs.microsoft.com/en-us/aspnet/core/host-and-deploy/health-checks?view=aspnetcore-3.1)
