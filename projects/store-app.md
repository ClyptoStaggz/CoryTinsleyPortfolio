# Store Web Application - E-Commerce API (Revature Project, 2021)

[GitHub Repo](https://github.com/08162021-dotnet-uta/CoryTinsley_Project1)

## Overview
A basic e-commerce web application with backend API for user accounts, product browsing, cart management, and order processing. Demonstrated full-stack development with user auth and data persistence.

## Key Features
- User registration and login
- Product catalog display
- Shopping cart and checkout flow
- Order history and management
- Secure API endpoints

## My Contributions
- Developed authentication and user account management
- Created order views, cart functionality, and checkout logic
- Built repositories for data access using Entity Framework
- Ensured API documentation and testing for reliability

## Tech Stack
- Frontend: JavaScript/HTML/CSS (basic)
- Backend: ASP.NET Core API, Entity Framework
- Database: SQL Server
- Other: Git, Agile practices, Local IIS Express

## Code Example (Placeholder)
```csharp
// Example: Order repository method
public async Task<Order> CreateOrder(Order order)
{
    _context.Orders.Add(order);
    await _context.SaveChangesAsync();
    return order;
}