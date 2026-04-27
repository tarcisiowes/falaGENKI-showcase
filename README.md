# falaGENKI

A mobile-first Japanese learning app for Brazilian Portuguese speakers, designed around local-first study flows, approachable SRS review, and music-driven engagement.

> This public repository is a product showcase. The production codebase is private.  
> This repo focuses on product direction, architecture, technical decisions, and delivery progress.

## Overview

falaGENKI is built for Brazilian learners who want a more approachable path into Japanese than traditional textbook-first or flashcard-only tools.

The product combines:

- PT-BR contextual explanations
- mobile-first lesson flows
- SRS review
- kana and early N5 foundations
- music-based learning loops
- optional cloud backup and premium foundations

The current product direction is intentionally mobile-first. Web support exists as a future possibility, but it does not drive the core architecture.

## What makes it different

- **Brazilian-first learning experience** instead of generic English-first UX
- **Local-first study loop** designed to work well before cloud sync is fully expanded
- **City Pop and music-based learning surfaces** as part of engagement and retention
- **Anki-compatible deck ecosystem** with import/export support
- **Guest-first progression** with optional account and sync boundaries
- **Casual spoken Japanese direction** as a real curriculum concern, not only JLPT-style memorization

## Product Areas

- Guided lessons
- Kana study and practice
- SRS review sessions
- Deck and card management
- Music learning / City Pop mode
- Progress, streak, XP, and study-plan support
- Optional login, backup, and premium foundations

## Demo Assets

### Screenshots

#### SplashScreens | App Icon
<div align="center">
  <img src="docs/screenshots/splash-background-light-with-logo.png" width="250">
  <img src="docs/screenshots/splash-background-dark-with-logo.png" width="250">
  <img src="docs/screenshots/app-icon.png" width="250">
</div>

---

#### Home
<div align="center">
  <img src="docs/screenshots/%5Bhome%5D-1.png" width="200">
  <img src="docs/screenshots/%5Bhome%5D-2%20plano%20de%20estudos-1.png" width="200">
</div>

---

#### Learn
<div align="center">
  <img src="docs/screenshots/%5Baprender%5D-1.0.png" width="200">
  <img src="docs/screenshots/%5Baprender%5D-1.1%20hiragana%20tabela.png" width="200">
  <img src="docs/screenshots/%5Baprender%5D-2%20pratica.png" width="200">
  <img src="docs/screenshots/%5Baprender%5D-2.1%20pratica.png" width="200">
  <img src="docs/screenshots/%5Baprender%5D-2.2%20pratica.png" width="200">
  <img src="docs/screenshots/%5Baprender%5D-3%20licao.png" width="200">
  <img src="docs/screenshots/%5Baprender%5D-3.2%20gramatica.png" width="200">
  <img src="docs/screenshots/%5Baprender%5D-3.2%20licao.png" width="200">
</div>

---

#### Music
<div align="center">
  <img src="docs/screenshots/%5Bmusica%5D-1.png" width="200">
  <img src="docs/screenshots/%5Bmusica%5D-2%20aprendendo%20musica.png" width="200">
  <img src="docs/screenshots/%5Bmusica%5D-3%20aprendendo%20musica.png" width="200">
</div>

---

#### Cards
<div align="center">
  <img src="docs/screenshots/%5Bcartas%5D-1.png" width="200">
  <img src="docs/screenshots/%5Bcartas%5D-12.png" width="200">
</div>

---

#### Profile
<div align="center">
  <img src="docs/screenshots/%5Bperfil%5D-1.png" width="200">
  <img src="docs/screenshots/%5Bperfil%5D-8.png" width="200">
  <img src="docs/screenshots/%5Bperfil%5D-10.png" width="200">
</div>


### Navigation GIF
A navigation GIF will be added later.

Recommended file name:

- `assets/gifs/falagenki-navigation.gif`

## Simple Architecture Diagram

```mermaid
flowchart TD
    A[Mobile App / Expo + React Native] --> B[Expo Router Navigation]
    A --> C[Local SQLite Database]
    C --> D[Drizzle ORM]
    A --> E[Lesson + Review Domain Logic]
    A --> F[Decks + .apkg Import/Export]
    A --> G[City Pop Learning Mode]
    A --> H[Profile / Study Plan / Streak]
    H --> I[Supabase Sync Layer]
    H --> J[RevenueCat Billing Foundation]
    A --> K[Storybook + CI + QA Workflow]
```

## Documentation

- [Architecture Summary](docs/architecture.md)
- [Technical Decisions](docs/technical-decisions.md)
- [Roadmap](docs/roadmap.md)
- [Changelog](docs/changelog.md)

## Why this repository is public

This repository exists to present the product direction, engineering thinking, and system design behind falaGENKI without exposing the private production codebase.

It is intended to show:

- product thinking
- architecture choices
- mobile-first system design
- delivery progress
- engineering depth behind the app

## Contact

If you are a recruiter, collaborator, or hiring manager and want to discuss the project, feel free to reach out through my GitHub or LinkedIn profile.
