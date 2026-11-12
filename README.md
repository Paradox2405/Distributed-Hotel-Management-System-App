# Distributed Hotel Management System: Android Table App

The customer-facing Android app of a three-part restaurant automation system. A tablet on each table lets guests browse the menu, order, call a waiter and leave feedback, with no waiter needed to take the order.

| Part | Repo |
|---|---|
| Admin web panel | [Distributed-Hotel-Management-System-Web](https://github.com/Paradox2405/Distributed-Hotel-Management-System-Web) |
| Mobile API | [Distributed-Hotel-Management-System-API](https://github.com/Paradox2405/Distributed-Hotel-Management-System-API) |
| **Android table app (this repo)** | Distributed-Hotel-Management-System-App |

## Features

- Menu by **category**, dish lists and **dish details** with ingredients
- Order dishes, see **current orders** and **order history**, with taxes applied
- **Call waiter** from the table
- **Favourite dishes**
- **Feedback** and feedback history
- Promotional **ads** and greetings, plus About and Contact screens
- Table number setup per device

## Tech stack

- **Java**, Android SDK (Eclipse ADT project, later opened in Android Studio)
- HTTP calls to the Mobile API (JSON)

## Project structure

```
src/com/comsats/restaurantandroid/
  activity/     menu, categories, dishes, dish detail, favourites, feedback,
                current orders, about, contact (+ list adapters)
  *.java        models: Dish, OrderDetail, Customer, Tax, TableNumbers, Ad, ...
res/            layouts and drawables
AndroidManifest.xml
```

## Running

1. Start the Mobile API and the admin web app on Tomcat.
2. The app points at `http://10.0.2.2:8080/RestAutomationMobile/`, which is the host machine from the emulator. Change it for real devices.
3. Open in Android Studio (import the Eclipse project) and run.
