# BulkyBook
Simple MVC project (.NET6)

This is a simplest of simplest .NET6 MVC project implementing CRUD operations.



Since the application has been implemented on my Arch Linux box (I prefer using Linux), you can run it like this:

    Step 1) fire up docker and start an SQL server container:
      
      docker run -e 'ACCEPT_EULA=Y' -e 'MSSQL_SA_PASSWORD=SqlServer12345678' -p 1433:1433 -v sqlvolume:/var/opt/mssql -d --name sqlserver mcr.microsoft.com/mssql/server:2019-latest

    Step 2) run the application

        cd BulkyBookWeb && dotnet watch run
    