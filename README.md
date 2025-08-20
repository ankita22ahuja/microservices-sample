Microservices architecture using ASP.NET Core Web API and Ocelot API Gateway, featuring:

Two independent microservices:

1. StudentAdmissionManagement

2. StudentAttendanceManagement

Model and controller setup for each, with simple GET endpoints returning static data.

A third project, SchoolAPIGateway, using Ocelot configured via Ocelot.json to act as the API gateway. 
The gateway routes incoming requests (e.g. /apigateway/AttendanceService) to the appropriate microservice.

Here’s a structured approach for turning a GitHub repo:

1. Create a New Repository (e.g. aspnetcore-microservices-sample).

2. Add Three Projects in the solution:

   i.) StudentAdmissionManagement

   ii.) StudentAttendanceManagement

   iii) SchoolAPIGateway

3. Include Models & Controllers for each service exactly as in the tutorial:

   i.) StudentAdmissionDetailsModel

   ii.) StudentAttendanceDetailsModel

   iii.) StudentAdmissionController and StudentAttendanceController

4. Configure Ocelot in the gateway:

   i.) Add services.AddOcelot() and app.UseOcelot() in Startup.cs

   ii.) Create Ocelot.json mapping upstream to downstream routes, 

