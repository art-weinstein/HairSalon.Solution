# Hair Salon

### By Art Weinstein

### A basic webpage created as an Epicodus project to test basic web development skills in C#.

## Technologies Used

* HTML
* CSS
* C#
* ASP.NET Core MVC
* NuGet
* MySql WorkBench
* Entity Framework Core

## Description

This program allows a user to create a list of hair stylists and their associated clients. The project was designed to test students on one-to-many relationships through the use of databases. Users will be able to create, delete, edit and view both stylists and clients. Links prompt the user to navigate through the website and input both stylist and client information which then get stored within the database. 

## Setup/Installation Requirements

1. [Clone](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository-from-github/cloning-a-repository) this repository.
2. Within VS code or similar software, create an "appsettings.json file with the "HairSalon" directory.
3. Within the appsettings.json file copy the following code and replace "EXAMPLE_PASSWORD" with your SQL workbench password.
```
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=art_weinstein;uid=root;pwd=EXAMPLE_PASSWORD;"
  }
}
```
4. Import the database:
- Open MySql Workbench
- In the navigator window on the left side, navigate to Administration and select Data Import/Restore.
- Under Import Options, select Import from Self-Contained File
- Navigate to "HairSalon.Solutions/art_weinstein.sql"
- Under Default Schema to be Imported To, click New and enter art_weinstein
- Select the "Import Progress" tab and click "Start Import."
- Select the Schemas tab within the Navigator and select "refresh" to view the database. 
5. Install the necessary dependencies:
- Open a powershell terminal and navigate to the HairSalon directory.
- type ```dotnet add package Microsoft.EntityFrameworkCore -v 5.0.0```
- type ```dotnet add package Pomelo.EntityFrameworkCore.MySql -v 5.0.0-alpha.2```
- type ```dotnet add package Microsoft.EntityFrameworkCore.Proxies -v 5.0.0 ```
6. enter ```dotnet build``` in your powershell terminal to build the program.
7. enter ```dotnet watch run``` to create a localhost in your browser and view the program. 

## Known Bugs

* No bugs known at the moment.

## License

* [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2021 Art Weinstein

## Contact Information

[Email](artur.weintsein@gmail.com)