# !FightClub (Not Fight Club) - Gamified Debate App (Revature Capstone, 2021)


[GitHub Repo](https://github.com/Not-Fight-Club)
## Overview
A full-stack gamified web application where users create characters and engage in asynchronous debates, live chat discussions, spectator voting, and rewards earning. Designed as a social platform with competitive elements, deployed to Azure using Docker and Kubernetes for scalability.

## Key Features
- Character creation (noun + adjective + weapon combinations)
- Public/private debate rooms with live chat and voting
- Spectator mode for non-participants
- !Bucks currency system with daily rewards and shop for upgrades/seasons
- Leaderboards and user profiles

## My Contributions
- Implemented login/register backend endpoints and authentication logic.
- Developed daily rewards system and user currency/rewards management.
- Configured Docker logging and containerization for deployment.
- Served as Scrum Master: Organized Kanban board, facilitated standups, resolved blockers for team of 5+.

## Tech Stack
- Frontend: Angular 2+
- Backend: .NET Core microservices, Entity Framework
- Database: Azure SQL
- Deployment: Azure DevOps, Docker, Kubernetes
- Other: Git, Scrum/Agile

## Code Example (Placeholder)
```csharp
// Example: Simple login endpoint (recreated from memory)
[HttpPost("login")]
public async Task<IActionResult> Login(LoginModel model)
{
    var user = await _userService.Authenticate(model.Username, model.Password);
    if (user == null) return Unauthorized();
    var token = _jwtService.GenerateToken(user);
    return Ok(new { Token = token });
}