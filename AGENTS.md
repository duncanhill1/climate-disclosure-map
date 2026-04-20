# AGENTS.md

## Project name
Climate Disclosure Map

## Goal
Build a polished web app mockup that educates users about climate disclosure requirements around the world.

## Core experience
- A full-width world map is the main feature of the homepage.
- Jurisdictions with climate disclosure requirements are shown in blue.
- Jurisdictions without disclosure data shown are grey.
- When a user hovers over a highlighted jurisdiction, a popup/tooltip appears.
- The popup should show:
  - jurisdiction name
  - disclosure title
  - short summary
  - link to the official government source
- The app must support both:
  - countries
  - subnational jurisdictions such as California

## Tech stack
- Next.js
- TypeScript
- Tailwind CSS
- react-simple-maps

## Design style
- Clean
- Modern
- Professional
- Minimal
- Strong emphasis on readability
- The world map should dominate the page visually
- Smooth but restrained interactions
- Avoid overdesign

## Functional requirements
- Responsive layout
- Reusable components
- Disclosure data stored separately from components
- Easy to replace placeholder data with real data later
- Hover tooltip on desktop
- Structure should allow later expansion to click interactions or side panels

## Data model
Each disclosure record should support:
- id
- type ("country" or "state")
- name
- parentCountry (optional)
- isoCode
- disclosureTitle
- summary
- officialUrl
- status
- coordinates (optional, for markers/callouts)

## Build guidance
- Use reusable React components
- Keep map logic separated from page layout
- Keep disclosure data in `/data`
- Add clear TypeScript types
- Add a legend to explain blue vs grey
- Include California as a subnational example
- Use placeholder data until the full jurisdiction list is provided

## Avoid
- Hard-coding all disclosure text in JSX
- Overly flashy animations
- Cluttered layout
- Backend setup for now
