# TravelPlanner
# TrailCraft — travel planning website by MiloEgg

A prototype travel planning website that lets a traveler build a day-by-day itinerary and track a trip budget in one place, styled around a travel-journal / boarding-pass look instead of a generic dashboard.

[Add your demo video link here]
[Add your live prototype / deployed link here]

---

## Table of contents

- [Problem statement](#problem-statement)
- [Target users](#target-users)
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

TrailCraft addresses this by combining itinerary planning and budget tracking into a single, lightweight interface, so a traveler can see their whole trip — day by day, dollar by dollar — in one place.

## Target users

- The independent trip planner — solo travelers, couples, or small friend groups planning a multi-day trip who want one place to see the itinerary and budget together, instead of splitting the work across a notes app, spreadsheet, and group chat.
- The budget-conscious traveler — students and first-time international travelers for whom cost is a real constraint, who want a running total against what they've planned so they can catch overspending before the trip, not after.
- The group trip organizer — someone coordinating a trip for multiple people who needs a clear, shareable day-by-day plan rather than details scattered across a chat thread.


## Design

- https://www.figma.com/design/CBwI86aEKxSqrzdAVMJ61u/TrailCraft?node-id=0-1&t=ff7z4Wi3rEicG6ny-1

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

API endpoints
Method	Route	Description
GET / PUT	/api/trip	Get or update trip name and dates
GET / POST	/api/destinations	List or add destinations
DELETE	/api/destinations/:index	Remove a destination
GET / POST	/api/days	List or add itinerary days
PUT / DELETE	/api/days/:dayId	Rename or remove a day
POST	/api/days/:dayId/activities	Add an activity to a day
PUT / DELETE	/api/days/:dayId/activities/:activityId	Update or remove an activity
GET / POST	/api/budget	List or add a budget line
PUT / DELETE	/api/budget/:lineId	Update or remove a budget line
GET	/api/budget/total	Get the running budget total
GET	/api/health	Health check

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

| Name    | Role | Contribution |
|---|---|---|
| KHOO CHEE YOUNG | [Team Leader] | [Planning,Assigning] |
| TAN HAO KIT     | [Team Member] | [Documentation] |
| RONAN CHAN      | [Team Member] | [Video] |
| NEO JIA LER     | [Team Member] | [Documentation] |


## Roadmap

- [ ] Connect activity costs to the budget ledger automatically
- [ ] Add a map view alongside the itinerary
- [ ] Add persistence (backend + database)
- [ ] Add multi-user trip sharing
- [ ] Add authentication
