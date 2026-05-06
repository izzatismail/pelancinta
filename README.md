# 💍 PelanCinta — Wedding Checklist App (MY)

> A simple, offline-first wedding planning app tailored for Malaysian Malay weddings.

Built with React Native, this app focuses on what most wedding apps get wrong: **simplicity, speed, and cultural relevance.**

---

## ✨ Why This Exists

Most wedding planning apps today are:
- Overloaded with features
- Vendor-driven (ads, marketplaces)
- Not relevant to local wedding customs

This project aims to solve that by being a clean, focused checklist app that actually helps users plan their wedding — without distractions.

---

## 🎯 Core Features

### ✅ Smart Checklist
- Preloaded tasks based on a typical Malay wedding:
  - Akad Nikah
  - Reception (Majlis Sanding)
  - Hantaran
  - Legal / documents
- Add, edit, delete tasks
- Mark tasks as complete

### 📊 Progress Tracking
- Visual completion percentage
- Motivational and simple

### ⏳ Countdown
- Days remaining to wedding date
- Always visible on home screen

### 📴 Offline-First
- No login required
- Works fully without internet
- Local database is the source of truth

---

## 🧱 Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | React Native (Expo) |
| Language | TypeScript |
| State Management | Zustand |
| Local Storage | SQLite |
| Navigation | React Navigation |
| Optional (future) | Firebase |

---

## 🏗️ Architecture

The app follows a simple, scalable structure:

```
src/
├── screens/        → UI (Home, Checklist, Timeline)
├── components/     → Reusable UI components
├── store/          → Zustand state
├── db/             → SQLite access layer
├── models/         → Type definitions
└── utils/          → Helpers
```

**Principles:**
- Clear separation of concerns
- Minimal abstraction
- Offline-first by design

---

## 📱 Screens

| Screen | Features |
|--------|----------|
| **Home** | Progress bar, countdown, upcoming tasks |
| **Checklist** | Categorized task list, quick toggle completion |
| **Timeline** *(planned)* | Tasks grouped by time (e.g. "3 months before") |

---

## 🧩 Data Model

```typescript
interface ChecklistItem {
  id: string
  title: string
  category: 'akad' | 'reception' | 'hantaran' | 'legal'
  dueDate: Date
  isCompleted: boolean
  notes?: string
}
```

---

## 🚀 Roadmap

### v1 — MVP
- [x] Checklist with categories
- [x] Task completion
- [x] Progress tracking
- [x] Countdown
- [x] Offline storage

### v1.1
- [ ] Timeline view
- [ ] Local notifications

### v1.2
- [ ] Budget tracker
- [ ] Vendor management

### v2.0
- [ ] Smart checklist engine (dynamic by state/budget)
- [ ] Multi-user sync (optional backend)

---

## 🇲🇾 Cultural Focus

Unlike generic wedding apps, this app includes:
- Akad Nikah preparation
- Hantaran planning
- Local legal processes (e.g. kursus kahwin)

Future versions may adapt tasks based on:
- State (Selangor, Kelantan, etc.)
- Wedding size/budget

---

## ⚠️ Non-Goals

To keep the app focused, the following are intentionally excluded:
- Vendor marketplaces
- Social feeds / inspiration boards
- E-commerce features

---

## 🧠 Development Philosophy

- Build for real usage, not feature count
- Optimize for speed and clarity
- Prefer simple solutions over complex ones
- Avoid premature scaling

---

## 🏁 Getting Started

```bash
# Install dependencies
npm install

# Run app
npx expo start
```

**Simulator shortcuts after `expo start`:**
- Press `i` — open iOS Simulator
- Press `a` — open Android Emulator
- Press `w` — open in web browser

---

## 📌 Status

🚧 **In active development**

---

## 🤝 Contributions

This is a learning + portfolio project, but suggestions are welcome.

---

> 💡 This project is less about building "just another app" and more about building something **thoughtful, usable, and intentional.**