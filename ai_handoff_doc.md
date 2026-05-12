# Star Citizen Fast Travel — AI Handoff Document for CIG Design Team

## Purpose

This document is a structured brief that can be fed directly into any AI tool (Claude, ChatGPT, Copilot, Gemini, or internal tooling) to generate implementation plans, technical specifications, or design evaluations for Star Citizen's fast travel system. It contains the complete context an AI needs to work productively on this problem.

---

## Prompt for CIG's AI Tool

Copy everything below this line into your AI tool of choice:

---

### CONTEXT

You are assisting CIG's design team in evaluating and implementing a fast travel / grouping system for Star Citizen. The system must solve the problem of players taking 10-30 minutes to group up while respecting the game's core design pillars.

### GAME DESIGN PILLARS (NON-NEGOTIABLE)

1. **Physicalization:** Every player, NPC, bullet, weapon, armor piece, ship, and ship component is a real physical object in the game world obeying physics. Players must exist as physical bodies at all times. No popping in/out of existence.

2. **Persistence:** "If you drop a coke can on a planet in a random spot, if you come back a week later the coke can will still be there." Objects, bodies, and world state do not vanish for convenience. The game uses a physicalized destruction engine called Maelstrom — ships break apart realistically, soil erodes, rain falls, wreckage persists.

3. **No Loading Screens:** The game is marketed as having no loading screens. Any solution that introduces a loading screen or fade-to-black transition violates this pillar.

4. **Death of a Spaceman (DOAS):** Death has consequence. Players clone via DNA imprinting at medbeds, but each death costs a clone life (finite), triggers death taxes, asset transfer fees, reputation loss, and skill degradation. Death is a fail state, not a mechanic to exploit.

5. **Item Integrity / No Duplication:** All weapons, armor, and equipment are either crafted (high quality) or purchased from NPC shops (lower quality). Items are physical objects with real scarcity. Any system that could result in an item existing in two places simultaneously is unacceptable. Item duplication must be structurally impossible, not just prohibited by rules.

6. **One System Principle:** The solution should be a single unified mechanic that covers multiple use cases, not separate systems for each scenario. This minimizes engineering burden and maintenance.

### ESTABLISHED IN-UNIVERSE TECHNOLOGY

- FTL communication exists (Dr. Betel's breakthrough, December 2025 lore). Information can travel faster than light. FTL matter transport does NOT exist.
- DNA imprinting and cloning at medbeds is established technology.
- Medbeds use medgel as a consumable resource to limit respawns.
- Bed log-in/log-out functionality exists (players can lie in a bed, log out, and log back in at that bed).
- NPC bodies exist in-game (enemy AI crews on ships, FPS NPCs, ambient NPCs at stations).
- NPC crew for player ships has been delayed past 1.0 (estimated 2027+).
- Ship components are modular and installable.
- Crew quarters exist on ships with beds, suit lockers, and armor racks — currently almost entirely non-functional.

### USE CASES THE SYSTEM MUST SOLVE

1. **Ship Crewing:** A player wants to join a friend's multicrew ship that's already in space or docked. Currently takes 10-30 minutes of travel.
2. **Open World Grouping:** Players scattered across a star system want to meet up for activities. Currently takes 10-30 minutes.
3. **Instanced Content:** Players need to group up at instanced mission entrances (e.g., Municipal Works, Siege of Orison). Currently requires everyone to travel there independently.

### COMMUNITY DATA

Community Pareto analysis of time lost when grouping up:
- Loading ship with vehicles/boxes: 30 minutes
- Server switching: 15 minutes
- ASOP ship location unknown: 10 minutes
- Jump point broken: 10 minutes
- Inventory doesn't load: 8 minutes
- Can't set QT route: 8 minutes
- Ship spawns upside down: 7 minutes
- Fall through floor: 6 minutes
- Can't see party marker: 6 minutes
- Hangar doors won't open: 5 minutes
- Party invite issues: 5 minutes
- **Actual travel time: 5 minutes (~4% of total)**

### COMMUNITY IDEAS EVALUATED (11 PROPOSALS, RANKED)

Each scored 1-5 across: Physicalization, Persistence, Lore Compatibility, Effectiveness, Exploitability Resistance, Feasibility, Versatility. Max score 35.

1. **C.I.V. / I.R.C. (31/35):** Cybernetic drone bodies stored as cargo, controlled via consciousness transfer. Relay Core ship component. No NPC AI needed. Range-limited. Strong anti-exploit (destroying IRC kills all CIVs). Weakness: cybernetic bodies may clash with SC's organic aesthetic.

2. **Agent Smithing (30/35):** Take over an existing NPC crew member's body. Consciousness moves, original body stays behind. No gear transfers. Crew hire tokens as consumable limiters. Weakness: requires NPC crew tech (delayed past 1.0). Strongest versatility — covers all three use cases.

3. **Commercial Flights / Genesis Starliner (28/35):** Board a real physicalized commercial ship at a spaceport, ride it to destination. Scheduled departures, accelerated QT. Perfect physicalization and lore. Weakness: relocation only, not grouping. Doesn't get you onto a friend's ship.

4. **Bed Log Transit (28/35):** Log out at transit hub, server-side real-world countdown starts (travel time = ~0.75x manual QT time, 30-minute minimum). Body is physically aboard a transport. Log in after timer completes: spawn at destination. Log in early: wait or cancel and wake up at departure hub. Virtually unexploitable. Weakness: pre-planned only, useless for spontaneous grouping.

5. **Transfer Transit / Temporary Clone (27/35):** Consciousness into a temporary clone with a degradation timer. Memory loss if clone dies before syncing. Weakness: materializing a body from nothing is hard to justify in a physicalized universe.

6. **Crew Quarters Registry (27/35):** Pre-register to a bed on a ship. Captain issues "call to arms," crew wakes up aboard in underwear. Highest feasibility — every component exists today. Weakness: body teleports (physicalization: 3/5).

7. **Rare Alien Structures (25/35):** Ancient alien bridges at edges of space. Perfect physicalization but barely solves grouping — endgame exploration only.

8. **Formalized Medbed Clone-In (25/35):** Deliberately clone to a party member's medbed. Everything exists already. Weakness: conflicts with DOAS — each use costs a clone life once death penalties are live.

9. **Remote Medical Imprint Transfer (28/35):** Expand existing medbed functionality — remotely transfer medical imprint via FTL comms to a party member's medbed or hangar medbed. Gear auto-stores at departure location (no duplication). Spawn on ship = gear from armory. Spawn in hangar = access own stored ships/equipment. Framed as "consciousness relocation" not death. Simplest implementation of any high-scoring idea. Weakness: DOAS cost tension remains — if no clone-life cost, needs another anti-abuse gate.

10. **Group Launch (24/35):** Spawn at party leader's station when logging in after 1+ hour offline. Pay QT fuel. UEE only. Session-start only.

10. **Paid NPC Transport / Fade-to-Black (23/35):** Pay fare, screen fades, arrive at destination. Good concept but body doesn't exist during transit.

11. **Teleport to Docked Ship (22/35):** Raw teleportation with a "docked only" condition. Effective but violates physicalization and persistence.

### SYNTHESIZED HYBRID SOLUTION: IMPRINT SHELL NETWORK (33/35)

**Two-layer system:**

**Layer 1 — Long Haul:** Physicalized Commercial Flights (ride a real Starliner) + Bed Log Transit (log out at transit hub, real-world countdown at 0.75x manual QT speed with 30-min minimum, body physically aboard transport, log in after timer to spawn at destination or cancel to return to departure point). Handles cross-system relocation.

**Layer 2 — Last Mile:** Imprint Shells. Key specs:
- Organic clone bodies grown at medical facilities, sold at ports as physical consumables
- Must be physically transported to a ship and placed in crew quarter beds
- Ship requires a Relay Beacon component (tiered capacity, range-limited)
- Player transfers consciousness from an Imprint Terminal at any port via FTL comms
- Player's real body enters stasis at the terminal — physical, persistent, vulnerable
- Player wakes up in Shell wearing medical gown — NO gear transfers in either direction
- Player gears up from ship's armory (owner must pre-stock)
- Shell has biological degradation timer (4-8 hours)
- On departure or timer expiry: consciousness returns to real body, Shell dies and leaves a corpse with gear
- Combat lockout: cannot transfer into a Shell on a ship in active combat
- Cooldown: 30-60 minutes between transfers
- Instanced content variant: Contractor Shells at mission entrances, cannot interact with loot, despawn on mission complete

**Anti-duplication guarantee:** Consciousness crosses the transfer boundary. Matter never does. In either direction. Item duplication is structurally impossible.

**Upgrade path:** When NPC crew ships, Shells evolve into Agent Smithing. The inert clone in the bed becomes a living NPC crew member. Player takes over the NPC instead of a blank Shell. Same mechanic, same Relay Beacon, same transfer UI. Only the body changes from inert to active.

### COMMUNITY COUNTERARGUMENTS TO CONSIDER

- Fast travel becomes mandatory once introduced — game and community optimize around it, eroding social structure
- Breaks player-driven economy: regional scarcity disappears, hauling/escort/refueling/repair roles lose purpose, markets flatten (documented in New World and EVE Online)
- "NPC Crew Tinfoil Theory": if CIG is considering teleportation instead of Agent Smithing, does this signal NPC crew won't happen?
- Convenience treadmill: "those who demand the most convenience are the first to lose interest"

### YOUR TASK

Given the above context, constraints, community proposals, and synthesized hybrid solution:

1. Evaluate the Imprint Shell Network against CIG's internal technical constraints and development timeline.
2. Generate a phased implementation plan:
   - **Phase 1 (Pre-1.0):** What can ship with existing tech? (Bed Log Transit, Commercial Flight infrastructure, Crew Quarters Registry as interim)
   - **Phase 2 (1.0):** Imprint Shell system (Shells, Relay Beacons, Imprint Terminals, degradation timers)
   - **Phase 3 (Post-1.0 / NPC Crew):** Evolution to full Agent Smithing via NPC crew integration
3. Identify technical dependencies, risks, and engineering cost estimates for each phase.
4. Propose tuning values for: Shell cost, Relay Beacon tiers/capacity/range, degradation timer length, transfer cooldown, Contractor Shell restrictions.
5. Draft the in-universe lore entry that introduces Imprint Shell technology (grounded in existing FTL comms and cloning lore).
6. Identify any edge cases or exploit vectors not already addressed in the anti-exploitation design.

---

*This document was compiled from community analysis of 11 proposals, 7 counterargument threads, player data, and 13+ years of Star Citizen design pillar documentation. All community sources are linked in the full analysis document.*
