# Smoke App - Gamer Social Platform (Revature Project, 2021)

[GitHub Repo](https://github.com/08162021-dotnet-uta/P2_Group3)
## Overview
A social platform for gamers integrating the RAWG API to display game data, enabling users to discuss games, post comments, and interact in a forum-like environment. Focused on user authentication, content creation, and API consumption.

## Key Features
- Game search and display via RAWG external API
- User posts, comments, replies, and threaded discussions
- Login/register with secure authentication
- Form validation and error handling

## My Contributions
- Built login/register functionality with backend integration
- Designed frontend layouts and UI components for game display and discussions
- Handled API calls to RAWG and integrated data into the app
- Implemented form validation, Entity Framework database operations, and user session management

## Tech Stack
- Frontend: Angular 2+
- Backend: .NET Core, Entity Framework
- API: RAWG (external games API)
- Database: SQL Server/Azure SQL
- Other: Git, Scrum

## Code Example (Placeholder)
```csharp
// Example: RAWG API call integration (conceptual)
public async Task<List<Game>> GetGames(string searchTerm)
{
    var response = await _httpClient.GetAsync($"https://api.rawg.io/api/games?search={searchTerm}&key={_apiKey}");
    response.EnsureSuccessStatusCode();
    return await response.Content.ReadFromJsonAsync<List<Game>>();
}
