---
layout: project
title: Carcassonne Unity
---

{% assign page_data = site.data.board_game %}

{%
    include title.html
    title=page_data.name
    image=page_data.logo
    color=page_data.color
%}

## ℹ️ **Info**

- **Duration**: 2024. January - Now

- **Type**: Hobby Project

---

## 📚 **Description**

A digital adaptation of the [Carcassonne](<https://en.wikipedia.org/wiki/Carcassonne_(board_game)>) board game, developed using **Unity**.

The game supports up to **five players**, who can play either on a **single device** (local multiplayer) or via **network connection**.  
It is available on both **Android** and **desktop platforms**.
Currently, the game supports only the **Hungarian language**.

---

## ⚙️ **Current Features**

- **Base game** implementation
- Optional **Farming** feature
- **Expansions**:
  - **The River**
  - **The Abbot**
  - **Traders and Builders**

---

## 🚧 **Upcoming Features**

- Improved **tile designs**
- **UI improvements**
- **More game expansions**

---

## 💻 **Technologies**

| **Category**      | **Technologies**      |
| ----------------- | --------------------- |
| **Foundational**  | Unity ([1]), C# ([2]) |
| **Network**       | Unity Netcode ([3])   |
| **Visual Assets** | Blender ([4])         |

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

[1]: https://unity.com/
[2]: https://learn.microsoft.com/dotnet/csharp
[3]: https://unity.com/products/netcode
[4]: https://www.blender.org/
