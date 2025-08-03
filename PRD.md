# Product Requirements Document (PRD)

**Product Name:** SilentPlate  
**Owner:** Abdelrahman Elsayed  
**Version:** 1.0  
**Last Updated:** August 2, 2025

---

## 1. Overview

SilentPlate is a retro-themed mobile app that helps users discover restaurants near them, view AI-generated summaries of public reviews (Google/Yelp), and leave private feedback for restaurants. The goal is to empower users with better dining decisions while reducing public review fatigue.

---

## 2. Goals & Objectives

- Allow users to find restaurants near their location
- Summarize reviews from public sources using AI
- Enable anonymous, private feedback to restaurants
- Minimize external API usage via caching strategies
- Provide a native, smooth experience on iOS and Android using KMM

---

## 3. Target Audience

- Restaurant-goers seeking faster, less noisy review experiences
- Foodies looking to discover hidden gems
- People hesitant to leave public reviews

---

## 4. Key Features (MVP)

### 4.1 Onboarding
- Welcome screen with branding
- Permissions request (location)

### 4.2 Map View
- Show user’s current location
- Nearby restaurant pins via Google Places API
- Cuisine filtering

### 4.3 Restaurant Profile
- Name, location, rating, photos
- AI-generated review summary
- Button to leave private feedback

### 4.4 Feedback Submission
- Simple thumbs up/down
- Optional free text input
- Stored privately (linked to place, not user)

### 4.5 Caching System
- **In-memory:** Session cache
- **Local:** SQLDelight for recent places (1–7 day TTL)
- **Remote:** Supabase for shared summaries & metadata

---

## 5. Technical Stack

**Frontend:**
- Android: Jetpack Compose
- iOS: SwiftUI

**Shared Code (KMM):**
- Kotlin Multiplatform Mobile
- SQLDelight (local cache)
- Ktor Client (networking)
- kotlinx.serialization

**Backend:**
- Supabase (database, auth, API)
- OpenAI (AI review summarization)

---

## 6. Non-MVP Features (Backlog)

- Loyalty & rewards system
- Restaurant dashboard
- Public review aggregation feed
- User profiles and history

---

## 7. Monetization

- Freemium model
- Premium tier (save favorites, advanced filters)
- Restaurant dashboard subscription (B2B)

---

## 8. Analytics & Feedback

- Firebase / Mixpanel for usage tracking
- In-app survey for continuous feedback

---

## 9. Success Metrics

- Time-to-first discovery interaction
- Summary read-through rate
- Feedback submission volume
- API cost per user kept under target

---

> This PRD will evolve as we begin development and gather feedback from early users and stakeholders.