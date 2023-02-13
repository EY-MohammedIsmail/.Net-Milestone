# .Net-Milestone
Steps to run :
1.Create Database structure
2.Create new project in MVC
3.Perform this on Package manager console: Scaffold-DbContext "Data Source=server_name;Initial Catalog=database_name;Trusted_Connection=True;TrustServerCertificate=True" Microsoft.EntityFrameworkCore.SqlServer -OutputDir Models 
4.Provide connection string on application.json
5.Configue the service on middleware i.e Program.cs file ->builder.Services.AddDbContext<EmployeeContext>(options => options.UseSqlServer(builder.Configuration.GetConnectionString("DefaultConnection")));
6.Add the controllers using MVC with read/write using entity framework
7.run the program

