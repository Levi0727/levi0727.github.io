---
layout: project
title: Cocktail Craft
---

{% assign page_data = site.data.cocktail_craft %}

{%
    include title.html
    title=page_data.name
    image=page_data.logo
    color=page_data.color
%}

## ℹ️ **Info**

- **Duration**: 2025. February – 2025. April

- **Type**: Kotlin Multiplatform-based Software Development course project

---

## 📚 **Description**

Cocktail Craft is a **cocktail discovery app** that helps users explore new drinks.
It enables users to search a wide selection of cocktails,
view their ingredients and preparation methods, and save their favorite recipes.

The app is available on both **Android and desktop** platforms.

Cocktails are provided by [The Cocktail DB](https://www.thecocktaildb.com/api.php).

---

## ⚙️ **Features**

- View **randomly recommended cocktails**

- **Search for cocktails** by name, including **speech-to-text** support

- Read **detailed information** about each cocktail

- **Mark cocktails as favorites** for easy access

- **Offline caching** for both the cocktail list and favorites

---

## 💻 **Technologies**

| **Category**             | **Technologies**                                                             |
| ------------------------ | ---------------------------------------------------------------------------- |
| **UI Framework**         | Jetpack Compose ([1]) · Material 3 ([2]) · Compose Material 3 Adaptive ([3]) |
| **Navigation**           | Compose Navigation ([4]) · Adaptive Navigation ([5])                         |
| **Dependency Injection** | Koin ([6])                                                                   |
| **Caching**              | Room (_Android_) ([7]) · SQLDelight (_Desktop_) ([8])                        |
| **Media**                | Coil ([9])                                                                   |
| **Networking**           | Ktor ([10]) · Kotlin Serialization ([11])                                    |
| **API**                  | **The Cocktail DB** ([12])                                                   |

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

[1]: https://developer.android.com/jetpack/compose
[2]: https://m3.material.io/
[3]: https://developer.android.com/develop/ui/compose/build-adaptive-apps
[4]: https://developer.android.com/jetpack/compose/navigation
[5]: https://developer.android.com/develop/ui/compose/layouts/adaptive/build-adaptive-navigation
[6]: https://insert-koin.io/
[7]: https://developer.android.com/training/data-storage/room
[8]: https://cashapp.github.io/sqldelight/
[9]: https://coil-kt.github.io/coil/compose/
[10]: https://ktor.io/
[11]: https://github.com/Kotlin/kotlinx.serialization
[12]: https://www.thecocktaildb.com/api.php
