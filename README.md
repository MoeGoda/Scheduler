# Building REST APIs using ASP.NET Core and Entity Framework Core
Frameworks - Packages - Patterns - Features used
<ul>
<li>ASP.NET Core</li>
<li>Entity Framework Core</li>
<li>Entity Framework Migrations - Code First</li>
<li>Repository pattern</li>
<li>FluentValidation</li>
<li>Automapper</li>
<li>Global exception handler</li>
<li>Cors</li>
</ul>
<h3>Installation Instructions (1)</h3>
<ul>
<li>Install <a href="https://www.microsoft.com/net/core" target="_blank">.NET Core</a></li>
</ul>

<h3>Installation Instructions (2) - Visual Studio</h3>
<ol>
<li>Open the solution in VS 2017</li>
<li>Open Package Manager Console and navigate to Scheduler.API by typing cd <i>path_to_Scheduler.API</i></li>
<li>Modify the connection string in <i>appsettings.json</i> to reflect your database environment</li>
<li>run the following commands
<ol>
<li><b>Add-Migration Initial</b></li>
<li><b>Update-Database</b></li>
</ol>
</li>
<li>Build and run the Scheduler.API project</li>
</ol>

<h3>Installation Instructions (2) - Without Visual Studio</h3>
<ol>
<li>Clone or download the repository</li>

<li>Open a terminal/cmd</li>
<li>Open <i>Scheduler.API</i> folder in your favorite text editor (preferably VS Code). If you get a message <i>Required assets to build and debug are missing from your project. Add them?</i>, click Yes</li>
<li>Navigate to Scheduler.Model and run <b>dotnet restore</b></li>
<li>Navigate to Scheduler.Data and run <b>dotnet restore</b></li>
<li>Navigate to Scheduler.API and run <b>dotnet restore</b></li>
<li>If you haven't SQL Server <i>(Linux or MAC)</i> set "InMemoryProvider": <b>true</b> in the <i>appsettings.json</i> file and skip to the last step</li>
<li>Modify the connection string in <i>appsettings.json</i> to reflect your database environment</li>
<li>While at Scheduler.API run the following commands
<ol>
<li><b>Add-Migration Initial</b></li>
<li><b>Update-Database</b></li>
</ol>
</li>
<li>While at Scheduler.API run <b>dotnet run</b></li>
</ol>
