# iOS Social App - Design Guidelines

## Brand Identity

**Purpose**: A social platform for iOS users (specific features TBD - template should support feeds, profiles, and interactions).

**Aesthetic Direction**: Clean and approachable - prioritizing content over decoration. Think Instagram's clarity with softer, more welcoming tones. The app should feel modern but not cold, with enough breathing room to let social content shine.

**Memorable Element**: Generous whitespace and soft shadows that create depth without clutter. The interface should fade into the background, letting user content take center stage.

## Navigation Architecture

**Root Navigation**: Tab Bar (3 tabs)
- **Home Tab**: Social feed/content discovery
- **Create Tab**: Core action for posting/sharing (center position)
- **Profile Tab**: User settings and account

**Stack Structure**:
- Home Stack: Home screen → Detail views (future)
- Create Stack: Creation flow (modal for now)
- Profile Stack: Profile screen → Settings

All screens use native modals for temporary actions (e.g., filters, help).

## Screen-by-Screen Specifications

### 1. Home Screen
**Purpose**: Primary content area (placeholder for future social feed)

**Layout**:
- Header: Transparent, app name centered, no buttons
- Main Content: ScrollView with welcome message placeholder
- Safe Area: Top inset = headerHeight + Spacing.xl, Bottom inset = tabBarHeight + Spacing.xl

**Components**: Text container centered vertically with app name and subtitle

---

### 2. Create Screen
**Purpose**: Core action placeholder (future: post creation, media upload)

**Layout**:
- Header: Default navigation, title "Create", left: Cancel
- Main Content: ScrollView with centered placeholder text
- Safe Area: Top inset = Spacing.xl, Bottom inset = tabBarHeight + Spacing.xl

**Components**: Centered text indicating future functionality

---

### 3. Profile Screen
**Purpose**: User account and settings

**Layout**:
- Header: Transparent, title "Profile"
- Main Content: ScrollView
  - Avatar placeholder (circular, 80pt diameter)
  - Display name field
  - Email display (if auth implemented)
  - Settings button
- Safe Area: Top inset = headerHeight + Spacing.xl, Bottom inset = tabBarHeight + Spacing.xl

**Components**: Avatar, text fields, touchable settings row

**Authentication**: Include Apple Sign-In (required for iOS apps with accounts). Mock flow for prototype - use local state. Profile must have "Sign Out" button (with confirmation alert).

---

## Color Palette

**Primary**: #5B7FFF (soft blue - approachable, trustworthy)
**Secondary**: #8B9DFF (lighter blue for accents)
**Background**: #FFFFFF
**Surface**: #F8F9FA (off-white for cards/containers)
**Border**: #E8EAED
**Text Primary**: #1A1D1F
**Text Secondary**: #6C757D
**Error**: #FF5757
**Success**: #34C759

## Typography

**Font**: System default (SF Pro for iOS)

**Type Scale**:
- Display: 32pt, Bold (screen titles)
- Title: 20pt, Semibold (section headers)
- Body: 16pt, Regular (main content)
- Caption: 14pt, Regular (secondary text)
- Small: 12pt, Regular (metadata, timestamps)

## Visual Design

- Icons: Use SF Symbols for iOS (@expo/vector-icons/Ionicons as fallback)
- Touchable Feedback: Opacity 0.6 on press
- Border Radius: 12pt for cards, 8pt for buttons, 40pt for circular avatars
- Spacing Scale: xs=4, sm=8, md=12, lg=16, xl=24, xxl=32
- Tab Bar: Height 80pt, icons 24pt, labels 11pt

**Shadows** (floating elements only):
- shadowOffset: {width: 0, height: 2}
- shadowOpacity: 0.10
- shadowRadius: 2

## Assets to Generate

1. **icon.png**
   - Description: App icon with soft geometric shape on gradient background (blue tones)
   - WHERE USED: Device home screen

2. **splash-icon.png**
   - Description: Simplified version of app icon for launch screen
   - WHERE USED: App startup/splash screen

3. **avatar-placeholder.png**
   - Description: Neutral circular avatar with abstract person silhouette in #E8EAED
   - WHERE USED: Profile screen default avatar

4. **empty-home.png**
   - Description: Soft illustration of empty social feed (abstract shapes suggesting content cards)
   - WHERE USED: Home screen before content loads

All assets should use the app's color palette (#5B7FFF primary) with soft, friendly styling.