# Music Library App

This repository contains the code for the Music Library App, a web application built using ASP.NET Core with CQRS pattern and Domain-Driven Design (DDD) principles for the backend, and Angular for the frontend. The app allows users to search, manage, and interact with a collection of music albums and artists.

## Table of Contents
- [Features](#features)
- [Technologies](#technologies)
- [Architecture](#architecture)
- [Getting Started](#getting-started)
- [Configuration](#configuration)
- [Running the Application](#running-the-application)


## Features
- View details of artists, albums, and songs
- Navigate through the web application using search functionality
- Manage the database by adding, updating, and deleting any of the entities

## Technologies
### Backend
- ASP.NET Core
- CQRS pattern
- Domain-Driven Design (DDD)
- Entity Framework Core

### Frontend
- Angular
- TypeScript
- HTML & CSS
- Bootstrap

### Database
- SQL Server

## Architecture
The backend of the application follows the CQRS pattern and DDD principles to ensure separation of concerns and scalability. The frontend is built using Angular for a responsive and dynamic user experience.

## Getting Started
### Prerequisites
- [.NET 6 SDK](https://dotnet.microsoft.com/download/dotnet/6.0)
- [Node.js and npm](https://nodejs.org/)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)

### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/dennisapascaritei/MusicLibraryApp.git
   cd MusicLibraryApp
   ```

2. Set up the backend:
   ```sh
   cd API
   dotnet restore
   dotnet build
   ```

3. Set up the frontend:
   ```sh
   cd ../MusicLibraryUI
   npm install
   npm run build
   ```

## Configuration
### Backend
1. Update the `appsettings.json` file in the `MusicLibraryApi` project with your SQL Server connection string:
   ```json
   {
     "ConnectionStrings": {
       "DefaultConnection": "Your SQL Server connection string here"
     }
   }
   ```

### Frontend
1. Update the `environment.ts` file in the `MusicLibraryUI/src/environments` directory with the API URL:
   ```typescript
   export const environment = {
     production: false,
     apiUrl: 'http://localhost:5000/api'
   };
   ```

## Running the Application
### Backend
1. Navigate to the `MusicLibraryApi` project directory and run:
   ```sh
   dotnet run
   ```
2. The API will be available at `http://localhost:5000`.

### Frontend
1. Navigate to the `MusicLibraryUI` project directory and run:
   ```sh
   ng serve
   ```
2. The application will be available at `http://localhost:4200`.

## Testing
### Backend
- To run the backend tests, navigate to the `MusicLibraryApi` project directory and run:
  ```sh
  dotnet test
  ```

### Frontend
- To run the frontend tests, navigate to the `MusicLibraryUI` project directory and run:
  ```sh
  ng test
  ```

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request for review.

### Steps to Contribute
1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Create a new pull request

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to open an issue if you have any questions or need further assistance.

---

Happy coding! 🎵

---

This README follows best practices for clarity and completeness, helping users set up, configure, run, and contribute to the project effectively.
