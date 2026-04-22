# CityGPT: Urban Odyssey

Build a city from nothing, then hold it together long enough to win the next election.

**CityGPT: Urban Odyssey** is a deterministic single-player browser city-builder where every month matters. Start with an empty map, place your first City Hall, zone your early neighborhoods, balance utilities and services, respond to public pressure, and steer your city through political campaigns, civic crises, and election seasons.

It is part strategy game, part political balancing act, and part evolving city story.

Play the game here: https://joelorange.github.io/joelorange/

---

## What kind of game is this?

CityGPT: Urban Odyssey is a turn-based city-builder played in monthly turns.

You do not place roads or micromanage individual citizens. Instead, you shape the city through:

- building placement
- district development
- policy decisions
- public services
- economic tradeoffs
- crisis management
- campaign strategy

Each turn, your choices ripple through the city. More housing can grow population, but it also raises service demand. Industry can create jobs and revenue, but it can also drive up pollution, public dissatisfaction, and political risk. Strong services and smart district planning can help you build a city that thrives instead of spirals.

---

## Core loop

1. Start a new city or resume a saved one.
2. Place **City Hall** on the empty map.
3. Build housing, utilities, jobs, and services.
4. Adjust policies using political capital.
5. End the month and resolve the simulation.
6. Read the city newspaper summary.
7. Respond to events, long-term pressures, and elections.
8. Keep growing without losing public support.

---

## What makes it interesting

### A city-builder with politics
You are not only optimizing a map. You are managing approval, voter groups, advisor trust, campaign boosts, manifesto promises, and recurring elections.

### Deterministic simulation
The game is seed-based and deterministic, which makes runs consistent, replayable, and good for experimentation.

### District identity matters
Each district can develop its own strengths through building mix, adjacency, tags, and specialization. Your city gradually develops recognizable neighborhoods instead of feeling like a flat spreadsheet.

### Events and pressure arcs
You will face major events, event chains, and longer civic pressure arcs that can reshape the direction of a run.

### Readable city feedback
Monthly newspapers, chronicle entries, citizen quotes, financial history, and the live HUD make it easier to understand what is happening and why.

---

## Current gameplay features

- Fixed **24 x 12** city map split into six districts
- Building placement, demolition, and City Hall relocation
- Utilities for **power** and **water**
- Service simulation for healthcare, education, police, fire, parks, culture, and transit
- Population growth based on housing, desirability, services, jobs, pollution, crime, and reputation
- Education and workforce matching that affects labor efficiency and revenue
- Policy sliders with political-capital costs and previewable effects
- District tags and specializations that shape local identity and performance
- Voter groups, advisor trust, manifesto commitments, and election cycles
- Queued events, event chains, and late-game civic pressure arcs
- Monthly newspaper summaries, chronicle history, and financial tracking
- Local save/load support in the browser
- Procedural sound effects and ambient music, muted by default

---

## How to play

### Early priorities
A stable opening usually means:

- place **City Hall** first
- secure **power** and **water**
- build **housing** so residents can move in
- add **jobs** so unemployment does not spike
- cover basic services before the city starts to drift into trouble

### Watch these closely

- **Money**: can you keep revenue ahead of upkeep and policy costs?
- **People**: are residents moving in, staying employed, and remaining satisfied?
- **Services**: are districts getting enough support?
- **Risk**: are pollution, crime, shortages, or crisis pressure starting to build?

### Longer-term goals

- develop specialized districts
- keep public approval healthy
- survive crisis spikes
- prepare for campaign season
- win the election

---

## Running the game locally

```bash
npm install
npm run dev
```

Then open the local Vite URL shown in your terminal.

Useful additional commands:

```bash
npm run build
npm run test
npm run lint
npm run validate:data
npm run test:e2e
```

---

## Save data

The game saves locally in your browser using `localStorage`.

That means:

- there is no backend account system
- saves stay on the browser/profile you used
- clearing browser storage can remove your save

---

## Current scope notes

This version is focused on the city simulation and political layer.

It currently does **not** include:

- multiplayer
- roads or traffic simulation
- pathfinding
- backend services
- individual citizen agent simulation

---

## Who this is for

You will probably enjoy CityGPT: Urban Odyssey if you like:

- city-builders with visible system interplay
- strategy games where tradeoffs matter
- political or civic management layers
- deterministic simulation you can learn and master over time
- watching a city develop a narrative identity through play

---

## Tips for first-time players

- Do not overbuild too early.
- Utility failures can shut down growth fast.
- Housing alone is not enough; residents also need jobs and services.
- Pollution and crime can quietly damage a run before they become obvious.
- Political capital is limited, so policy changes should be deliberate.
- A city that looks stable economically can still lose at the ballot box.

---

## Technical notes

Built with **React**, **TypeScript**, **Vite**, **Zustand**, and **Vitest**.

---

## Status

The current repository documentation describes this build as verified on **2026-04-22**, with passing production build, linting, validation, unit tests, and Playwright smoke coverage.

