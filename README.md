# PG Quartermaster

A companion tool for [Project Gorgon](https://projectgorgon.com) that helps players plan efficient routes for completing work orders, delivery quests, and tracking missing recipes.

**Live version:** [shamorshinf.github.io/PGQuartermaster](https://shamorshinf.github.io/PGQuartermaster/)

## Features

### Work Orders
- Browse and filter all available work orders by industry level, craft status, contract ownership, and more
- **Route Planner** — generates an optimized multi-stop route for completing selected work orders, grouping pickups, crafting steps, vendor purchases, and turn-ins by zone
- Shopping list generator with ingredient breakdowns and storage shortfall detection
- Craft chain resolution — automatically plans sub-crafts for complex recipes

### Quests
- View and filter delivery quests (active, available, or all)
- **Quest Route Planner** — plan efficient routes for completing delivery quests
- Search, sort, and hide completed quests

### Missing Recipes
- Shows recipes you haven't learned yet, filterable by crafting skill
- Displays trainer NPCs, locations, and favor level requirements
- Links to the Project Gorgon wiki for each recipe

### Imports
- **Inventory JSON** — import your full inventory from the in-game report
- **Character JSON** — import skills, active work orders, and quest progress
- **Game Data** — automatically fetched from the Project Gorgon CDN (items, recipes, quests, NPCs)
- Drag-and-drop file import with visual status indicators

## Getting Started

1. Open the app in your browser (either the [live version](https://shamorshinf.github.io/PGQuartermaster/) or the HTML file locally)
2. Go to the **Imports** tab
3. Export your data from Project Gorgon:
   - In-game, use `/reportinventory` and `/reportcharacter` to generate JSON files
   - These are saved to `%LocalAppData%Low\Elder Game\Project Gorgon\Reports\`
4. Drag and drop the JSON files onto the import drop zones (or click to browse)
5. Game data (items, recipes, NPCs) is fetched automatically from the CDN on first load

## Tech Stack

- Single self-contained HTML file — no build step, no frameworks, no server required
- Vanilla HTML, CSS, and JavaScript
- IndexedDB for local data persistence
- Project Gorgon CDN for game data

## Bug Reports

Click the **Bug Report** button (bottom-right corner) to auto-generate a debug report and open a pre-filled GitHub issue.

## Credits

- **Game**: [Project Gorgon](https://projectgorgon.com) by Elder Game, LLC
- Some portions copyright 2026 Elder Game, LLC
