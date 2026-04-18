# Hard Pass — Build Guide (V1)

## Overview

Hard Pass is a one-screen mobile app that helps users say no.

The app generates a short response that the user can copy or share.

This is intentionally simple. The goal is to ship a working V1 quickly.

---

## Core Flow

1. User opens app  
2. User taps button  
3. App displays a response  
4. User can copy or share the response  

No other flows are required.

---

## UI Layout

Single screen only.

### Elements:

- Title: "Hard Pass"
- Main text area (center of screen)
  - Displays the current response
  - Large, readable text

- Primary button:
  - Label: "Give Me an Excuse"

- Secondary actions (below response):
  - Copy button
  - Share button

- Optional (if easy):
  - Category selector (Polite / Funny / Firm)

---

## Behavior

- On button press:
  - Select a random response
  - Display it immediately

- Default behavior:
  - Pull from all categories

- If category is selected:
  - Only use responses from that category

- Each new press:
  - Replaces the previous response

---

## Data Source

Responses are stored locally in the app.

Use the file:
`/docs/excuses.md`

Categories:
- Polite
- Funny
- Firm

---

## Technical Notes

- No backend required
- No accounts or authentication
- No data persistence required
- No API calls required
- Local-only logic is fine

---

## Out of Scope (V1)

Do NOT implement:

- User accounts
- Saving favorites
- Editing responses
- AI-generated content
- Settings menus
- Notifications

---

## Definition of Done

The app is complete when:

- Button generates a random response
- Response displays clearly
- Copy button works
- Share functionality works

---

## Priority

Speed over perfection.

We want a working version, not a perfect version.

---

## Notes

If something is unclear, default to the simplest possible implementation.
