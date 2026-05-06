💍 PelanCinta - A Wedding Checklist App (MY)
A simple, offline-first wedding planning app tailored for Malaysian Malay weddings.
Built with React Native, this app focuses on what most wedding apps get wrong:👉 simplicity, speed, and cultural relevance

✨ Why this exists
Most wedding planning apps today are:
* Overloaded with features
* Vendor-driven (ads, marketplaces)
* Not relevant to local wedding customs
This project aims to solve that by being:
A clean, focused checklist app that actually helps users plan their wedding — without distractions.

🎯 Core Features
✅ Smart Checklist
* Preloaded tasks based on a typical Malay wedding:
    * Akad Nikah
    * Reception (Majlis Sanding)
    * Hantaran
    * Legal / documents
* Add, edit, delete tasks
* Mark tasks as complete

📊 Progress Tracking
* Visual completion percentage
* Motivational and simple

⏳ Countdown
* Days remaining to wedding date
* Always visible on home screen

📴 Offline-First
* No login required
* Works fully without internet
* Local database is the source of truth

🧱 Tech Stack
* React Native
* State management: Zustand
* Local storage: SQLite
* Navigation: React Navigation

🏗️ Architecture
The app follows a simple, scalable structure:
/src
  /screens        → UI (Home, Checklist, Timeline)
  /components     → Reusable UI components
  /store          → Zustand state
  /db             → SQLite access layer
  /models         → Type definitions
  /utils          → Helpers
Principles:
* Clear separation of concerns
* Minimal abstraction
* Offline-first by design

📱 Screens
* Home
    * Progress bar
    * Countdown
    * Upcoming tasks
* Checklist
    * Categorized task list
    * Quick toggle completion
* Timeline (planned)
    * Tasks grouped by time (e.g. “3 months before”)

🧩 Data Model (simplified)
ChecklistItem
* id
* title
* category (akad, reception, hantaran, legal)
* dueDate
* isCompleted
* notes

🚀 Roadmap
v1 (MVP)
*  Checklist with categories
*  Task completion
*  Progress tracking
*  Countdown
*  Offline storage

v1.1
*  Timeline view
*  Local notifications

v1.2
*  Budget tracker
*  Vendor management

v2.0
*  Smart checklist engine (dynamic by state/budget)
*  Multi-user sync (optional backend)

🇲🇾 Cultural Focus
Unlike generic wedding apps, this app includes:
* Akad Nikah preparation
* Hantaran planning
* Local legal processes (e.g. kursus kahwin)
Future versions may adapt tasks based on:
* State (Selangor, Kelantan, etc.)
* Wedding size/budget

⚠️ Non-Goals
To keep the app focused, the following are intentionally excluded:
* Vendor marketplaces
* Social feeds / inspiration boards
* E-commerce features

🧠 Development Philosophy
* Build for real usage, not feature count
* Optimize for speed and clarity
* Prefer simple solutions over complex ones
* Avoid premature scaling

🏁 Getting Started
# install dependencies
npm install

# run app
npx expo start

📌 Status
🚧 In active development

🤝 Contributions
This is a learning + portfolio project, but suggestions are welcome.

📄 License
MIT

💡 Final Note
This project is less about building “just another app”and more about building something thoughtful, usable, and intentional.