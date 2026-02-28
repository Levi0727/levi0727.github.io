---
layout: project
title: Shopping Tracker
---

{% assign page_data = site.data.shopping_tracker %}

{%
    include title.html
    title=page_data.name
    image=page_data.logo
    color=page_data.color
%}

## ℹ️ **Info**

- **Duration**: 2024. September – 2026. January

- **Type**: MSc Thesis

- **References**:
  - [MSc Thesis](/assets/shopping_tracker/msc_thesis.pdf)

---

## 📚 **Description**

Shopping Tracker is a household inventory app that scans barcodes and expiration dates
to log products and track stock levels, making household organization quicker and easier.

---

## ⚙️ **Current Features**

- **Barcode and expiration‑date scanning**

- **Household sharing** via in‑app invitations

- Multiple sign‑in options: **guest, email + password, Google Auth**

- **Charts** that visualize stored items

- Localization: **English, Hungarian, Spanish**

- **Light and dark themes**

- Home‑screen **widget** for the shopping list

- **App shortcuts** for quick access

- Community **product submissions** available to all users

- **Submission review screens** for admin users

- **In‑app notifications** for household invites and product‑submission decisions

- **Local caching** for offline use

- **Push notifications** for upcoming expirations

- **Product price tracking** for expected expenditure calculation

- **Storage history** for tracking stored items since account creation

- **Storage statistics** for visualizing monthly expenses and category-based cost distribution

---

## 🚧 **Upcoming Features**

- **Minor improvements** (in development)

- **Bug fixes** (in development)

---

## 💻 **Technologies**

| **Category**                | **Technologies**                                                                   |
| --------------------------- | ---------------------------------------------------------------------------------- |
| **UI Toolkits**             | Jetpack Compose ([1]) · Material 3 ([2]) · Glance ([3]) · Lottie Compose ([4])     |
| **Build & Language**        | Kotlin ([5]) · Gradle KTS ([6]) · KSP ([7])                                        |
| **Data Layer**              | Room ([8]) · Jetpack DataStore ([9]) · Firebase Firestore ([10]) · Supabase ([11]) |
| **Networking & API**        | Retrofit ([12]) · Ktor ([13]) · Kotlin Serialization ([14])                        |
| **Authentication**          | Firebase Auth ([15]) · Google Credential Manager ([16])                            |
| **Media & Visualization**   | Coil ([17]) · CameraX ([18]) · Charts-Android ([19]) · Apache POI OOXML ([20])     |
| **Machine Learning and AI** | Google ML Kit ([21]) · Firebase AI ([22])                                          |
| **Background Services**     | WorkManager ([23])                                                                 |
| **Dependency Injection**    | Hilt ([24])                                                                        |
| **Testing**                 | JUnit4 ([25]) · Espresso ([26]) · Compose UI Test ([27])                           |
| **Analytics**               | Firebase Analytics ([28])                                                          |

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
[3]: https://developer.android.com/jetpack/compose/glance
[4]: https://github.com/airbnb/lottie-android
[5]: https://kotlinlang.org/
[6]: https://docs.gradle.org/current/userguide/kotlin_dsl.html
[7]: https://github.com/google/ksp
[8]: https://developer.android.com/training/data-storage/room
[9]: https://developer.android.com/topic/libraries/architecture/datastore
[10]: https://firebase.google.com/docs/firestore
[11]: https://supabase.io/
[12]: https://square.github.io/retrofit/
[13]: https://ktor.io/
[14]: https://kotlinlang.org/docs/serialization.html
[15]: https://firebase.google.com/docs/auth
[16]: https://developer.android.com/guide/topics/connectivity/credential-manager
[17]: https://coil-kt.github.io/coil/
[18]: https://developer.android.com/training/camerax
[19]: https://https://github.com/dautovicharis/Charts
[20]: https://poi.apache.org/
[21]: https://developers.google.com/ml-kit
[22]: https://firebase.google.com/docs/ai-logic
[23]: https://developer.android.com/topic/libraries/architecture/workmanager
[24]: https://developer.android.com/training/dependency-injection/hilt-android
[25]: https://junit.org/junit4/
[26]: https://developer.android.com/training/testing/espresso
[27]: https://developer.android.com/jetpack/compose/testing
[28]: https://firebase.google.com/docs/analytics
