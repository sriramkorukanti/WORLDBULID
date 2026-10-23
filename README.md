
# WORLDBUILD

### Build a world. Shape its nature. Watch civilizations rise.

WORLDBUILD is an ambitious procedural worldbuilding and simulation project focused on creating fictional worlds and exploring how geography, climate, natural resources, settlements, and civilizations interact over time.

The goal is to build more than a map generator. WORLDBUILD aims to become an interactive sandbox where every world begins with a seed and gradually develops its own geography, ecosystems, societies, and history.

> **Project status:** Active development  
> **Current focus:** Procedural world generation, natural systems, and civilization simulation

---

## Overview

Every world has a story, but that story begins long before its first civilization.

Mountains influence settlement locations. Rivers provide access to water. Climate shapes ecosystems. Resources influence economic development. Settlements grow, civilizations expand, and the conditions of the world influence what happens next.

WORLDBUILD explores these relationships through a modular simulation engine and an interactive world map.

The long-term vision is to let users generate a world, inspect its underlying systems, influence its development, and observe the history that emerges.

## Vision

- **Generate** unique, reproducible fictional worlds.
- **Explore** terrain, elevation, climate, biomes, and hydrology.
- **Populate** worlds with settlements and civilizations.
- **Simulate** populations, resources, economies, and trade.
- **Observe** historical events and the rise and fall of societies.
- **Customize** worlds and experiment with different initial conditions.
- **Preserve** generated worlds and revisit their development.

The objective is not to script every event. It is to create systems that interact in meaningful ways.

---

## Planned features

### 1. Procedural world generation

Generate fictional worlds using configurable parameters and deterministic seeds.

- Seed-based world generation
- Interactive map navigation
- Elevation and terrain classification
- Tile selection and inspection
- Reproducible world generation
- Local world saving and loading

### 2. Natural systems

Give each world a coherent physical environment.

- Temperature and rainfall simulation
- Biome generation
- Mountains, plains, forests, deserts, and coastlines
- Rivers, lakes, and drainage systems
- Natural resource distribution
- Environmental suitability for settlements

### 3. Civilizations and settlements

Populate worlds with societies that respond to their surroundings.

- Villages, towns, cities, and ports
- Procedurally generated civilization names
- Population dynamics
- Cultural identities
- Territorial influence
- Settlement development

### 4. Economy and trade

Model the resources that allow settlements to survive and develop.

- Food production and consumption
- Resource inventories
- Wood, stone, ore, and other resources
- Resource shortages and surpluses
- Trade route generation
- Inter-settlement resource exchange
- Economic effects on population and development

### 5. Historical simulation

The long-term plan is to turn simulation outcomes into a coherent world history.

- Chronological event logs
- Civilization expansion and decline
- Migration and settlement founding
- Diplomacy and political relationships
- Conflicts and territorial changes
- Historical timelines
- Persistent world states

*These are development goals, not a claim that every feature is already implemented.*

---

## Development roadmap

WORLDBUILD is being developed incrementally, with each phase building on the systems established by earlier phases.

| Phase | Focus | Goal |
|---|---|---|
| 1 | World foundation | Seeded generation, interactive map, tile inspection, local persistence |
| 2 | Natural systems | Terrain, climate, biomes, hydrology, and resources |
| 3 | Civilization engine | Settlements, populations, economies, and trade |
| 4 | History and politics | Timelines, diplomacy, conflicts, and historical events |
| 5 | Advanced simulation | Deeper interactions, customization, and balancing |
| 6 | Release and polish | Performance, usability, documentation, and distribution |

The roadmap describes the intended direction. Features should be considered complete only when implemented and tested in the repository.

---

## Design principles

### Deterministic simulation

A world generated with the same seed and settings should be reproducible. This makes experimentation, debugging, and sharing worlds more reliable.

### Modular architecture

World generation, natural systems, civilization simulation, and rendering should remain separate concerns. Each system should be testable and extendable without requiring a rewrite of the entire application.

### Geography matters

Settlements, resources, and trade should respond to actual world data instead of being placed arbitrarily.

### Systems over scripted outcomes

The aim is to model understandable rules and let their interactions produce interesting outcomes.

### Transparency

World data and simulation rules should be inspectable. When a settlement grows or declines, the simulation should provide meaningful reasons.

### Incremental development

Each phase should preserve existing functionality, include automated tests, and be verified before the next layer is added.

---

## Technology

The final technology stack should reflect the actual implementation in the repository.

The current architectural direction includes:

- **Language:** TypeScript
- **Frontend:** React
- **Build tooling:** Vite
- **Rendering:** Canvas-based interactive map
- **Persistence:** Browser-based local storage, such as IndexedDB
- **Testing:** Automated unit and integration tests

Additional technologies, including Web Workers or a backend database, may be introduced if the scale of the simulation justifies them.

*Update this section to match the dependencies and implementation currently present in the repository.*

---

## Getting started

### Prerequisites

- Node.js, using a version supported by the project
- npm or the package manager specified by the repository

### Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/WORLDBUILD.git
cd WORLDBUILD
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Open the local URL printed by the development server.

### Testing

Run the test command configured by the project:

```bash
npm test
```

The exact scripts may differ as development progresses. Check `package.json` for the commands actually supported by the current repository.

---

## Project structure

The project is intended to keep simulation logic separate from the user interface.

A possible organization is:

```text
src/
├── app/            # Application shell and page composition
├── components/     # Reusable interface components
├── world/          # World data models and generation
├── simulation/     # Natural and civilization systems
├── rendering/      # Map rendering and visual layers
├── persistence/    # Save, load, and schema migration
├── utils/          # Shared utilities
└── tests/          # Automated tests
```

This is an illustrative structure, not a guarantee of the repository's current layout.

---

## Contributing

Contributions, suggestions, bug reports, and technical discussions are welcome.

Before submitting a change:

1. Check existing issues and planned work.
2. Keep changes focused and consistent with the current architecture.
3. Avoid breaking existing world saves or simulation behavior.
4. Add tests for new simulation rules.
5. Run the relevant tests and checks.
6. Document new configuration options and known limitations.

For substantial changes, open an issue first to discuss the proposed approach.

---

## Current limitations

WORLDBUILD is an evolving project. Its simulation models are intended to balance interesting behavior, technical clarity, and performance.

Early models may simplify real-world climate, ecology, demographics, economics, and historical processes. Outputs should not be interpreted as scientifically accurate predictions.

Advanced systems such as diplomacy, warfare, migration, and long-term historical simulation depend on the completion of earlier foundational systems.

---

## The idea

A map is only the beginning.

The real question is what happens when geography, resources, populations, and time begin interacting.

**WORLDBUILD is an attempt to make that question explorable.**

