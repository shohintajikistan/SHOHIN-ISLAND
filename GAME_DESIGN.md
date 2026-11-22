# SHOHIN ISLAND — Game Design & Production Plan

## Locked creative direction

- Genre: open-world island life simulation + exploration + adventure + survival + construction.
- Camera: switchable first-person and third-person.
- Visual target: high-end, realistic AAA-inspired presentation, with scalable settings for Android.
- World target: 143,100 km² of designed land and surrounding marine territory.
- Current prototype: a procedural Three.js island scene. The currently rendered terrain is a small development showcase, not the complete 143,100 km² world.

## Core player promise

A player can choose their own life on a vast island: explore wilderness, discover secrets, build a home, develop a business, travel between settlements, survive expeditions, meet wildlife, and eventually play with other people.

## World regions

The world is planned as twelve distinct macro-regions. Names are working names and may change during production.

1. SHOHIN CITY — main city, residential districts, services, transport hub.
2. GREEN JUNGLE — dense rainforest, wildlife, trails, hidden ruins.
3. BLUE COAST — beaches, lagoons, resorts, harbors and reefs.
4. DRAGON MOUNTAINS — high peaks, cliffs, mountain roads and alpine weather.
5. WATERFALL VALLEY — rivers, cascades, pools and cave systems.
6. VOLCANO LAND — volcanic terrain, geothermal areas and hazard missions.
7. LOST WORLD — ancient structures, archaeology and story mysteries.
8. WILD NORTH — remote wilderness and rare animal habitats.
9. GOLDEN DESERT — dry interior, canyons and isolated settlements.
10. CRYSTAL LAKES — highland lakes, forests and scenic exploration.
11. SOUTHERN ISLANDS — smaller islands, boat travel and coastal villages.
12. BLUE OCEAN — open sea, diving, shipwrecks and marine life.

## Essential gameplay systems

### Exploration
- Discoverable map, landmarks, viewpoints, trails and hidden locations.
- Fog-of-war or unexplored map areas.
- Collectibles, journals, clues, treasure maps and environmental storytelling.
- Fast travel only where it fits the world design.

### Life and settlement
- Player home, interior spaces and furnishing.
- NPCs with daily routines, schedules and reactions.
- Shops, food venues, clinics, police, schools, hotels and garages.
- Jobs, services and legal businesses as optional progression paths.

### Building and economy
- Placeable building pieces and modular structures.
- Farms, gardens, fishing, crafting and resource gathering.
- Player-owned shops, guest houses, restaurants and transport services.
- Prices, inventory, supply and demand kept understandable and balanced.

### Survival and wildlife
- Health, stamina, hunger, thirst and weather exposure where appropriate.
- Wildlife habitats, feeding, fleeing, territorial behavior and predator/prey interactions.
- Gathering, shelter, tools and expedition preparation.
- Survival should be optional or adjustable so the game remains welcoming to life-simulation players.

### Vehicles
- Cars, off-road vehicles, motorcycles, bicycles, boats, yachts, helicopters and aircraft.
- Distinct handling, acceleration, braking, traction and damage.
- Fuel and repairs can be optional settings.
- Vehicles must be introduced only after stable character movement and world scale are established.

### Missions and narrative
- Exploration, rescue, ecology, delivery, racing, business, archaeology and survival missions.
- Main story supported by optional side stories.
- Environmental clues and multi-step mysteries.
- No requirement to complete every activity to enjoy the world.

### Social and multiplayer (later phase)
- Friends, shared expeditions, cooperative building and trading.
- Player-owned spaces and events.
- Server authority, moderation, privacy and anti-cheat must be designed before public multiplayer.
- Multiplayer is not part of the current offline prototype.

## Visual and audio quality targets

- Physically based materials for terrain, rock, foliage, wood, metal and water.
- Layered terrain materials: sand, grass, forest floor, rock and snow.
- Natural coastline transitions, beaches, cliffs and shallow-water color variation.
- High-quality tree silhouettes, varied foliage, ground cover and rocks.
- Dynamic sky, sun position, time of day, fog, rain and storms.
- Ambient wildlife, wind, insects, water, footsteps and location-specific sound.
- Cinematic lighting and post-processing only when performance permits.

## Technical production requirements

- Three.js WebGL renderer for the browser prototype.
- World partitioning into streamed regions/chunks; never load the whole island at once.
- Level of Detail (LOD), frustum culling, instanced vegetation and asset batching.
- Texture atlases and compressed textures where supported.
- Adaptive render resolution and selectable Low / Medium / High / Ultra profiles.
- Mobile touch controls, camera sensitivity settings and optional keyboard/gamepad support.
- Save system for settings, player position and progression.
- Stable asset pipeline with optimized GLB/glTF models.
- Procedural generation must use deterministic seeds so the same world can be recreated.
- Use real measured scale and a world-coordinate system; avoid pretending the current 5 km prototype is the complete world.

## Development milestones

### Milestone 1 — playable vertical slice
- Reliable loading and error handling.
- Island terrain, shoreline, sea, hills and forest.
- Character movement and jump.
- Correct first-person / third-person camera switching.
- Mobile joystick and camera drag.
- Initial landmarks: beach, waterfall, river and lookout.
- Performance profiling on a real Android phone.

### Milestone 2 — believable environment
- Replace placeholder tree shapes with optimized quality assets.
- Better water, shore transitions, rocks, ground cover and terrain materials.
- Day/night cycle, moving clouds, wind and ambient audio.
- Wildlife prototype with a small number of species.
- Basic map, compass and discovery markers.

### Milestone 3 — meaningful gameplay
- Interactions, inventory, gathering and crafting.
- One village with NPC routines and usable buildings.
- Basic quests, treasure clues and save/load.
- A first vehicle prototype.

### Milestone 4 — expand the island
- Region streaming and deterministic world generation.
- Multiple biomes, settlements, caves, beaches and mountain areas.
- Expand playable territory gradually while profiling memory and frame rate.

### Milestone 5 — life simulation and online features
- Housing, farming, jobs, business and economy.
- More advanced NPC and wildlife systems.
- Multiplayer architecture only after the single-player game is stable.

## Quality gates

A milestone is not complete because it looks attractive in a screenshot. It must:
1. Load without console/runtime errors.
2. Work with touch controls on Android.
3. Maintain acceptable frame rate on target devices.
4. Have tested collisions and interaction boundaries where applicable.
5. Save and restore required player state.
6. Be clearly labeled as prototype, beta or production-ready.

## Honest scope statement

A 143,100 km² world with AAA-level assets is a major game-production effort. A single HTML file and procedural primitives cannot deliver that quality by themselves. The project will build a working vertical slice first, then add optimized art assets and streamed regions in stages. The current Three.js scene is a foundation for that process, not a finished AAA game.
