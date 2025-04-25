---
layout: project
title: Restaurant Manager
---

{% assign page_data = site.data.restaurant_manager %}

{%
    include title.html
    title=page_data.name
    image=page_data.logo
    color=page_data.color
%}

## ℹ️ Info

- **Duration**: 2024. September – 2024. November

- **Type**: Team project for university coursework

---

## 📚 **Description**

This project was developed to provide a comprehensive system for restaurant management.
It enables restaurant staff to manage employees and monitor storage inventory,
while also offering features for customers to place delivery orders, and share feedback about their dining experience.

The application was built by a team of four.
I contributed to backend development, which handled client requests and managed data operations through a database.
Both the backend and the database are containerized, simplifying deployment and ensuring a consistent environment across all stages.

---

## ⚙️ **Features**

We developed two client applications: a mobile app for customers and a web interface for restaurant staff.
The mobile app was named _FoodJoy_, and its logo is also used as the icon for this webpage.

### 📱 Mobile App Features

- **Authentication**: Login with email and password
- **Profile Management**: View and edit name, email, address, and phone number
- **Food List**:
  - Displays available dishes with name, photo, and price
  - Items can be added to the shopping cart for ordering
- **Shopping Cart**:
  - Contains selected foods ready to order
  - Order can be submitted if address and phone number are provided
  - Tip percentage can also be set before submission
- **Orders**:
  - View active orders and order history
  - Download generated invoice after the order is completed
- **Coupons & Loyalty Points**:
  - Earn loyalty points after each order
  - Points can be used to redeem coupons
  - Coupons provide either a fixed amount or percentage-based discount
- **Reviews**:
  - Users can leave feedback with a 1–5 star rating
  - Optional written description can be included

### 🌐 Management App Features

- The web application includes two distinct views, tailored to the role of the logged-in employee.

- #### Waiter View

  - **Reservations**: Manage customer reservations
  - **In-house Orders**: Handle dine-in orders

- #### Manager View
  - **Order Management**: Accept/reject online orders, track order status
  - **Tables**: Add or remove tables
  - **Inventory**: Track and update ingredient stock
  - **Staff Accounts**: Create/delete accounts, assign roles (waiter/kitchen)
  - **Schedules**: Manage shifts and ensure staffing coverage
  - **Menu Items**: Manage the restaurant’s menu by creating and removing dishes
  - **Reviews**: View customer feedbacks
  - **Coupons**: Manage discount coupons
  - **Tip Distribution**: Choose how tips are shared at the end of the shift (evenly or shift-based)

---

{%
    include feature.html
    title=page_data.architecture.title
    icon=page_data.architecture.icon
    description=page_data.architecture.description
    images=page_data.architecture.image
%}

---

## 💻 **Technologies**

| **Category**            | **Technologies**                                       |
| ----------------------- | ------------------------------------------------------ |
| **Backend**             | ASP.NET Core ([1]) · Entity Framework ([2]) · C# ([3]) |
| **Database**            | Microsoft SQL Server (MSSQL) ([4])                     |
| **Client Applications** | Angular ([5]) · Ionic Angular ([6])                    |
| **Containerization**    | Docker ([7])                                           |

[1]: https://learn.microsoft.com/aspnet/core
[2]: https://learn.microsoft.com/ef/core
[3]: https://learn.microsoft.com/dotnet/csharp
[4]: https://www.microsoft.com/sql-server
[5]: https://angular.io
[6]: https://ionicframework.com/docs/angular/overview
[7]: https://www.docker.com
