# JokesWebApp

A simple ASP.NET Core MVC web application for creating, viewing, searching, editing, and deleting jokes. Includes user authentication and modern UI styling.

## Features
- User registration and login (ASP.NET Core Identity)
- Create, edit, and delete jokes (authorized users only)
- View all jokes
- Search jokes by question
- Responsive, modern design with custom CSS

## Technologies Used
- ASP.NET Core MVC (.NET 10)
- Entity Framework Core (SQLite)
- ASP.NET Core Identity
- Bootstrap (via lib folder)
- Custom CSS

## Getting Started

### Prerequisites
- [.NET 10 SDK](https://dotnet.microsoft.com/download)
- SQLite (optional, for direct DB access)

### Setup
1. Clone the repository or copy the project files.
2. Restore dependencies:
   ```
   dotnet restore
   ```
3. Apply database migrations:
   ```
   dotnet ef database update
   ```
4. Run the application:
   ```
   dotnet run
   ```
5. Open your browser and navigate to `https://localhost:5001` (or the URL shown in the terminal).

### Default Database
- The app uses a local SQLite database file: `app.db`.
- Connection string is in `appsettings.json`.

## Project Structure
- `Controllers/` - MVC controllers
- `Models/` - Data models (Joke, etc.)
- `Views/` - Razor views for each page
- `Data/` - Entity Framework DbContext and migrations
- `wwwroot/` - Static files (CSS, JS, libraries)

## Customization
- Update CSS in `wwwroot/css/site.css` for custom styles.
- Add or modify jokes via the web interface (requires login).

## License
This project is for educational/demo purposes.
