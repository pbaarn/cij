# Phase 1.1: Architecture & Setup

## 1. Real-Time Journeys Platform Overview
- **Source**: [Microsoft Learn — Real-Time Marketing Overview](https://learn.microsoft.com/en-us/dynamics365/customer-insights/journeys/real-time-marketing-overview)
- **Tags**: `Overview`, `Channels`, `Architecture`

### Core Concept
Customer Insights – Journeys unifies **event-driven triggers**, **segments**, and **multi-channel messaging** (email, SMS, push notifications, and custom channels) natively on **Microsoft Dataverse**. It connects directly with **Customer Insights – Data** unified customer profiles and **Copilot AI** to personalize every customer touchpoint in real time.

### Key Architectural Pillars
1. **Dataverse Foundation**: Runs directly on Dataverse tables (`Contact`, `Lead`, and unified `Customer Profile` from CI-Data), eliminating separate marketing-data sync silos.
2. **Real-Time Triggers vs. Segments**:
   - *Triggers*: React immediately to customer actions or Dataverse record changes (e.g., form submission, purchase, website visit, custom event).
   - *Segments*: Target groups based on demographic, behavioral, or unified profile attributes.
3. **Multi-Channel Orchestration**: Native support for Email, SMS, Push notifications, plus extensible Custom Channels.
4. **Copilot & AI**: Embedded AI for content ideas, segment creation, journey drafting, and form fill assistance.

### My Notes & Questions
- *(Add your takeaways or questions here as you read the Microsoft Learn page)*
