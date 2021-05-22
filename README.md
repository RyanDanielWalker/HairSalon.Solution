# _Eau Claire's Salon_

#### _A C# web application to help keep track of Stylists and Clients using a database_

#### By _Ryan Walker_

## Description
This application will allow Eau Claire to manage information about the Stylists they employ and the Clients that a Stylist services. This application allows for the creation, viewing, editing, and deleting of Stylists and Clients while connecting to a database. Client information can be accessed while looking at the details of any Stylist.  

## Setup and Use

### Prerequisites
* [.NET 5 SDK](https://dotnet.microsoft.com/download/dotnet/5.0)
* A text editor like [VS Code](https://code.visualstudio.com/)
* A command line interface like Terminal or GitBash to run and interact with the console app.
* [MySQL Workbench](https://www.mysql.com/products/workbench/)

### Creating a database using SQL via MySQL
1. In the `Navigator>Administration` window of MySQL Workbench, select `Data Import/Restore`
2. In `Import Options` select `Import from Self-Contained File`
3. Navigate to the `HairSalon.Solution/ryan_walker.sql` file 
4. Under `Default Schema to be Imported To` select `New` 
5. Enter the name of your database following this naming convention `schema_name`
6. Click `Start Import`

### Connecting project to database via appsettings.json
1. In the production folder `HairSalon.Solution/HairSalon` create a file called `appsettings.json`
2. Add the following code:`{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;database={YOUR_SCHEMA_NAME};uid=root;pwd={YOUR_PASSWORD};"
  }
}`
   * Fill in your the name of your schema and your MySQL Workbench password, omitting the curly braces

### Installation
1. Clone the repository: `$ git clone https://github.com/RyanDanielWalker/HairSalon.Solution`
2. Navigate to the `HairSalon.Solution/` directory on your computer
3. Open with your preferred text editor to view the code base
4. To run the app:
    * Navigate to `HairSalon.Solution/HairSalon` in your command line
    * Run the command `dotnet restore` to restore the dependencies that are listed in the .csproj
    * Run the command `dotnet build` to build the project and its dependencies into a set of binaries
    * Finally, run the command `dotnet run` to run the project!
    * Note: `dotnet run` also restores and builds the project, so you can use this single command to start the app
    * View the application via your preferred web browser by visiting `localhost:5000/`


## Known Bugs
There were no bugs found.

## Technologies Used
* ASP .NET Core MVC
* C#
* VS Code
* MS Test

### License

MIT

Copyright (c) 2021 _Ryan Walker_

## Contact Information
[Ryandanielwalker@gmail.com](mailto:ryandanielwalker@gmail.com)




