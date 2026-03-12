# 📚 Logic-Based Student Study Planner

An automated, intelligent study scheduler that uses **Prolog** to generate optimized study plans based on logical constraints like task difficulty, exam deadlines, and the student's available daily hours.

## 📂 Project Structure (Monorepo)
To keep our code clean and prevent conflicts, the project is strictly divided into four main directories:

* **`/client`**: The Frontend application (React + Vite). Contains the student dashboard, input forms for subjects/deadlines, and the generated study schedule view.
* **`/server`**: The Backend API bridge (Node.js/Express). Handles requests from the client, translates them into Prolog queries, and formats the optimized schedule response.
* **`/logic`**: The Prolog Engine. Contains `facts.pl` (scenario data for subjects) and `rules.pl` (the automated planning, priority calculation, and scheduling logic).
* **`/docs`**: Project documentation, including UML Diagrams (Use Case, Sequence, Activity) and initial data scenarios.

## 🚀 Workflow Guidelines
1.  **Do not cross folders:** If your task is Frontend, stay in `/client`. Do not modify `/logic` unless paired with the Logic team.
2.  **UML & Docs:** All non-code files and diagrams MUST go into the `/docs` folder.
3.  **MVP Scope:** For this phase, authentication is simulated on the frontend to focus our technical efforts on the core Prolog scheduling engine.

## 🛠️ Tech Stack
* **Frontend**: React (Vite)
* **Backend Bridge**: Node.js (Express)
* **Logic Engine**: SWI-Prolog
