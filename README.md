# NomadBound

**A Premium Community Platform for Van Lifers and Digital Nomads**

NomadBound is a native iOS application built specifically for the nomadic community. Developed for the RevenueCat Shipyard Creator Contest, this platform addresses the unique challenges faced by van lifers by facilitating meaningful connections, enabling route based matching, and providing professional technical support in a secure, verified environment.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [The Problem](#the-problem)
3. [The Solution](#the-solution)
4. [Key Features](#key-features)
5. [Technical Architecture](#technical-architecture)
6. [RevenueCat Integration](#revenuecat-integration)
7. [Security and Safety](#security-and-safety)
8. [User Experience Highlights](#user-experience-highlights)
9. [Installation and Setup](#installation-and-setup)
10. [Team](#team)
11. [Hackathon Alignment](#hackathon-alignment)
12. [Roadmap](#roadmap)
13. [License](#license)

---

## Project Overview

NomadBound is more than a social app. It is a comprehensive platform designed to solve the isolation and logistical challenges inherent to van life. Built for creator Quin Gable and her 1.2M+ nomadic audience, NomadBound enables travelers to form authentic connections with others who share their mobile lifestyle, participate in community driven activities, and access professional van building expertise on demand.

---

## The Problem

Van life offers freedom and adventure, but it comes with unique social and practical challenges:

**Social Isolation:** Traditional dating and friend finding apps are location based. They connect nomads with people who remain stationary, resulting in connections that dissolve as soon as the nomad moves to the next destination.

**Safety Concerns:** The nomadic community is tight knit and protective. Open platforms feel unsafe, particularly for solo female travelers who need assurance that community members are verified and trustworthy.

**Technical Support Gaps:** When a van breaks down or requires specialized work (electrical, plumbing, solar installations), finding reliable, expert help on the road is difficult and stressful.

There is no single, trusted digital space that combines safe nomadic connection with practical, on demand life support.

---

## The Solution

NomadBound addresses these challenges through three core pillars:

1. **Nomadic Dating and Friend Finding:** Matches users based on upcoming travel routes rather than static proximity, ensuring connections with others moving in the same direction.

2. **Activity Based Community Building:** Enables nomads to organize and join real world meetups (climbing, hiking, coffee gatherings) at current or future locations.

3. **The Garage Professional Marketplace:** Provides on demand access to verified van building experts for paid technical consultations, solving urgent maintenance issues while on the road.

---

## Key Features

### 1. The Compass (Discovery and Matching)

**Nomadic Dating:** A dual mode interface that allows users to toggle between "Looking for Dates" and "Looking for Friends."

**Route Overlap Matching:** A proprietary algorithm that identifies when two users' travel paths will intersect in the next 30 days, creating opportunities for meaningful in person connections.

**Map and Swipe Views:** Users can browse nearby nomads on an interactive map or through a premium card based swipe interface.

### 2. Basecamp (Community Activities)

**Activity Feed:** A curated list of user generated meetups and events (sunrise yoga, group hikes, coffee meetups) organized by location and interest.

**RSVP and Group Chat:** Users can join events and coordinate logistics through integrated group messaging.

### 3. The Garage (Builder Marketplace)

**Expert Directory:** A searchable marketplace of verified van builders specializing in electrical work, plumbing, solar installations, carpentry, and more.

**Paid Consultations:** Users purchase one time consultation tokens via RevenueCat to unlock priority chat sessions with technical experts.

**Portfolio and Reviews:** Each builder profile includes past work, ratings, and community feedback to ensure quality and trust.

### 4. Verification and Security

**Invite Only Access:** All users must enter a unique invite code or request approval to join, maintaining community integrity.

**Video Selfie Verification:** A mandatory video verification step ensures every profile belongs to a real person, reducing bots and fake accounts.

**Verified Nomad Badge:** Profiles display a prominent verification badge, signaling trustworthiness to the community.

### 5. Messaging

**Organized Inbox:** Separate tabs for personal connections (dates and friends) and professional consultations (garage sessions).

**Priority Access:** Premium members and paid consultation purchasers receive prioritized messaging features.

---

## Technical Architecture

NomadBound is built using modern, industry standard technologies to ensure performance, scalability, and maintainability.

### Tech Stack

**Platform:** iOS 17.0+  
**Language:** Swift  
**UI Framework:** SwiftUI  
**Monetization SDK:** RevenueCat  
**Backend Services:** Firebase Cloud Firestore  
**Authentication:** Firebase Authentication  
**Storage:** Firebase Cloud Storage  
**Notifications:** Apple Push Notification Service (APNs)  

### Design Principles

**Native iOS Experience:** Utilizes SF Symbols, native navigation patterns, and iOS Human Interface Guidelines.

**Dark Mode First:** Default dark theme optimized for battery conservation during van travel.

**Performance Optimized:** Asynchronous data loading, image caching, and efficient state management for smooth performance on the road.

---

## RevenueCat Integration

Monetization is seamlessly integrated using the RevenueCat SDK, ensuring a reliable and scalable subscription infrastructure.

### Revenue Streams

#### 1. NomadPlus Subscription (Recurring Revenue)

**Monthly Plan:** $14.99 per month  
**Yearly Plan:** $119.99 per year (33% savings)

**Premium Features:**
* Unlimited matching and messaging
* Advanced route overlap visibility (see who will cross your path in the next 30 days)
* Unlimited activity meetup participation
* Priority profile visibility
* Exclusive access to premium nomad events

**Paywall Triggers:**
* After the 5th swipe in The Compass
* After the 3rd activity join attempt in Basecamp
* From the Profile tab "Upgrade to NomadPlus" button

#### 2. Builder Consultation Tokens (Transactional Revenue)

**Price:** $19.99 per consultation

**What's Included:**
* Priority one on one chat with a verified expert
* 30 minute dedicated consultation session
* 7 days of follow up message access

**Paywall Trigger:**
* When a user taps "Book Consultation" on any builder profile in The Garage

### Implementation Details

All subscription logic, paywall UI, and purchase flows are handled natively by the RevenueCat SDK. This ensures compliance with App Store guidelines, secure transaction processing, and robust receipt validation.

---

## Security and Safety

Safety is the foundation of NomadBound. The platform implements multiple layers of protection to create a trusted environment for all users, especially solo female travelers.

### Safety Features

**Invite Only System:** New users require a unique invite code, limiting access to verified community members.

**Video Selfie Verification:** Mandatory video verification ensures all profiles are authentic and connected to real individuals.

**Report and Block:** Every profile, message, and activity includes prominent "Report" and "Block" buttons for immediate action.

**Privacy Controls:** Users can hide exact locations, restrict who can message them, and control profile visibility.

**Community Guidelines Enforcement:** Zero tolerance policy for harassment, with clear consequences outlined in the Terms of Service.

---

## User Experience Highlights

### Onboarding Flow

1. Welcome screen with community values
2. Invite code entry or approval request
3. Video selfie verification
4. Profile creation (name, pronouns, van details)
5. Interest selection (climbing, hiking, photography, etc.)
6. Route planning (optional)
7. Premium upsell (optional)
8. Confirmation and entry to the community

### Visual Design

**Color Palette:**
* Deep Forest Green (primary actions)
* Burnt Orange (notifications and alerts)
* Slate Grey (backgrounds)
* Off White (primary text)

**Typography:** San Francisco (iOS system font) with bold headings for clarity and professionalism.

**Animations:** Smooth spring animations, haptic feedback, and micro interactions create a polished, premium experience.

---

## Installation and Setup

### Prerequisites

* macOS 13.0 or later
* Xcode 15.0 or later
* iOS 17.0+ device or simulator
* Active Apple Developer account
* RevenueCat account (for monetization setup)
* Firebase project (for backend services)

### Steps

1. Clone the repository:
```bash
git clone https://github.com/Haruna2004/NomadBound.git
cd NomadBound
```

2. Install dependencies:
```bash
pod install
```

3. Open the Xcode workspace:
```bash
open NomadBound.xcworkspace
```

4. Configure Firebase:
   * Download `GoogleService-Info.plist` from your Firebase console
   * Add the file to the Xcode project

5. Configure RevenueCat:
   * Add your RevenueCat API key to the configuration file
   * Set up subscription products in the RevenueCat dashboard

6. Build and run the project on your device or simulator.

---

## Team

NomadBound was designed and developed by a dedicated team of builders committed to solving real problems for the nomadic community.

* [**Haruna Faruk**](https://github.com/Haruna2004)
* [**Ohi Moiza**](https://github.com/Ohimoiza1205)
* [**Peace Enesi**](https://github.com/AhuoyizaEnesi)

---

## Hackathon Alignment

NomadBound was built specifically for the RevenueCat Shipyard Creator Contest and fully meets all submission requirements.

### Judging Criteria Alignment

**Audience Fit (30%):** Designed exclusively for Quin Gable's 1.2M+ van life audience. Directly addresses the challenges she outlined: nomadic dating, friend finding, and van builder access.

**User Experience (25%):** Premium iOS native design with intuitive navigation, seamless onboarding, and verified safety features.

**Monetization Potential (20%):** Dual revenue streams via RevenueCat (subscriptions and in app purchases) with clear, compelling paywalls.

**Innovation (15%):** Introduces route overlap matching, a first of its kind feature for nomadic communities, and creates a professional marketplace for van builders.

**Technical Quality (10%):** Built with SwiftUI, Firebase, and RevenueCat. Stable, performant, and production ready.

---

## Roadmap

### Phase 1 (Months 1 to 2)
* Launch Android version
* Implement push notifications for route overlap alerts
* Add user reported safety incident tracking

### Phase 2 (Months 3 to 4)
* Community marketplace for gear swaps and van sales
* Group trip planning feature
* Integration with popular campground booking platforms

### Phase 3 (Months 6+)
* International expansion (Europe, Australia, New Zealand)
* Partnerships with van rental companies
* Premium tier insurance partnerships

### Long Term Vision
* AI powered route recommendations based on user preferences
* Integration with van life content creators for exclusive events
* Blockchain based verified identity system for enhanced trust

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

Special thanks to:
* **Quin Gable** for providing the creator brief and inspiring this solution
* **RevenueCat** for hosting the Shipyard Creator Contest and providing the monetization infrastructure
* **The Van Life Community** for being the inspiration and audience for this platform

---

## Contact

For questions, feedback, or partnership inquiries, please reach out via:

* GitHub Issues: [NomadBound Issues](https://github.com/Haruna2004/NomadBound/issues)
* Email: nomadbound.app@gmail.com

---

**Built with care for the nomadic community. Safe travels.** 
