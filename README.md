# Water Reminder Application 💧📱

The Water Reminder App is a native Android utility engineered to help users maintain consistent and optimal hydration habits throughout their busy days. Built with a focus on simple workflows, fluid performance, and stable background tracking, the application allows users to configure automated notification loops, log precise daily intake milestones, and manage historical records.

---

## 🏗️ Architectural Pattern & Engineering

The application strictly implements the modern **MVVM (Model-View-ViewModel)** architectural pattern using structural native practices to separate concerns and handle clean lifecycle states:

1. **View Layer**: Handles UI layouts, XML data configurations, user click bindings, and active state animations rendered natively via **Android Studio**.
2. **ViewModel Layer**: Evaluates underlying state logic, holds hydration tracking matrices, and guarantees UI state persistence across device configuration modifications or screen rotations.
3. **Model / Data Persistence Layer**: Interacts with local system preferences and storage blocks to keep track of persistent water log parameters across active app restarts.

---

## 🛠️ Technology Stack & Environment

| Component | Technology | Implementation Context |
| :--- | :--- | :--- |
| **Language** | Kotlin 2.x | Native Application Engine (Type-Safe & Concurrent) |
| **Development IDE** | Android Studio / IntelliJ IDEA | Native Code Compilation, Layout Building, & Debugging |
| **Asynchronous Routines** | Kotlin Coroutines & Handlers | Dynamic background notification countdown tasks |
| **UI Framework** | Jetpack Core View Components | Responsive XML view hierarchies and Material theme variables |
| **Data Synchronization** | Shared Preferences / Local Storage | Lightweight relational data caching for persistent logs |

---

## 🧠 Core System Features

### 1. Dynamic Interval Notification Engine
* Empowers users to input targeted, custom minute intervals (e.g., every 30, 60, or 90 minutes) directly into the UI.
* Dispatches local background alarm threads that trigger accurate Android push notification alerts even when the device is idle.
* Provides quick cancel operations to tear down background notification loops instantly.

### 2. Hydration Intake Logger & Reset System
* Tracks real-time water bottle counts sequentially with straightforward add-and-subtract inputs.
* Implements a localized clear/reset switch that safe-wipes daily runtime trackers without corrupting separate historical logs.

### 3. Complete History CRUD Management
* Preserves past tracking data lists categorized distinctly by specific tracking sessions/days.
* Supports robust local CRUD functionality: Users can select existing log entries to dynamically execute an **Edit Count** mutation or perform a **Delete Day** cascade to clean up historical arrays.

---

## ⚡ Setup & Initialization Guide

### Prerequisites
* **Android Studio** (Latest Stable Version) or **IntelliJ IDEA**
* Android SDK (Target API Level 34 or higher)
* Gradle Version 8.5+

### Installation & Execution
1. Clone the repository source code to your machine:
   ```bash
   git clone <your-repository-url>
   cd water-reminder-app
