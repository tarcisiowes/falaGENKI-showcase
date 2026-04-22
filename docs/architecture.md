# Architecture Summary

falaGENKI uses a mobile-first architecture centered on local persistence and deterministic product flows.

## App Layer

- Expo + React Native
- Expo Router navigation
- TypeScript across app logic
- shared design system and theme primitives
- Storybook for UI review and component composition

## Data Layer

- local SQLite persistence
- Drizzle ORM for schema and repository structure
- structured content packs and review blueprints
- deterministic lesson, kana, and review-related contracts

## Product Logic

The application is organized around a few core loops:

- lesson progression
- SRS scheduling and review flow
- kana progression and practice
- deck import/export and review unlocking
- music-learning interactions
- progress, streak, XP, and study-plan support

## Cloud and Platform Layer

- Supabase for authentication and backup/sync foundations
- RevenueCat as the premium/billing foundation
- local notifications for reminder workflows

## Design and Validation Layer

- Storybook for UI review and composition-level validation
- Jest + React Native Testing Library for automated validation
- ESLint and TypeScript checks in the development workflow
- CI validation and ongoing runtime QA documentation

## Architectural Direction

The product is intentionally optimized for iOS and Android first.

Key architectural priorities:

1. Keep the core study loop useful offline.
2. Add cloud continuity without making the app cloud-dependent.
3. Model learning content as structured data instead of loose text blobs.
4. Keep music-learning flows as part of the product architecture, not as a superficial add-on.
5. Preserve a clear path for premium, sync, and content expansion without weakening the local-first foundation.
