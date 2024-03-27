<h1>Setup</h1>

<h2>Prerequisites</h2>
<ul>
  <li>Visual Studio must be previously installed.</li>
  <li>SQL Server Management Studio (SSMS) must be previously installed.</li>
</ul>

<h2>Steps</h2>
<ol>
  <li>
    <h3>Download the ZIP file:</h3>
  </li>
  
  <li>
    <h3>Unpack the ZIP file:</h3>
  </li>
  
  <li>
    <h3>Open in Visual Studio:</h3>
    <p>Navigate to the extracted folder and open the solution file (.sln) using Visual Studio.</p>
  </li>

  <li>
    <h3>Create Database in SSMS:</h3>
    <ul>
      <li>Open SQL Server Management Studio (SSMS).</li>
      <li>Connect to your SQL Server instance.</li>
      <li>Create a new database with a suitable name.</li>
      <li>Note the database name and ensure it matches the connection string in your application configuration.</li>
    </ul>
  </li>
  
  <li>
    <h3>Add Connection String:</h3>
    <ul>
      <li>Open the project in Visual Studio.</li>
      <li>Locate the configuration file (e.g., <code>appsettings.Development.json</code>) where you need to add your connection string.</li>
      <li>Add your connection string according to your database setup.</li>
    </ul>
  </li>
  

  
  <li>
    <h3>Apply Migrations:</h3>
    <ul>
      <li>Open Package Manager Console in Visual Studio (Tools -&gt; NuGet Package Manager -&gt; Package Manager Console).</li>
      <li>Enter the command to apply migrations:
        <pre><code>Add-Migration Init</code></pre>
      </li>
      <li>After the migration is added successfully, enter the command to update the database:
        <pre><code>Update-Database</code></pre>
      </li>
    </ul>
  </li>
  
  <li>
    <h3>Verify:</h3>
    <p>Ensure that there are no errors and the database is updated successfully.</p>
  </li>
</ol>

<p>These steps should complete the setup process. You should now be ready to use the application.</p>

