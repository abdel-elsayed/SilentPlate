# SilentPlate

**Interactive restaurant review application**

---

## ✅ Objective

Build a mobile-first app where users can:
- Discover restaurants via an interactive map
- View AI-generated summaries of public reviews
- Leave private feedback for restaurants (buffered before going public)
- *(Future)* Join loyalty programs, access restaurant profiles, and more

**Tech stack:**  
Kotlin Multiplatform Mobile (KMM) for shared logic  
SwiftUI for iOS & Kotlin for Android frontends

---

## 📅 Phase 0: Project Planning

### 1. Define Core Features (MVP)
- Interactive map showing nearby restaurants
- Tap restaurant pin to view profile and AI-generated review summary

### 2. Define Non-MVP (Post-launch)
- Loyalty/rewards integration
- Public review feeds
- Chat with restaurant
- Points redemption system

### 3. Define Personas
- **Primary:** App Users / Diners
- **Secondary:** Restaurant Owners / Managers (future onboarding)

---

## 🚀 Phase 1: Technical Setup

### 1. Initialize Git Repository
- Setup GitHub / GitLab with dev, staging, main branches

### 2. KMM Project Setup
- Create base KMM project
- Shared module for business logic, networking, models
- iOS: Integrate via Swift Package Manager or CocoaPods
- Android: Integrate shared module via Gradle

### 3. Dependency Planning
- Ktor (networking)
- SQLDelight or Realm (offline/local storage)
- Koin / Kodein (DI)
- Jetpack Compose (Android UI)
- SwiftUI (iOS UI)
- Google Maps SDK (Android)
- MapKit (iOS)

---

## 🔧 Phase 2: Core Feature Development

### 1. Onboarding Flow
- Retro-styled welcome screen
- Explain app value proposition ("Find & review with AI")
- Request location permission

### 2. Map Screen
- Show user''s location
- Display nearby restaurants as pins (Google Places API or similar)
- Tap pin to open Restaurant Profile

### 3. Restaurant Profile Screen
- Show name, location, cuisine, photos
- Display AI-generated review summary (from scraped reviews)
- Call to Action: "Leave Private Feedback"

### 4. Feedback UI
- Short form: thumbs up/down, optional text
- Feedback submitted privately to system (simulated initially)
- Placeholder for review buffer feature

---

## 📋 Phase 3: Testing & QA

### Manual QA
- UI tests on Android and iOS
- Location permission flows
- Restaurant pin accuracy
- Offline behavior (if local storage)

### Automated
- Unit tests for shared logic (KMM)
- Snapshot tests for iOS UI
- Instrumented tests for Android

---

## 📊 Phase 4: Launch Prep

1. **App Store Setup**
   - Create App Store & Play Console entries
   - Prepare assets: icons, screenshots, description
2. **Analytics & Crash Reporting**
   - Firebase / Sentry / Mixpanel setup
3. **Marketing Page (Optional)**
   - Static landing page explaining app purpose and collecting emails

---

## 🎉 Post-Launch Plan

1. **Gather User Feedback**
   - Feedback loop inside app ("What would you improve?")
   - Track top-used features and drop-offs
2. **Prioritize Phase 2 Features**
   - Loyalty program
   - Public review aggregation
   - User accounts and history
3. **Explore Monetization**
   - Freemium model
   - Premium features (saved favorites, advanced filtering, loyalty perks)
   - Restaurant-facing dashboard (B2B model)

---

> *This document will evolve as the project progresses. Each section will be expanded with code architecture, wireframes, and task breakdowns as needed.*
