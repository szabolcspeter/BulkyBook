# BulkyBook
ASP.NET MVC project (.NET6)

Main focus was on the below patterns and the relationship between them:

 - Repository Pattern
 - Unit Of Work Pattern 


Also, "Admin" and "Customer" areas have been configured and used.


Since the application has been implemented on my Arch Linux box (I prefer using Linux), you can run it like this:

    Step 1) fire up docker and start an SQL server container:
      
      docker run -e 'ACCEPT_EULA=Y' -e 'MSSQL_SA_PASSWORD=SqlServer12345678' -p 1433:1433 -v sqlvolume:/var/opt/mssql -d --name sqlserver mcr.microsoft.com/mssql/server:2019-latest

    Step 2) create DB
    
        cd BulkyBookWeb && dotnet ef database update
    
    Step 3) 

        dotnet watch run
    
