# TravelPlanner
# Wayline — travel planning app

A prototype travel planning app that lets a traveler build a day-by-day itinerary and track a trip budget in one place, styled around a travel-journal / boarding-pass look instead of a generic dashboard.

[Add your demo video link here]
[Add your live prototype / deployed link here]

---

## Table of contents

- [Problem statement](#problem-statement)
- [Target users](#target-users)
- [Ideation](#ideation)
- [Design](#design)
- [Features](#features)
- [Tech stack](#tech-stack)
- [Project structure](#project-structure)
- [Getting started](#getting-started)
- [Team](#team)
- [Roadmap](#roadmap)

---

## Problem statement

Planning a multi-day trip usually means juggling several disconnected tools — a notes app for the itinerary, a spreadsheet for the budget, a maps app for locations, and a messaging thread for sharing plans with travel companions. This fragmentation makes it easy to lose track of what's booked, what's still open, and how much the trip actually costs.

Wayline addresses this by combining itinerary planning and budget tracking into a single, lightweight interface, so a traveler can see their whole trip — day by day, dollar by dollar — in one place.

## Target users

- [Add your target user description here, e.g. independent travelers planning multi-city trips]
- [Add secondary persona if relevant, e.g. group trip organizers]

## Ideation

- [Add link to ideation board, e.g. Miro / FigJam / Jamboard]
- [Add link to brainstorming notes or mind map]
- [Add link to competitor analysis, if any]

## Design

- [Add link to Figma / wireframes]
- [Add link to user flow diagrams]

**Design language used in the prototype:**

| Element | Choice |
|---|---|
| Concept | Travel journal / boarding pass, rather than a generic SaaS dashboard |
| Primary colors | Ink navy `#12232E`, cloud cream `#F7F3E8`, runway gold `#D9A544` |
| Secondary accent | Harbor teal `#2E6E6E` |
| Typography | Fraunces (headings), Inter (body and UI) |
| Layout | Day-by-day "ticket stub" cards with a perforated divider; dashed dividers in place of drop shadows |

## Features

- **Trip header** — editable trip name and date range, with an at-a-glance day count
- **Destination chips** — add or remove destinations for the trip
- **Day-by-day itinerary** — add, label, and remove days; each day is a card of timed activities
- **Activities** — add a time, description, and cost per activity; remove any activity
- **Budget ledger** — add custom budget line items with a live running total

## Tech stack

| Layer | Technology |
|---|---|
| Frontend | HTML5, CSS3, vanilla JavaScript |
| Fonts | Google Fonts (Fraunces, Inter) |
| Data | In-memory state (prototype only — no backend or persistence yet) |
| Hosting | [Add hosting platform once deployed, e.g. GitHub Pages / Vercel] |

> This version is a frontend prototype used to validate the interaction design. It does not yet include a backend, database, or authentication.

## Project structure

```
.
├── index.html          # Prototype markup, styles, and logic
├── README.md
└── [add other files/folders as the project grows]
```

## Getting started

1. Clone the repository:
   ```
   git clone [add your repo URL here]
   ```
2. Open `index.html` directly in a browser, or serve it locally:
   ```
   npx serve .
   ```
3. No build step or dependencies are required for the current prototype.

## Team

| Name | Role | Contribution |
|---|---|---|
| [Add name] | [Add role] | [Add contribution] |
| [Add name] | [Add role] | [Add contribution] |

## Roadmap

- [ ] Connect activity costs to the budget ledger automatically
- [ ] Add a map view alongside the itinerary
- [ ] Add persistence (backend + database)
- [ ] Add multi-user trip sharing
- [ ] Add authentication
