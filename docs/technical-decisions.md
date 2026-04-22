# Technical Decisions

## 1. Mobile-first over web-first

The product is optimized for iOS and Android first. Web support is intentionally treated as a later track so the early product does not sacrifice mobile quality for premature cross-platform parity.

## 2. Local-first before cloud-first

Study flows, review behavior, and core progression are designed to work locally first. Cloud sync is layered on top for backup and continuity, not as the primary operational dependency.

## 3. PT-BR-first UX

The product is built around Brazilian Portuguese explanations and learning guidance, while keeping the codebase and technical docs in English.

## 4. Music as a real product surface

City Pop mode is not treated as a decorative add-on. It is part of the learning and engagement model.

## 5. Structured content instead of loose text blobs

Lessons, review blueprints, kana content, examples, and related metadata are modeled in structured content files and validated contracts.

## 6. Premium foundations before full commercialization

The repository already lays groundwork for entitlements and premium flows, but product quality and core study loop maturity remain ahead of aggressive monetization.

## Libraries Worth Highlighting

- Expo / React Native
- Expo Router
- expo-sqlite
- Drizzle ORM
- Zustand
- @tanstack/react-query
- @supabase/supabase-js
- react-native-purchases
- expo-notifications
- expo-audio
- jszip
- Storybook
- zod
- react-native-reanimated
- react-native-gesture-handler

## Integrations Worth Highlighting

- Supabase
- RevenueCat
- SQLite + Drizzle
- Anki-compatible `.apkg` import/export
- local notifications
- music-learning / City Pop mode

## Product Challenges

### Designing for Brazilian learners without making the app feel academic
The app needs to explain Japanese clearly in PT-BR while still feeling modern, fast, and product-led.

### Combining multiple loops in one coherent product
falaGENKI includes lessons, review, deck management, kana, and music-based study flows. Keeping those loops coherent is a core product challenge.

### Building a local-first experience that still scales to cloud backup
The app needs to remain dependable offline while still supporting future sync, account continuity, and premium portability.

### Teaching spoken Japanese more naturally
The product direction increasingly values casual spoken Japanese and practical communication, rather than only formal textbook-style progression.

### Balancing pedagogy with engagement
The challenge is not just content completeness, but making study sessions sustainable enough that users keep returning.

## Trade-offs

- mobile quality over early web parity
- deterministic local flows over cloud dependency
- structured content evolution over fast but messy content growth
- premium groundwork over immediate monetization pressure
- approachable, productized learning UX over textbook-style rigidity
