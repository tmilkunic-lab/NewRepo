# Hospital Supply Chain Management System (HSCMS)

## Project Summary
The **Hospital Supply Chain Management System (HSCMS)** is an ASP.NET Core MVC web application designed to help hospital admins and staff manage medical supplies, orders, and supplier information efficiently and effectively. The proposed system will streamline the process of tracking current inventory levels, recording supply orders, managing vendors, and generating reports.
It aims to tackle issues of supply shortages,  overstocking of inventory items, and  transparency within the hospital’s supply chain. The HSCMS will demonstrate core ASP.NET concepts such as data modeling, dependency injection, CRUD operations, diagnostics, logging, and stored procedures through incremental weekly development. After completion, app will be deployed on Azure platform.

<style>

</style>

<table style="width: 100%; border-collapse: collapse;">
  <tr style="background-color: white;">
    <th style="border: 1px solid #ddd; padding: 8px;">Week</th>
    <th style="border: 1px solid #ddd; padding: 8px;">Concept</th>
    <th style="border: 1px solid #ddd; padding: 8px;">Feature</th>
    <th style="border: 1px solid #ddd; padding: 8px;">Goal</th>
    <th style="border: 1px solid #ddd; padding: 8px;">Acceptance Criteria</th>
    <th style="border: 1px solid #ddd; padding: 8px;">Evidence in README.md</th>
    <th style="border: 1px solid #ddd; padding: 8px;">Testing Method</th>
  </tr>
  <tr style="background-color: white;">
    <td style="border: 1px solid #ddd; padding: 8px;"><strong>10</strong></td>
    <td style="border: 1px solid #ddd; padding: 8px;">Modeling</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Create Models for <code>Product</code>, <code>Supplier</code>, and <code>Order</code></td>
    <td style="border: 1px solid #ddd; padding: 8px;">Define core entities and establish database schema for the hospital’s supply chain</td>
    <td style="border: 1px solid #ddd; padding: 8px;">- [ ] Entity classes created<br>- [ ] DbContext configured<br>- [ ] Migration applied<br>- [ ] Database updated successfully</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Code committed on GitHub; screenshots of entity classes and database tables in README </td>
    <td style="border: 1px solid #ddd; padding: 8px;">Run migration and verify tables in SQL Server or SQLite</td>
  </tr>
  <tr style="background-color: white;">
    <td style="border: 1px solid #ddd; padding: 8px;"><strong>11</strong></td>
    <td style="border: 1px solid #ddd; padding: 8px;">Separation of Concerns / DI</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Implement Repository and Service Layers using DI</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Separate data access logic from controllers for cleaner architecture</td>
    <td style="border: 1px solid #ddd; padding: 8px;">- [ ] Repository interfaces and classes created<br>- [ ] Registered in <code>Startup.cs</code>/<code>Program.cs</code> via DI<br>- [ ] Controllers using injected services</td>
    <td style="border: 1px solid #ddd; padding: 8px;">GitHub code + README explanation showing DI setup with code snippets</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Run app and verify data retrieval through repository methods</td>
  </tr>
  <tr style="background-color: white;">
    <td style="border: 1px solid #ddd; padding: 8px;"><strong>12</strong></td>
    <td style="border: 1px solid #ddd; padding: 8px;">CRUD</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Build “Product Management” Module (Add/Edit/Delete/View Products)</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Enable admin to manage hospital supply records from a simple UI</td>
    <td style="border: 1px solid #ddd; padding: 8px;">- [ ] Razor Views created for all CRUD ops<br>- [ ] Controller actions working<br>- [ ] Validation messages displayed</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Screenshots of forms and operations + explanation in README</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Manual browser testing for all CRUD actions</td>
  </tr>
  <tr style="background-color: white;">
    <td style="border: 1px solid #ddd; padding: 8px;"><strong>13</strong></td>
    <td style="border: 1px solid #ddd; padding: 8px;">Diagnostics</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Add Error Handling and Custom Error Pages</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Gracefully handle invalid inputs, missing pages, and database errors</td>
    <td style="border: 1px solid #ddd; padding: 8px;">- [ ] Custom error page (<code>Error.cshtml</code>)<br>- [ ] Middleware configured for exceptions<br>- [ ] Try-catch blocks for DB ops</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Code snippets and screenshots of custom error pages</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Induce deliberate errors (e.g., invalid ID) to check responses</td>
  </tr>
  <tr style="background-color: white;">
    <td style="border: 1px solid #ddd; padding: 8px;"><strong>14</strong></td>
    <td style="border: 1px solid #ddd; padding: 8px;">Logging</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Implement Logging for Admin Actions</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Track key events like product additions, deletions, and supplier updates</td>
    <td style="border: 1px solid #ddd; padding: 8px;">- [ ] Logging configured using built-in ASP.NET logger<br>- [ ] Log entries written to file or console<br>- [ ] Meaningful log messages created</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Log file or console output shown in README with explanation</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Perform CRUD operations and verify logs captured accurately</td>
  </tr>
  <tr style="background-color: white;">
    <td style="border: 1px solid #ddd; padding: 8px;"><strong>15</strong></td>
    <td style="border: 1px solid #ddd; padding: 8px;">Stored Procedures</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Use Stored Procedure for “Low Stock Report”</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Generate a report of products below a certain quantity threshold using SQL SP</td>
    <td style="border: 1px solid #ddd; padding: 8px;">- [ ] Stored Procedure created and executed through EF<br>- [ ] Results displayed in Razor View</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Screenshot of SP code and result table + README description</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Run SP manually in SQL Server and verify report correctness</td>
  </tr>
  <tr style="background-color: white;">
    <td style="border: 1px solid #ddd; padding: 8px;"><strong>16</strong></td>
    <td style="border: 1px solid #ddd; padding: 8px;">Deployment</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Deploy the application to  Azure App Service and publish documentation</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Make the app accessible online and provide final deliverables for grading</td>
    <td style="border: 1px solid #ddd; padding: 8px;">- [ ]  App deployed and reachable via URL<br>- [ ] README updated with deployment steps and live URL<br>- [ ] Release tag in GitHub</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Link to live app deployment logs/screenshots; final summary in README; GitHub release or tag</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Access app via public URL; run smoke tests (login, view products, generate report)</td>
  </tr>
</table>