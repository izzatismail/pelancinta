# 🇲🇾 PelanCinta - A Malaysian Malay Wedding Checklist App — Copilot Context

## Project Overview
A simple, offline-first React Native app designed for Malaysian Malay weddings.
Focused on checklist-based planning with cultural relevance and clean UX.

**Dual Purpose:**
- A genuinely useful real-world app
- A strong portfolio project demonstrating senior-level engineering thinking

---

## Tech Stack
- **Framework**: React Native with Expo
- **Language**: TypeScript
- **State Management**: Zustand
- **Local Database**: SQLite (offline-first)
- **Navigation**: React Navigation
- **Optional (future)**: Firebase for backend sync

---

## Project Architecture
```
src/
├── screens/         # Full-page screen components
├── components/      # Reusable UI components
├── store/           # Zustand state management
├── db/              # SQLite database layer
├── utils/           # Helper functions
└── constants/       # Static data (templates, categories, etc.)
```

**Key Architectural Principles:**
- Clear separation: UI → State → Data Layer
- Prefer simplicity over abstraction
- Build for current needs, not hypothetical scale
- Offline-first by default (no login required for MVP)

---

## Core MVP Features (v1)
- [ ] Wedding checklist (categorized)
  - Akad Nikah
  - Reception
  - Hantaran
  - Legal tasks
- [ ] Mark tasks as complete
- [ ] Progress tracking (%)
- [ ] Countdown to wedding date
- [ ] Offline-first local storage
- [ ] Preloaded "Malay wedding template"

---

## Planned Evolution
| Version | Features |
|---------|----------|
| **v1 (MVP)** | Checklist, progress tracking, countdown, local persistence |
| **v1.1** | Timeline view, local notifications |
| **v1.2** | Budget tracker, vendor tracking |
| **v2+** | Smart checklist engine, optional Firebase sync (multi-user) |

---

## Coding Standards
- Use functional components with hooks
- Always type props with TypeScript interfaces
- Use `const`/`let` — never `var`
- Use arrow functions
- Type all function parameters and return values
- Keep components small and single-responsibility
- Use meaningful, descriptive variable/function names
- Use ES6+ syntax throughout

---

## What to Keep
- Simple, clean UX
- Offline-first design
- Fast interactions
- Minimal navigation complexity

## What to Avoid
- Vendor marketplaces
- Social feeds
- E-commerce features
- Over-engineering early architecture
- Premature abstraction

---

## Cultural Context
This app focuses specifically on **Malaysian Malay wedding workflows**, including:
- Akad Nikah preparation
- Hantaran (gift exchange) planning
- State-specific requirements (future)
- Local cultural logic not found in generic wedding apps

---

## AI Engineering Guidance
When assisting with this project, the AI must:
- ❌ Not blindly agree with decisions
- ✅ Challenge decisions when necessary
- ✅ Suggest alternatives when better options exist
- ✅ Enforce best practices (TypeScript safety, clean architecture)
- ✅ Prioritize simplicity, maintainability, and offline-first design
- ✅ Think long-term but implement minimally

---

## Supporting Docs
- `AGENTS.md` → Defines AI engineer behavior + architecture rules
- `README.md` → Product + technical overview + roadmap
- `CONTEXT.md` → This file (Copilot project context)

---

## Current Status
- ✅ Product defined
- ✅ Architecture decided
- ✅ MVP scope locked
- ✅ React Native + Expo setup complete
- ⏳ Ready for implementation (first screens + SQLite setup)