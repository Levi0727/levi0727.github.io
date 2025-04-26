---
layout: project
title: Terra Imperium
---

{% assign page_data = site.data.terra_imperium %}

{%
    include simple_title.html
    title=page_data.name
    icon=page_data.icon
%}

## ℹ️ **Info**

- **Duration**: 2023. February – 2024. January

- **Type**: BSc Project Lab, BSc Thesis

- **References**:
  - [BSc Thesis](/assets/terra_imperium/bsc_thesis.pdf)
  - [Github page](https://github.com/pasztork/Polytopia-Clone/tree/web-dev)

---

## 📚 **Description**

Terra Imperium is a turn-based strategy game designed to be played
by containerized AI agents through a network connection to a game server.

The development began as a team project for the BSc Project Lab course,
where we originally created the game for human players in a local pass-and-play format.  
The gameplay draws heavy inspiration from the [Civilization](https://civilization.2k.com/civ-vi/)
series and [The Battle of Polytopia](https://polytopia.io/).
We also implemented a logging system that recorded every move, state, and interaction.

For my BSc Thesis, I continued the project individually, extending it to support AI agents.  
This involved developing a replay system to rewatch matches,
creating a web portal for game configuration and AI submissions,
and containerizing the game environment for deployment.
I also created a simple AI agent to test the other components of the system.

---

## ⚙️ **Features**

### 🎮 Game

- Up to 4 players
- Last-man-standing win condition
- Strategic gameplay featuring:
  - 5 different map tiles
  - 7 types of troops
  - 6 types of buildings
  - Resources: money, material, food
  - Tech tree for upgrades
- Custom map generation algorithm

### 🗂️ Logging System

- Saves the full game state, including:
  - Generated map files
  - Game configurations
  - Player actions (moving, attacking, building, etc.)

### 🔁 Replay System

- Loads and visualizes saved game logs
- Replay controls:
  - Manual: step-by-step playback
  - Automatic: time-interval-based playback (adjustable speed)

### 🤖 Automation System

- Conducts tournaments configured through the web portal
- Manages AI agent connections
- Handles data transmission between server and clients

### 🧠 AI Agents

- Run in isolated containers
- Communicate with the game server over the network
- Can be written in any programming language
  - Must implement the required interface defined by the server

### 🌐 Web Portal

- Authentication
- AI agent uploads
- Displays past tournament results
- Admin functionalities:
  - Tournament creation and evaluation
  - User management

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

| **Category**          | **Technologies**                                                  |
| --------------------- | ----------------------------------------------------------------- |
| **Foundational**      | C# ([1]) · .NET Core ([2])                                        |
| **Serialization**     | JSON ([3])                                                        |
| **Game UI Framework** | Unity ([4])                                                       |
| **Web Portal**        | ASP.NET Core ([5]) · ASP.NET Identity ([6]) · Blazor Server ([7]) |
| **Networking**        | WebSocket ([8])                                                   |
| **AI Agent**          | Python ([9])                                                      |
| **Containerization**  | Docker ([10])                                                     |

---

## 📸 **Feature Showcase**

{% include feature_shortcut.html features=page_data.features %}

{% for feature in page_data.features %}
{%
    include feature.html
    title=feature.title
    icon=feature.icon
    description=feature.description
    images=feature.images
%}
{% endfor %}

[1]: https://learn.microsoft.com/dotnet/csharp
[2]: https://dotnet.microsoft.com/en-us/
[3]: https://www.json.org/json-en.html
[4]: https://unity.com/
[5]: https://learn.microsoft.com/aspnet/core
[6]: https://learn.microsoft.com/en-us/aspnet/identity/overview/getting-started/introduction-to-aspnet-identity
[7]: https://learn.microsoft.com/en-us/aspnet/core/blazor/hosting-models?view=aspnetcore-9.0#blazor-server
[8]: https://learn.microsoft.com/en-us/aspnet/core/fundamentals/websockets
[9]: https://www.python.org/
[10]: https://www.docker.com
