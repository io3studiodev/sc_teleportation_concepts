# Star Citizen Fast Travel Solutions — Community Ideas Megathread

## The Problem

It currently takes 10-30 minutes to group up with friends or other players. Quantum travel times, spawn locations, and the sheer scale of the universe make casual grouping painful. CIG has floated "fast travel to party leader" as a potential solution, but the community is rightfully concerned that teleportation undermines the persistent, physicalized universe that defines Star Citizen.

**This thread compiles community-sourced ideas that solve the grouping problem WITHOUT breaking the core pillars of the game.**

## The Rules

Any proposed solution must respect these non-negotiable constraints:

1. **Persistence** — "If you drop a coke can on a planet, it will still be there a week later." Objects, bodies, and world state don't vanish for convenience.
2. **Physicalization** — Every player, NPC, bullet, and ship component is a real object in the world obeying physics. Players must exist as physical bodies at all times.
3. **Lore Consistency** — Solutions should fit within established Star Citizen fiction. FTL communication now exists in-lore (Dr. Betel's breakthrough, December 2025), but FTL matter transport does not.
4. **One System** — The solution should work across multiple use cases (ship crewing, open world grouping, instanced content) as a single unified mechanic, not three separate band-aids.

## Scoring Rubric

Each idea is scored 1-5 across seven axes. A score of 1 on Physicalization or Persistence is effectively disqualifying.

| Axis | Weight | Description |
|------|--------|-------------|
| **Physicalization Compliance** | High | Does the player remain a physical object in the world at all times? No popping in/out of existence. |
| **Persistence Compliance** | High | Does it respect the "coke can" rule? No phasing, instancing tricks, or world-state cheats. |
| **Lore Compatibility** | Medium | Could this plausibly exist in the Star Citizen universe without contradicting established fiction? |
| **Effectiveness** | High | Does it meaningfully reduce the 10-30 minute grouping time? |
| **Exploitability** | Medium | How resistant is this to abuse? (Combat repositioning, cargo teleporting, consequence evasion, gear duplication) |
| **Implementation Feasibility** | Low-Medium | Can CIG realistically build this given known tech and scope? |
| **Versatility** | Medium-High | Does a single system cover ship crewing, open world grouping, AND instanced content? |

---

## IDEA #1: Agent Smithing

**Composite Score: 30/35**

**Original Concept:** Community discussion dating back to ~2015, based on the "Agent Smith" concept — a player's consciousness takes over an existing NPC body at the destination.

### Summary

Players transfer their consciousness into an NPC crew member aboard a party leader's ship, or into a hireable NPC at an instanced mission entrance. Instead of physically traveling, you take control of a body that's already physically present. Your original body remains wherever you left it (asleep in a bed, in a pod, etc.), persistent and vulnerable. You inherit the NPC's equipment (a basic ship uniform — essentially nothing). The ship owner pre-stocks weapons and armor in the armory for smithed-in crew to equip.

### How It Works Across Use Cases

- **Ship Crewing:** Smith into an NPC sleeping in crew quarters. Wake up in a ship uniform, gear up from the ship's armory.
- **Open World Grouping:** Smith into an NPC near the party leader's location.
- **Instanced Content:** Smith into a hireable guard NPC at the mission entrance. You control the guard's body, cannot pick up or extract loot, and despawn when the mission completes. The party leader extracts loot via existing freight elevator systems.

### Anti-Exploitation Mechanics

- **Token System:** Ship owners purchase "crew hire tokens" at ports. Each token fills one bed/NPC slot, enabling one smith-in. 8 beds = 8 tokens max. Tokens are consumed on use, requiring a port visit to restock. Tokens are non-physical (cannot be hoarded in cargo).
- **Gear Restriction:** You spawn in the NPC's ship uniform — no personal gear transfers in either direction. The ship owner must pre-stock weapons/armor in the ship's armory.
- **One Spawn Per Token:** After the initial smith-in, you rely on the ship's existing medbed/medgel system. No infinite reinforcements.
- **Smith-Out Rules:** When you disconnect/smith-out, you return to your original body wherever you left it. The NPC body drops or goes limp with whatever gear it was holding. Gear stays with the NPC — you cannot use smithing to teleport equipment. The ship owner can recover the gear from the NPC corpse.
- **Instanced Loot Lockdown:** When smithed into a guard for instanced content, you cannot pick up loot or carry anything out. You despawn on mission completion.

### Scoring Breakdown

| Axis | Score | Reasoning |
|------|-------|-----------|
| Physicalization | 5/5 | No teleportation occurs. A physical NPC body already exists at the location. You change who controls it. Your original body persists. |
| Persistence | 4/5 | Strong — original body persists, NPC body persists. Minor deduction for unresolved edge cases around the original body's vulnerability while smithed out. |
| Lore Compatibility | 4/5 | FTL communication exists in-lore, making consciousness transmission plausible. DNA imprinting/cloning tech is established. "Remote mind control of a body" is a step beyond cloning but not a huge leap. Needs its own lore entry. |
| Effectiveness | 5/5 | Instant grouping. 30 minutes of travel reduced to a menu interaction and a wake-up animation. |
| Exploitability | 4/5 | Token system, gear restrictions, and loot lockdowns close most abuse vectors. Remaining question: should smithing into a ship actively in combat be restricted? Tuning decision for CIG. |
| Feasibility | 3/5 | Requires NPC crew to exist on ships (delayed past 1.0). However, enemy AI crews already control turrets and perform tasks. Bed log-in/log-out mechanics exist. The NPC "meat suit" concept is simpler than full AI crew — it just needs to sleep in a bed and be takeover-ready. |
| Versatility | 5/5 | One mechanic covers ship crewing, open world grouping, and instanced content. Single system, multiple applications. |

### Key Strengths

- Nothing teleports. A body was already there — you just change who's driving.
- Every anti-exploit mechanic maps to systems that already exist (medbeds, medgel, tokens/consumables, armories, freight elevators).
- Leverages crew quarters that currently serve almost no gameplay purpose.

### Key Risks

- Depends on NPC crew tech that CIG has delayed past 1.0, though the "sleeping meat suit" version is far simpler than full AI crew.
- "Smithing into active combat" needs clear rules to prevent instant reinforcement drops.

---

## IDEA #2: Transfer Transit (Temporary Clone)

**Composite Score: 27/35**

**Original Post:** [Maybe Transfer Transit is the way?](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/maybe-transfer-transit-is-the-way) — Posted May 8th, 2026

*Inspired by the Transfer Transit system from the sci-fi series Dark Matter.*

### Summary

A player enters a pod at their current location, and their consciousness is transmitted into a short-lived clone body generated at the destination. The clone has a built-in lifespan timer — it is inherently temporary. When the timer expires or the clone dies, the accumulated memories sync back to the original body, which wakes up in the pod. If the clone is killed before syncing, those memories are lost (consequence mechanic). The player is always anchored to their original physical location.

### How It Works Across Use Cases

- **Ship Crewing:** Clone generated from a pod aboard a friend's ship. Play together until the timer expires.
- **Open World Grouping:** Clone into a pod near the party leader. Temporary session-based grouping.
- **Instanced Content:** Clone pods placed at mission entrances. Timer naturally scopes to mission duration.

### Scoring Breakdown

| Axis | Score | Reasoning |
|------|-------|-----------|
| Physicalization | 4/5 | Original body stays physical in the pod. Clone is physical at the destination. However, the clone body is being *generated* at the destination — materializing matter from nothing. Where does the clone come from? Needs a physical source (bio-printer, pod, pre-placed infrastructure). |
| Persistence | 4/5 | Original body persists in the pod. But the clone despawning on timer expiry needs a physicalized explanation — bodies don't just vanish. Does it die? Dissolve? Leave a corpse? The "coke can rule" applies to clone remains. |
| Lore Compatibility | 3/5 | Cloning and DNA imprinting exist in SC lore. FTL consciousness transmission is plausible post-Betel. But instant remote clone *fabrication* is a significant leap beyond "respawn at a medbed you previously imprinted at." Would require substantial new lore. The original poster acknowledged this: "attempting a lore explanation would be insanely hard." |
| Effectiveness | 5/5 | Solves the grouping problem. Clone in near your friend, play together, timer expires or you return. Fast. |
| Exploitability | 4/5 | The ticking clock is a natural anti-exploit — you can't stay forever, preventing permanent relocation abuse. Clone death = lost memories adds consequence. Still needs gear/loot restrictions similar to Agent Smithing to prevent duplication. |
| Feasibility | 3/5 | Requires building clone fabrication systems, timer mechanics, memory sync on death/expiry, and pod infrastructure at destinations. More new tech than Agent Smithing, which piggybacks on existing NPC bodies and bed mechanics. |
| Versatility | 4/5 | Works for ship crewing and open world grouping. Instanced content is slightly awkward — clone pods at mission entrances work but feel less narratively natural than smithing into a guard NPC who's already there. |

### Key Strengths

- The timer is an elegant built-in guardrail that Agent Smithing doesn't naturally have.
- Clear "you are always anchored to your real location" philosophy — this is explicitly a temporary visit, not a relocation.
- Memory loss on clone death is a meaningful consequence that discourages reckless play.

### Key Risks

- Clone body materialization is hard to justify in a physicalized universe without significant new infrastructure and lore.
- Clone corpse/despawn on timer expiry needs a physicalized explanation.
- More new engineering required compared to solutions that leverage existing NPC and bed systems.

### Possible Hybrid

Agent Smithing's "take over an existing NPC body" approach combined with Transfer Transit's "ticking clock on how long you can stay" could be stronger than either idea alone. You occupy a body that's already physically there (no materialization problem), but you have a limited window before your consciousness snaps back to your original body.

---

## IDEA #3: "Fix the Friction First" (No Fast Travel Needed)

**Not Scored — Alternative Philosophy**

**Original Posts:**
- [Before we try teleportation](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/before-we-try-teleportation) — Posted May 10th, 2026
- [The teleport debate](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/the-teleport-debate) — Posted May 10th, 2026

### Summary

This isn't a fast travel mechanic — it's the argument that teleportation is treating the symptom instead of the disease. The 30-minute grouping time is the result of dozens of small friction points compounding on each other. Fix those first, and the problem may shrink enough that teleportation isn't necessary.

### The Data: What's Actually Eating Our Play Time?

Community-generated Pareto analysis (sourced from [The teleport debate](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/the-teleport-debate)) breaks down where time is actually lost when trying to group up. The numbers are community-estimated but align with long-term player experience:

- **Loading ship with vehicles/boxes: 30 minutes** — by far the largest single time sink
- **Need to switch server (bad performance, mission bugged): 15 minutes**
- **ASOP: Ship location is unknown: 10 minutes**
- **Jump Point is broken: 10 minutes**
- **Inventory doesn't load: 8 minutes**
- **Can't set QT route: 8 minutes**
- **Ship spawns upside down: 7 minutes**
- **Fall through floor: 6 minutes**
- **"I can't see your marker, let's remake the party": 6 minutes**
- **Hangar doors won't open: 5 minutes**
- **"Who is party lead, can I get an invite?": 5 minutes**
- **Actual travel time: 5 minutes**

**The critical takeaway: actual travel time accounts for roughly 4% of total time lost.** The top 4 issues alone (load ship, switch server, ASOP unknown, jump point broken) account for ~57% of all lost time. You hit 80% of the problem around the 7th item. Almost all of it is bugs and friction, not travel.

**The community isn't asking for teleportation to skip travel — they're asking for teleportation to skip bugs. That's a completely different problem with a completely different solution.**

### Proposed Friction Reductions

- Allow multiple ships to be called up in hangars simultaneously.
- Replace real elevators with instant-load transitions (invisible teleportation behind closed doors — players won't notice and it stops the elevator death bugs).
- Ships stored inside another ship's hangar should be covered by the parent ship's insurance/reclaim.
- Significantly reduce quantum jump times, potentially turning QT into an interactive mini-game (like wormhole traversal) instead of passive waiting.
- Get suit lockers working and make stored equipment part of ship insurance.
- Improve social tools and add sharable beacons for easier coordination.
- Fix "jumping back to mothership" functionality.
- **Autopilot:** Let players set a QT destination and AFK while the ship physically flies there. The ship remains real, interceptable, in the world — it's not fast travel, it's just making slow travel less demanding of active attention. Similar to EVE Online's autopilot system.
- **In-Game Calendar / Event Planner:** ([Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-is-not-the-answer-a-calender-is)) A WoW-style calendar where org leaders can schedule events, players can sign up, and everyone sees upcoming activities. The argument: the real time waste isn't travel, it's *coordination*. People show up late, aren't ready, don't know when to log in. If everyone plans ahead and is in position before the activity starts, much of the grouping delay disappears. Doesn't solve the "I have 45 minutes and want to join something NOW" case, but for organized group content it eliminates coordination overhead.
- **Group Bed Log (Fix, Not Feature):** ([Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-is-stupid-group-bed-log-should-be-prio)) If a crew bed-logs on a ship together, they should ALL be able to spawn back on that ship next session — in the same location, in the same state. The ship owner should be able to grant permissions for crew members to spawn the ship even if the owner isn't online first. Once the ship is in-game, anyone who bed-logged on it should be able to spawn aboard. This isn't a new feature — it's fixing broken functionality. As the poster puts it: "creating a new feature to go around bugs is stupid. CIG just needs to fix these bugs."

### Important Context: The Backspace Problem

Community member DarKsaid raised a critical point: players already have "teleportation" — it's called backspacing (suiciding to respawn at your last medbed). This works *now* because Death of a Spaceman penalties aren't implemented yet. Once they are, each death will cost a clone life (finite supply), trigger death taxes, asset transfer fees, reputation loss, and skill/perk degradation. The current backspace workaround will become prohibitively expensive, meaning the grouping problem actually gets *worse* post-1.0 without a solution.

### Why This Isn't Scored

This is a collection of QoL improvements rather than a single unified system, so the rubric doesn't cleanly apply. However, it's documented here because these improvements are valuable regardless of which fast travel solution (if any) CIG chooses. Reducing QT times and fixing elevators should happen whether or not Agent Smithing or CIVs exist.

### Key Strength

Every item on the list is independently valuable and should probably be done anyway. The data strongly suggests that fixing bugs and friction would eliminate the vast majority of the perceived "travel time" problem without any fast travel mechanic at all.

### Key Limitation

Even with all of these fixed, cross-system travel in a multi-system universe will still take significant time. These changes address the current pain, but as more star systems come online, actual travel time will grow and the 5-minute figure will increase substantially. Necessary groundwork, but probably not sufficient long-term.

---

## IDEA #4: C.I.V. / I.R.C. (Cybernetic Imprint Vehicle & Imprint Relay Core)

**Composite Score: 31/35**

**Original Post:** [An alternative to instant PC travel/teleportation — C.I.V. and I.R.C.](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/an-alternative-to-instant-pc-travel-teleportation-) — Posted May 10th, 2026

### Summary

Players log into a pod (shipboard or at a facility) and their consciousness is transmitted into a purpose-built cybernetic body (CIV) stored as physical equipment aboard the destination ship or location. CIVs are paired to an Imprint Relay Core (IRC) — a hardware module installed on the ship — which controls how many CIVs can operate simultaneously and defines their maximum operational range. CIVs are completely inert without a player consciousness driving them, requiring zero NPC AI. Destroyed CIVs leave salvageable wreckage. Destroying the IRC instantly deactivates all paired CIVs, creating tactical counterplay in combat.

### How It Works Across Use Cases

- **Ship Crewing:** IRC installed on ship, CIVs stored in cargo or equipment slots. Party members consciousness-link in and crew up on demand.
- **Open World Grouping:** Works within IRC range of the relay. Party leader's ship acts as the anchor point.
- **Instanced Content:** Requires an IRC and CIV stockpile near the mission entrance — either hauled by the party leader or provided by the facility.

### Key Mechanics

- IRCs are expensive ship components (comparable to high-end ship parts). CIVs cost roughly as much as torpedoes each.
- Each IRC supports a limited number of paired CIVs.
- CIVs have a maximum action radius from their paired IRC.
- Destroyed CIVs can be resynced to a replacement from storage with crew intervention and a time delay.
- Destroying the IRC immediately deactivates all paired CIVs — high-value tactical target.
- Requires both organic and inorganic materials to repair destroyed CIVs.
- Proposed lore hook: Imperator Laylani Addison loosened cybernetics research laws, repurposing technology from recent in-game events for rapid military deployment against the Vanduul.

### Scoring Breakdown

| Axis | Score | Reasoning |
|------|-------|-----------|
| Physicalization | 5/5 | CIVs are physical objects stored in cargo/equipment slots. They exist whether occupied or not. Your original body is in a pod. The IRC is a ship component. Everything is a real, destructible object with mass and location. |
| Persistence | 5/5 | CIVs persist as inert objects when unoccupied. Destroyed CIVs leave salvageable wreckage. The IRC persists as ship equipment. Deactivated CIVs go limp — nothing vanishes. Cleanest persistence answer of any idea so far. |
| Lore Compatibility | 4/5 | The poster provided a ready-made lore hook tying into existing in-game political events. Cybernetic remote-operated bodies fit military sci-fi comfortably. Minor deduction because Star Citizen has historically leaned away from robots/cybernetics in its aesthetic — CIG would need to decide if they want to open that door. |
| Effectiveness | 4/5 | Solves grouping well within range. The range limitation is intentional and prevents system-wide teleportation abuse, but it also means this doesn't help if your friend is across the system and out of IRC range. Less effective than Agent Smithing for long-distance meetups. |
| Exploitability | 5/5 | Strongest anti-exploitation design of any idea. Multiple layered costs: expensive IRC, torpedo-priced CIVs, limited count per IRC, range cap, IRC destruction kills all CIVs (tactical counterplay), resync delays. Very hard to abuse. |
| Feasibility | 4/5 | Major advantage — requires zero NPC tech. CIVs are inert cargo items with a player-control interface. The IRC is a ship component using existing component architecture. Pod login mirrors existing bed logout. Nothing depends on systems CIG has delayed. |
| Versatility | 4/5 | Ship crewing and open world grouping work naturally. Instanced content is slightly less elegant — requires IRC/CIV infrastructure at the mission site, which is less narratively seamless than smithing into a guard NPC who's already there. |

### Key Strengths

- Perfect physicalization and persistence scores — everything is a real object, nothing vanishes.
- Zero dependency on NPC crew tech. Could theoretically be built before 1.0.
- Strongest anti-exploitation design: expensive hardware, limited count, range caps, IRC destruction as tactical counterplay.
- Lore hook pre-written and tied to existing in-game events.

### Key Risks

- Cybernetic "robot bodies" may clash with Star Citizen's aesthetic, which leans heavily into organic physicality (flesh, blood, DNA, cloning). A drone body could feel tonally off even if it's mechanically clean.
- Range limitation helps prevent abuse but also limits effectiveness for long-distance grouping across star systems.
- Instanced content use case requires either hauling IRC/CIV infrastructure to the mission or pre-placing it, which is less seamless than other approaches.

---

## IDEA #5A: Teleport to Docked/Hangared Ship

**Composite Score: 22/35**

**Original Post:** [Teleporting / Fast Travel Would Be Great For Star Citizen](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-fast-travel-would-be-great-for-star-ci) — Posted May 9th, 2026

### Summary

Allow players to teleport directly to their party leader's ship, but only when the ship is docked at a station or sitting inside a hangar. The restriction prevents "clown car" combat drops — you can't teleport to a ship in flight. The poster argues this causes "zero harm" and that the only downside is the removal of wasted time.

### Scoring Breakdown

| Axis | Score | Reasoning |
|------|-------|-----------|
| Physicalization | 2/5 | The core problem: your physical body is at Station A, then it's on a ship at Station B. Your body ceased to exist at one location and appeared at another. The "docked only" restriction limits *when* it happens but doesn't change *what* it is — matter moving instantaneously without traversing the space between. |
| Persistence | 2/5 | During the teleport, you don't exist anywhere in the universe. If someone was watching you at Station A, you'd vanish. Breaks the coke can rule. |
| Lore Compatibility | 2/5 | No established mechanism for matter teleportation in SC lore. FTL communication exists, not FTL transport. Would require inventing matter teleportation tech — a far bigger lore change than consciousness transfer. |
| Effectiveness | 5/5 | Extremely effective. Instant grouping with minimal friction. Solves the practical problem completely. |
| Exploitability | 3/5 | "Docked only" prevents combat drops (smart). But still enables instant relocation of entire orgs across the universe. Strategic positioning and logistics become trivial. Travel time is a strategic resource in a persistent universe. |
| Feasibility | 5/5 | Technically the simplest solution — it's a spawn-point swap. |
| Versatility | 3/5 | Ship crewing — excellent. Open world grouping — only works near docking facilities. Instanced content — unclear application. |

### Key Strength

The poster makes a genuinely compelling argument about the *problem* — as a Legatus-tier backer, even massive financial investment isn't enough to outweigh the reality of how long it takes to do anything fun. "I log into something else instead" is the business case CIG is responding to.

### Key Weakness

The solution is functionally just teleportation with a condition attached. It prioritizes convenience (valid) over the simulation pillars (the thing the community is trying to protect). The "docked only" rule is smart game design but doesn't address the physicalization or persistence violations.

---

## IDEA #5B: Paid NPC Transport Service

**Composite Score: 23/35**

**Original Post:** [Teleporting / Fast Travel Would Be Great For Star Citizen](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-fast-travel-would-be-great-for-star-ci) — Posted May 9th, 2026

### Summary

Pay an NPC transport service to move you between major locations. Cost is distance-based, creating a money sink. You "board" the shuttle, the screen fades to black, and you arrive at your destination. Modeled after WoW flight paths, DAoC horses, PlanetSide 1's HART system, or SWG shuttle services.

### Scoring Breakdown

| Axis | Score | Reasoning |
|------|-------|-----------|
| Physicalization | 3/5 | Better than raw teleportation because there's a narrative wrapper — you're "boarding a shuttle." But the screen fades to black and you appear elsewhere. Your body isn't actually on a shuttle traversing space. If someone interdicted that route, there's no shuttle to intercept. It's a loading screen with flavor text. |
| Persistence | 2/5 | During the fade-to-black, you don't exist in the world. No one can interact with you, intercept you, or observe you in transit. That's a hole in the simulation. |
| Lore Compatibility | 4/5 | NPC transport services make perfect sense in-universe. Shuttles, commercial transit, passenger liners — all lore-friendly. The issue is the fade-to-black implementation, not the concept. |
| Effectiveness | 4/5 | Good for cross-system relocation. Cost system adds a money sink. Less instant than raw teleportation, especially if there's a wait for the shuttle. |
| Exploitability | 4/5 | Cost-based pricing naturally limits abuse. Distance pricing prevents trivial cross-system hopping. Tunable via economy. |
| Feasibility | 4/5 | Relatively simple — a paid spawn-point transition with a UI wrapper. |
| Versatility | 2/5 | Only covers point-to-point relocation between stations. Doesn't address ship crewing or instanced content at all. Would need a separate system for those. |

### Key Strength

The concept of NPC transport is lore-friendly and economically balanced. Cost-based pricing is a natural anti-abuse mechanism.

### Key Weakness / Upgrade Path

The weakness is the fade-to-black implementation, not the concept. If the shuttle were a *real physicalized ship* that actually flies the route — one you could see, board, ride on, and theoretically intercept — this idea's scores would jump significantly. Physicalization goes to 5/5, persistence goes to 4-5/5. A physicalized NPC transport network is actually a strong idea hiding inside a weaker implementation proposal. See Idea #6 for exactly this.

---

## IDEA #6: Physicalized Commercial Flights (Genesis Starliner Transit)

**Composite Score: 28/35**

**Original Post:** [Fast Travel done right](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/fast-travel-done-right) — Posted May 10th, 2026

### Summary

Major UEE spaceports have commercial flight terminals with ticket kiosks. You buy a ticket, go to a labeled departure hangar, and board a Genesis Starliner that physically exists in the world. The ship has food shops, seating areas, and large windows — you experience the journey. It travels on rails at dramatically faster QT speeds (system traversal in 1-2 minutes), is invincible during transit, and departs on a timed schedule (every 7-10 minutes per destination). Ships only spawn when a ticket is purchased. Lawless systems get reputation-gated gang-operated shuttles instead of commercial liners. No loading screens, no fade to black.

### How It Works Across Use Cases

- **Cross-System Relocation:** Buy a ticket, board the Starliner, ride to another major spaceport. Gets you to the same city/system as your friends.
- **Lawless Systems:** Reputation-gated gang shuttles with limited destinations — you have to earn access.
- **Ship Crewing / Instanced Content:** Does NOT address these. Would need a complementary system (Agent Smithing, CIV, etc.) for the last mile.

### Key Mechanics

- Departures staggered to avoid clogging large hangar ports, or one hangar dedicated to commercial flights.
- Big screen in lobby shows next departure timers for each destination.
- Only spawns the ship when a player buys a ticket — no empty ships flying back and forth.
- Transit ships travel at 2x+ normal QT/NAV speeds on fixed rails.
- Invincible during transit (gameplay carve-out for public transport).
- Limited to major UEE spaceport destinations — you can't fly commercial to a random outpost.

### Scoring Breakdown

| Axis | Score | Reasoning |
|------|-------|-----------|
| Physicalization | 5/5 | You physically walk to a terminal, buy a ticket, board a real ship, sit in a real seat, look out real windows. The Starliner exists in the world. You exist on it. At no point does anyone stop being a physical object. |
| Persistence | 4/5 | The ship is in the world, you're on it. Minor deduction: invincible ships on rails are a persistence carve-out in a universe where everything is supposed to be destructible. The "ship only spawns when a ticket is bought" is also slightly non-persistent, though justifiable as the Starliner arriving from its previous route. |
| Lore Compatibility | 5/5 | Highest lore score of any idea. Commercial spaceflight is one of the most natural things that should exist in this universe. The Genesis Starliner was literally designed for this role. Spaceports already have commercial flight areas built into their architecture. Rep-gated gang shuttles in lawless systems is a perfect lore touch. |
| Effectiveness | 3/5 | Solves cross-system relocation well but with intentional friction — get to spaceport, wait up to 7-10 minutes for departure, ride the ship, then get from destination spaceport to wherever your friends actually are. Reduces a 15-minute cross-system trip to maybe 5-8 minutes. Meaningful improvement, but not instant grouping. Does not solve "get to your friend's ship in deep space." |
| Exploitability | 5/5 | Near-impossible to abuse. Fixed routes between major ports only. Ticket cost as economic gate. Departure schedules prevent spamming. You're a passenger — can't bring your own ship. Limited destinations in lawless systems behind rep gates. |
| Feasibility | 4/5 | Most tech exists — spaceports, hangars, kiosks, trams/rail systems, QT. Genesis Starliner is planned but not yet in-game. Transit system refactor for server boundaries is in progress. Main new work: scheduling system, accelerated QT for transit ships, invincibility flag. |
| Versatility | 2/5 | The clear weakness. Only covers point-to-point relocation between major spaceports. Doesn't solve ship crewing or instanced content. You'd need a second system alongside this. |

### Key Strengths

- Perfect physicalization — no loading screens, no teleportation, no fade to black. You're a person on a ship the entire time.
- Best lore fit of any proposal. Commercial spaceflight should already exist in this universe.
- The Genesis Starliner was designed for exactly this purpose.
- Essentially unexploitable by design.
- The poster is right that almost no new tech is needed — most building blocks already exist.
- **Supporting evidence:** A separate community post ([Fast travel — Why not use what's already there?](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/fast-travel-why-not-use-whats-already-there)) confirms that major landing zones already have areas labeled "Commercial Flights" with secured passenger transit infrastructure, controlled access terminals, and civilian transportation hub architecture. The physical spaces are literally already built.
- **Additional support:** [YES! To Teleporting in Star Citizen](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/yes-to-teleporting-in-star-citizen) (posted May 9th, 2026) — despite the title, this post advocates for infrastructure-based commercial transit, not raw teleportation. Adds luggage limits, restricted equipment, and ticket-based travel. Useful analogy: "Nobody flies London to Hawaii and says 'thank God I experienced every minute of sitting on that plane.'" The Genesis Starliner, civilian transport careers, and passenger terminals are all already part of SC's lore and architecture.

### Key Weakness

This is a relocation system, not a grouping system. It gets you to the same spaceport as your friends, not onto their ship. For the "last mile" — crewing up a friend's ship, joining instanced content — you still need a complementary system. Pairs naturally with Agent Smithing or CIV as a two-layer solution: Starliner for the cross-system hop, then consciousness transfer for the ship crew-up.

---

## IDEA #7: Crew Quarters Registry ("Agent Smithing Lite")

**Composite Score: 27/35**

**Original Post:** [Crew quarters (an alternative to teleportation)](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/crew-quarters-an-alternative-to-teleportation) — Posted May 9th, 2026

### Summary

Players pre-register to a specific bed on a specific ship by physically visiting it and claiming a bed slot. This also assigns them a suit locker and armor rack. After registering, they go about their normal activities. When the captain needs crew, they use the captain's chair to issue a "call to arms" notification — potentially even to players who aren't logged in (via Spectrum or mobile). If a player accepts, they wake up in the crew quarter bed in their underwear. No gear transfers in either direction. They equip from pre-stocked suit lockers and armor racks aboard the ship. When done, they use the bed to return to their last location with whatever gear they had before. A cooldown timer prevents flip-flopping between ships.

### How It Works Across Use Cases

- **Ship Crewing:** The primary use case. Captain calls, crew wakes up, mission begins. Minimal delay.
- **Open World Grouping:** Works if the party leader has a ship with crew quarters nearby.
- **Instanced Content:** Less clear — would need a variant like mission-specific crew registries.

### Scoring Breakdown

| Axis | Score | Reasoning |
|------|-------|-----------|
| Physicalization | 3/5 | Your actual body materializes in a bed that was empty a moment ago. Unlike Agent Smithing, there's no pre-existing NPC body — your body teleports from wherever you were. The underwear-only restriction means no gear teleports, but the body itself moves instantaneously. |
| Persistence | 3/5 | When you answer the call, your body disappears from wherever you were. When you return via the bed, you vanish from the ship. Two persistence violations per session. |
| Lore Compatibility | 3/5 | Framed as "Agent Smithing Lite" but actually closer to restricted teleportation. Agent Smithing has a lore justification (consciousness transfer into an existing body). This doesn't explain how your physical body moves instantly — it would need its own lore explanation. |
| Effectiveness | 5/5 | Extremely effective. Captain calls, crew wakes up. The out-of-game notification system is a great touch for offline players. |
| Exploitability | 4/5 | Underwear-only spawn prevents gear teleportation. Pre-registration limits access. Cooldown prevents flip-flopping. Registry capacity tied to crew quarter size. Strong safeguards. |
| Feasibility | 5/5 | The killer feature. No NPC tech required. Essentially an extension of bed log-in/log-out plus a registry and notification system. Every component exists. Could ship before 1.0. |
| Versatility | 4/5 | Ship crewing — excellent. Open world — works near ships with crew quarters. Instanced content — needs a variant. Tightly coupled to ships with crew quarters. |

### Key Strengths

- Highest feasibility of any idea — could realistically ship soon with minimal new engineering.
- Gives crew quarters, suit lockers, and armor racks actual gameplay purpose.
- Out-of-game notifications (Spectrum/mobile) extend the system beyond active players.
- Pre-registration adds a social commitment layer — you're *assigned* to this ship's crew.

### Key Risks

- Your body does teleport, even if your gear doesn't. Scores lower than Agent Smithing on the purity metrics.
- Could evolve into Agent Smithing once NPC crew tech exists — ship it now as the "lite" version, upgrade later when NPCs populate crew quarters and players take them over instead of teleporting in.

---

## IDEA #8: Bed Log Transit (Offline Commercial Travel)

**Composite Score: 28/35**

**Original Post:** [Teleporting. Why it doesn't make sense.](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-why-it-doesn-t-make-sense-now-but-coul) — Posted May 9th, 2026 (Idea extracted from point 4 of a larger counterargument post)

### Summary

You go to a transit hub at any major spaceport. Interact with a terminal, select your destination from available commercial routes (major spaceports only). The terminal displays estimated travel time and ticket cost. You confirm, lie down in a transit hub bed, and log out. Your body is now physically aboard a commercial transport — asleep in a sleeper cabin.

A server-side countdown begins from the moment you log out: departure time + travel duration = arrival time. This runs in real-world time whether you're online or offline. Travel duration is proportional to actual in-game distance, calculated at approximately 0.75x of manual QT travel time with a minimum floor of 30 minutes — fast enough that planning ahead is rewarded, slow enough that it's not instant teleportation.

When you log back in: if the timer has completed, you spawn at your destination ("You slept through your commercial flight"). If the timer has NOT completed, you choose — stay committed and wait, or cancel and wake up back at the departure hub (ticket refunded minus a cancellation fee). You're never in limbo.

Ideally, your sleeping body is actually aboard a real physicalized transport during the timer. If someone could board that Starliner mid-flight, they'd find you asleep in a cabin.

### How It Works Across Use Cases

- **Pre-Planned Relocation:** Excellent. Log out at transit hub Tuesday night, log in Thursday for the org event already in position.
- **Ship Crewing:** Does not address — you arrive at a spaceport, not on a friend's ship.
- **Instanced Content:** Does not address.
- **Spontaneous Grouping:** Does not address — requires advance planning.

### Scoring Breakdown

| Axis | Score | Reasoning |
|------|-------|-----------|
| Physicalization | 4/5 | Your body is in a bed at a transit hub, narratively riding a transport. If the transport is a real ship your sleeping body rides on, this is a 5. If it's just a spawn-point change, it's a 3. The concept is sound regardless. |
| Persistence | 4/5 | Your body is in a bed the entire time — at the transit hub or on a transport. Consistent with how bed logging already works. You never just vanish. |
| Lore Compatibility | 5/5 | Sleeper cabins on commercial transit. Red-eye flights. Overnight trains. This is how real-world long-distance travel actually works. Perfect lore fit. |
| Effectiveness | 3/5 | Requires planning ahead — you must bed-log at a transit hub at least 30 minutes in advance. Great for scheduled org events, useless for "my friend just logged in, come join us." |
| Exploitability | 5/5 | Near-impossible to abuse. You're logged out for the duration. Can't use it reactively — must commit in advance. 30-minute minimum prevents rapid abuse. No mid-combat or mid-mission teleportation possible. |
| Feasibility | 5/5 | Bed logging exists. Transit hubs exist. Spawn point selection on login exists. This is essentially "offer a destination picker if you logged out in a transit hub bed." Minimal new engineering. |
| Versatility | 2/5 | Only covers pre-planned relocation between transit hubs. Single use case — but covers that use case perfectly. |

### Key Strengths

- Virtually unexploitable — you can't abuse something that requires you to be logged out for 30+ minutes.
- Trivial to implement — extends existing bed logout mechanics with a destination picker.
- Lore-perfect — sleeper cabins on commercial flights are completely natural.
- Complementary to other systems — use Bed Log Transit to pre-position for scheduled events, use Agent Smithing or CIV for spontaneous ship crewing.

### Key Weakness

Only solves the pre-planned case. If your friend logs in and says "come join us," this does nothing. Needs to be part of a multi-system approach, not a standalone solution.

---

## IDEA #9: Rare Alien Fast Travel Structures (Endgame Discovery)

**Composite Score: 25/35**

**Original Post:** [Teleporting. Why it doesn't make sense.](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-why-it-doesn-t-make-sense-now-but-coul) — Posted May 9th, 2026 (Idea extracted from point 8 of the same post)

### Summary

Ancient alien structures discovered at the edges of explored space that act as bridges between extremely distant locations. Rare, dangerous to access, lore-heavy, discovered through exploration. Not a menu button — something you physically travel to and enter. Bridges gaps "normally not traversable during a single game session." Endgame content, not a daily convenience.

### Scoring Breakdown

| Axis | Score | Reasoning |
|------|-------|-----------|
| Physicalization | 5/5 | You physically travel to the structure, physically enter it, physically exit at the other end. A jump point by another name — fixed, physicalized world infrastructure. |
| Persistence | 5/5 | The structure exists permanently in the world. You exist inside it during transit. Nothing vanishes. |
| Lore Compatibility | 4/5 | Jump points establish that spatial shortcuts exist. Ancient alien structures are part of SC lore. Natural extension, though would need careful introduction. |
| Effectiveness | 2/5 | By design, barely solves the grouping problem. Rare, remote, endgame. You can't use it to meet friends for a Tuesday session. |
| Exploitability | 5/5 | Fixed locations, dangerous access, rare — hard to abuse by definition. |
| Feasibility | 3/5 | Requires building alien structures, new traversal mechanics, and careful world placement. Not trivial but reasonable for post-1.0 content. |
| Versatility | 1/5 | Solves exactly one use case: crossing vast distances in deep space. Doesn't help with ship crewing, instanced content, or any standard grouping scenario. |

### Key Strengths

- Perfect physicalization and persistence. Pure to the simulation philosophy.
- Adds exploration and discovery content alongside the travel mechanic.
- Could create fascinating emergent gameplay around controlling/accessing these structures.

### Key Weakness

This is an exploration feature, not a grouping solution. It's a cool addition to the universe but doesn't address the core problem this megathread exists to solve. Best positioned as a far-future post-1.0 addition, not a near-term answer to the fast travel debate.

---

## IDEA #10: Group Launch (Session-Start Spawn Together)

**Composite Score: 24/35**

**Original Post:** [Not teleport/Fast travel — but group launch](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/not-teleport-fast-travel-but-group-launch) — Posted May 10th, 2026

### Summary

When launching into a server while in a party, you can choose to spawn at the same hangar/station as your party leader instead of your last location. You pay the QT fuel cost for the distance traveled. Only available at session start after being offline for 1+ hours — cannot be used mid-session. Not available outside UEE secure space (can't spawn into Pyro for free). Lore justification: "you traveled there before the session started." A 15-minute window after joining a session may also be available, after which the option closes.

### Scoring Breakdown

| Axis | Score | Reasoning |
|------|-------|-----------|
| Physicalization | 3/5 | Your body spawns somewhere it wasn't when you logged out. Since you were offline, no one watched you vanish — less disruptive than mid-session teleportation. The "you traveled there offscreen" narrative is thin but acknowledges travel occurred. |
| Persistence | 3/5 | Your last-known position changes between sessions. Creates edge cases: if your ship was parked at Lorville and you spawn at Microtech, where's your ship? What about belongings left behind? |
| Lore Compatibility | 3/5 | "You traveled there before the session" is handwaving, but paying the QT fee reinforces that travel happened. UEE-only restriction is a nice lore-consistent touch — traveling through Pyro isn't something you can "just do." |
| Effectiveness | 4/5 | Solves start-of-session grouping well. Doesn't help mid-session, which is by design. Still need another system for spontaneous grouping. |
| Exploitability | 5/5 | Very hard to abuse. Requires 1+ hour offline. Can't use mid-session. Costs QT fuel. UEE space only. Can't chain it. |
| Feasibility | 4/5 | Spawn point selection on login plus party integration. Straightforward engineering. |
| Versatility | 2/5 | Session-start only. Doesn't help with ship crewing, instanced content, or mid-session grouping. |

### Key Strengths

- Solves the most common scenario: "we all want to play tonight but we're scattered across the system."
- The offline requirement makes it unexploitable — you literally can't use this tactically.
- QT fuel cost and UEE-only restriction keep it grounded.

### Key Weakness

Only addresses session-start grouping. For everything else (ship crewing, mid-session meetups, instanced content), you still need a separate system.

---

## IDEA #11: Formalized Medbed Clone-In (Death as Fast Travel)

**Composite Score: 25/35**

**Original Post:** [Teleporting already exist, and how to implement it.](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-already-exist-and-how-to-implement-it) — Posted May 10th, 2026

### Summary

Formalize what players already do as an exploit. Instead of backspacing and hoping, let players deliberately trigger a clone revival at a party member's medbed. You die/clone, wake up at the medbed with no gear, consuming medgel. Your consciousness is transmitted to a new clone body — that's the existing lore. You rely on whatever gear the party has ready for you. This isn't a new system — it's a refined version of something players have done for years.

### Scoring Breakdown

| Axis | Score | Reasoning |
|------|-------|-----------|
| Physicalization | 3/5 | A clone body is generated at the medbed — physical once it exists. But the original body situation is unclear (corpse? vanish?). The clone generation at a distant medbed has the same materialization question as Transfer Transit. |
| Persistence | 3/5 | Original body should leave a corpse (persistence). Clone appears from medbed — medgel consumption provides a physicalized resource cost for the materialization. |
| Lore Compatibility | 4/5 | Well-grounded in existing SC lore. Cloning, DNA imprinting, medbed revival — all established. The poster is right: this is already possible. Formalizing it just removes the awkward suicide step. |
| Effectiveness | 4/5 | Fast grouping — clone in, gear up from whatever the ship has. Requires party leader to have a medbed with medgel and your DNA imprint. |
| Exploitability | 3/5 | Medgel limits uses. But the fundamental tension: once Death of a Spaceman is live, each use costs a clone life. Either the DOAS penalty makes this unusable for casual grouping, or the penalty is light enough to be easily abused. Hard to tune — the system works against its own use case as the game matures. |
| Feasibility | 5/5 | Everything already exists. Medbeds, medgel, DNA imprinting, clone revival. This is literally allowing deliberate use of an existing system. |
| Versatility | 3/5 | Works wherever medbeds exist — ships with medbeds, stations. Doesn't work for instanced content unless medbeds are placed at entrances. Limited by medbed placement. |

### Key Strengths

- The poster's core insight is sharp: this already happens. CIG might as well design around it rather than pretend it doesn't exist.
- Zero new engineering — just UI/UX to formalize an existing exploit into a feature.
- Medgel consumption creates a tangible, physicalized cost.

### Key Weakness

The Death of a Spaceman tension is fundamental. If DOAS penalties are meaningful (as intended), voluntarily dying to fast travel becomes increasingly punishing — burning clone lives for convenience. The system that makes it possible is the same system designed to make death consequential. These goals conflict directly, and CIG would have to decide which matters more.

---

## Community Counterarguments Against Fast Travel

These posts don't propose solutions but articulate *why* the community cares so deeply about this issue. They provide essential context for understanding why the rubric weights physicalization and persistence so heavily.

### "Time is a strategic resource"

**[Without time, distance doesn't matter](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/without-time-distance-doesn-t-matter)** — Posted May 9th, 2026

The strongest philosophical counterargument. The core thesis: travel time isn't wasted time, it's a *strategic variable*. Logistics, troop movement, "calling the banners" and gathering forces — all of that gameplay evaporates if you can teleport. Distance without time is meaningless. Why build better components? Why own faster ships? Why have a physical universe at all? The poster draws on WoW's early magic — it felt *huge* because it took time to cross. They also make the convenience treadmill argument: "those who demand the most convenience are the first to lose interest when their demand for more time-saving mechanics isn't satisfied. And you will erode this game to an arcade game."

### "Don't compromise the vision"

**[Please, Please, CIG Don't implement Fast Travel/Teleporting](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/please-please-cig-don-t-implement-fast-travel-tele)** — Posted May 9th, 2026

A straightforward appeal to preserve what makes Star Citizen unique. Includes an interesting minority perspective: the universe already feels *too small* — QT travel is already too fast, not too slow. One tank of fuel to traverse the known universe undermines the sense of scale. Also argues: get robust social tools in before even considering fast travel. If the social infrastructure is missing, that's the problem to solve first.

### "Fast travel doesn't stay optional — it becomes mandatory"

**[Teleporting. Why it doesn't make sense.](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-why-it-doesn-t-make-sense-now-but-coul)** — Posted May 9th, 2026

The behavioral argument: the moment fast travel exists, the game and community optimize around it. Players solo until something goes wrong, then it's "just teleport to me." This erodes the social structure the game is trying to build — traveling *together* becomes something you skip instead of something you do. The convenience treadmill is real.

### "It breaks the player-driven economy"

**[Teleporting. Why it doesn't make sense.](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-why-it-doesn-t-make-sense-now-but-coul)** — Posted May 9th, 2026

The economic argument, backed with cautionary examples from other games: regional scarcity disappears if players can instantly relocate. Hauling becomes pointless (no time, no risk, no profit margin). Support roles vanish (refuelers, repair ships, recovery — all rely on people being in transit). Markets flatten unrealistically. The poster cites New World's economy collapse after fast travel improvements, and EVE Online's "blue donut" problem where large alliances project power instantly across vast distances, crushing smaller groups. These aren't theoretical — they're documented outcomes from live games.

### "Teleporting creates more problems than it solves"

**[Teleporting is poorly conceived](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-is-poorly-conceived-or-at-best-kind-of)** — Posted May 9th, 2026

Stress-tests teleportation with specific abuse scenarios: bounty targets teleporting away mid-capture, losing a fight and teleporting to safety, unlimited combat reinforcements appearing from nowhere during sieges, economic scouting (find resources, teleport to get the right ship, come back). The poster argues CIG would inevitably need a "suite of limitations, counters, costs, new lore, reconsiderations, rebalances" to prevent abuse — so why build teleportation and then spend equal effort preventing its misuse?

The post also endorses Agent Smithing as CIG's original clean solution and raises the **NPC Crew Tinfoil Theory**: the fact that CIG is even considering teleportation instead of Agent Smithing likely means NPC crew won't happen in any meaningful timeframe. If NPC crew were coming, Agent Smithing would make teleportation unnecessary. This is relevant context for evaluating the feasibility axis across all ideas.

### "Social tools first, fast travel never"

**[Instant Travel.. Please no..](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/instant-travel-please-no)** — Posted May 9th, 2026

Argues CIG should implement robust social tools/features for orgs and friends first, then re-evaluate whether fast travel is actually needed. Compares Star Citizen to its intended niche: this is not a quick-session game. If players have limited time, SQ42, Arena Commander, or other games serve that need. Star Citizen is a thinking game requiring planning and strategy.

### What these arguments mean for the rubric

These counterarguments are why any solution scoring 1-2 on Physicalization or Persistence should be viewed skeptically regardless of its Effectiveness score. The community funded a physicalized, persistent universe — not a faster way to skip it. The challenge is solving the grouping problem *within* those constraints, not by abandoning them.

The economic arguments are particularly important: even ideas that score well on physicalization should be evaluated for whether they undermine travel-dependent careers (hauling, escort, refueling, repair, recovery). No idea in this megathread has been scored on economic impact yet, but it's worth noting as a potential eighth rubric axis.

---

## PROPOSED HYBRID: Imprint Shell Network (Layered Fast Travel System)

**Composite Score: 33/35**

**Origin:** Synthesized from analysis of all 11 community ideas, 7 counterarguments, community data, and the design constraints of Star Citizen's physicalized, persistent universe. This proposal takes the strongest scoring elements from the top ideas and combines them into a single coherent system with two complementary layers.

### The Core Insight

No single idea scored perfectly across all seven axes. But the weaknesses of each idea are covered by the strengths of another. The top ideas naturally sort into two complementary categories: **long-haul relocation** (getting to the same system/station) and **last-mile grouping** (getting onto a friend's ship or into instanced content). Combining them creates full coverage.

### Layer 1: Long Haul — Physicalized Commercial Flights + Bed Log Transit

This layer handles cross-system relocation. It uses two ideas that already scored 28/35 each, both with perfect or near-perfect physicalization and lore scores.

**Real-Time Transit:** Buy a ticket at a spaceport kiosk, board a Genesis Starliner (or equivalent commercial ship), ride it to another major spaceport. The ship physically exists in the world. Scheduled departures every 7-10 minutes. Accelerated QT speeds. Lawless systems use rep-gated gang shuttles. No loading screens. For when you're already in a session and need to relocate.

**Pre-Planned Transit (Bed Log Transit):** For when you want to reposition between sessions — the "our org event is tomorrow night" scenario. Here's exactly how it works:

1. **Booking:** Walk to a transit hub at any major spaceport. Interact with a terminal. Select your destination from available commercial routes (major spaceports only — you can't transit-sleep to a random outpost). The terminal displays the estimated travel time and ticket cost.

2. **Departure:** Confirm the booking, lie down in a transit hub bed, and log out. Your body is now physically aboard a commercial transport — asleep in a sleeper cabin. A server-side countdown begins from the moment you log out: departure time + travel duration = arrival time. This timer runs in real-world time whether you're online or offline.

3. **Travel Duration:** The transit takes real-world time proportional to actual in-game distance, calculated at approximately **0.75x of manual QT travel time, with a minimum floor of 30 minutes.** This means planning ahead is rewarded (it's faster than flying yourself), but it's not instant teleportation. The 30-minute floor prevents abuse on short-distance routes. Cross-system trips through jump points take proportionally longer. Routes only exist along established commercial lanes — some systems may have limited or no service.

4. **Arrival — Logging Back In:** When you log in after the timer has completed, you spawn at your destination spaceport. "You slept through your commercial flight." If you log in before the timer has completed, you get a choice: **stay committed** (remain logged out or sit in the transit ship if physicalized, and wait for arrival) or **cancel the trip** (wake up back at the departure hub where you started, ticket refunded minus a cancellation fee). You are never in limbo — you're either on the transport or you're back where you started.

5. **Physicalization:** Ideally, your body is actually aboard a real transport ship during the timer. If CIG physicalizes the transit fleet, a Starliner departs on schedule with your sleeping body in a cabin. If someone could board that ship mid-flight, they'd find you asleep. This is the cleanest persistence answer. At minimum, the server tracks your body as "in transit" so it exists somewhere in the world at all times — it never simply doesn't exist.

These two modes cover the full spectrum of relocation needs: Real-Time Transit for "I need to move right now during my session," Pre-Planned Transit for "I need to be somewhere tomorrow." The infrastructure already exists in-game — commercial flight terminals are built into every major landing zone.

### Layer 2: Last Mile — Imprint Shells (The New Mechanic)

This is the unified system that handles ship crewing, open world grouping, and instanced content with a single mechanic. It synthesizes the best elements of Agent Smithing (consciousness transfer into a pre-existing body), CIV (physical hardware with no NPC dependency), Transfer Transit (ticking clock), and Crew Quarters Registry (leverages crew quarter infrastructure).

**What is an Imprint Shell?**

An Imprint Shell is a purpose-grown organic clone body in stasis. It is a **physical, purchasable, consumable item** — like a torpedo or medgel cartridge. Shells are grown at medical facilities and sold at ports. They must be physically transported to a ship and placed in a crew quarter bed. When not occupied by a player, a Shell is an inert body sleeping in a bed — fully physicalized, fully persistent. It obeys the coke-can rule: if you leave a Shell in a bed, it's still there a week later.

**How It Works:**

1. **Setup (Ship Owner):** The ship owner purchases Imprint Shells at a port. They carry them aboard (physical cargo) and place them in crew quarter beds. The ship must also have a **Relay Beacon** installed — a ship component that enables consciousness transmission to the Shells aboard. Each Relay Beacon supports a limited number of Shells based on its tier.

2. **Transfer (Crew Member):** A player at any port or station walks to an **Imprint Terminal** (a facility in the medical/transit area). They select a party member's ship from the terminal UI. Their consciousness is transmitted via FTL communication (Dr. Betel's breakthrough) to an available Shell aboard that ship. Their **real body enters stasis at the terminal** — physical, persistent, vulnerable. It can be found, observed, even looted if the terminal is in an unsecured area.

3. **Arrival:** The player wakes up in the Shell's body, lying in the crew quarter bed. They're wearing a **medical gown** — nothing else. No weapons, no armor, no personal inventory. Everything they own stays with their real body at the terminal. They gear up from the ship's armory, weapon racks, and suit lockers — whatever the ship owner has pre-stocked.

4. **Session:** The player operates normally in the Shell — fighting, crewing turrets, completing missions. The Shell is a full physical body. It can be injured, healed with medbeds, equipped with gear from the ship.

5. **Departure:** When the player is done, they return to a bed and initiate transfer-out. Their consciousness snaps back to their real body at the Imprint Terminal. The Shell **dies and leaves a corpse** in the bed. Whatever gear the Shell was wearing stays with the corpse. The ship owner recovers the gear and disposes of the body. **Nothing transfers back with the player's consciousness — no gear, no items, no loot.** This is absolute: your consciousness moves, nothing else, in either direction. Item duplication is impossible because no items ever cross the transfer boundary.

6. **Timer:** Each Shell has a **biological degradation timer** (4-8 hours, tunable). When the timer expires, the Shell begins to fail and the player's consciousness snaps back to their real body. This prevents indefinite occupation and creates a natural session window.

7. **Shell Death:** If the Shell is killed in combat, the consciousness snaps back immediately. The Shell corpse persists with its gear. The player wakes up at their real body. Potential tuning option: partial memory loss on Shell death (borrowed from Transfer Transit) to discourage reckless play.

**How It Handles Each Use Case:**

- **Ship Crewing:** Owner buys Shells, places them in crew beds, installs Relay Beacon. Friends transfer in from any port, wake up in crew quarters, gear up, crew the ship. This is the primary use case and it works seamlessly.

- **Open World Grouping:** Same mechanic. The party leader's ship is the anchor point. Transfer into a Shell aboard, then take a shuttle or EVA to wherever the group activity is. The ship needs to be within the Relay Beacon's operational range of the activity.

- **Instanced Content:** Facilities near instance entrances (e.g., Municipal Works, Siege of Orison staging areas) have **Contractor Shells** available for hire. The party leader pays to activate them at the facility. Players transfer into Contractor Shells at the mission entrance. Contractor Shells operate under restricted rules: they **cannot pick up loot, cannot carry items out, and despawn when the mission completes.** The party leader extracts loot via existing freight elevator systems. This completely prevents duplication and loot exploitation.

### Anti-Exploitation Design

Every anti-abuse mechanic maps to a physicalized, in-universe cost:

- **Shells are expensive consumables.** Each one costs roughly what a torpedo costs. A ship with 8 crew beds needs 8 Shells — real money, real logistics. You have to fly to a port, buy them, haul them to your ship, and place them. They're one-use: once the player leaves, the Shell dies.
- **Relay Beacon limits.** The Beacon is a ship component with a tier-based capacity. Small ships might support 2-3 Shells, capital ships might support 20+. The Beacon also has a **maximum operational range** — you can't transfer into a Shell that's too far from a relay network or Imprint Terminal.
- **No gear transfers.** Absolute rule. Your real body keeps everything it had. The Shell starts with a medical gown. Whatever the Shell picks up stays with the Shell corpse. Consciousness moves, matter doesn't. Item duplication is structurally impossible.
- **Real body vulnerability.** Your real body is in stasis at an Imprint Terminal. It's physical and persistent. In secure UEE space, this is low-risk. In a lawless station, someone could theoretically find and loot your sleeping body. This creates a natural risk/reward calculation — transferring from a safe port is fine, transferring from a shady Pyro station carries risk.
- **Degradation timer.** 4-8 hours before the Shell fails. You can't permanently relocate via Shell — it's always temporary.
- **Combat lockout.** Cannot transfer into a Shell aboard a ship that is in active combat (shields taking fire, weapons deployed, hostile proximity alert). Prevents instant combat reinforcement drops.
- **Cooldown.** After transferring out of a Shell, there's a cooldown (30-60 minutes) before you can transfer into another one. Prevents rapid Shell-hopping across the universe.
- **Contractor Shell restrictions.** For instanced content, Contractor Shells cannot interact with loot, cannot carry items, and despawn on mission completion. Zero extraction exploit potential.

### Lore Justification

Every element of this system is grounded in existing Star Citizen lore:

- **FTL consciousness transmission:** Dr. Betel's FTL communication breakthrough (December 2025 lore) established that information can be transmitted faster than light. Consciousness is information. This is the transmission mechanism.
- **Clone bodies:** DNA imprinting, cloning, and medbed revival are all established SC technologies. Imprint Shells are a refinement — purpose-grown clone bodies optimized for temporary consciousness hosting rather than permanent revival. Think of them as "disposable clones" compared to the permanent clone you respawn into.
- **Military application:** The Vanduul war provides immediate lore justification. Rapid force deployment without moving troops across systems is an obvious military need. Imperator Addison's administration could have fast-tracked the technology for the war effort, with civilian applications following.
- **Shell degradation:** Clone bodies grown quickly for temporary use aren't as stable as a full clone grown for permanent revival. They degrade. This is biologically intuitive and provides the in-universe explanation for the timer.

### Feasibility & Upgrade Path

**What needs to be built:**
- Imprint Shell items (physical cargo/consumable — item system exists)
- Relay Beacon ship component (component system exists)
- Imprint Terminal facility object (terminal/kiosk system exists)
- Consciousness transfer UI (party system + destination picker)
- Degradation timer (timer mechanics exist)
- Contractor Shell variant for instanced content
- Shell corpse cleanup system

**What already exists:**
- Beds and crew quarters with log-in/log-out functionality
- Suit lockers and armor racks
- Medical/cloning lore and DNA imprinting
- FTL communication lore
- Ship component architecture
- Consumable items (medgel, torpedoes)
- Party/group systems

**No NPC crew AI is required.** Shells are inert objects. They don't walk around, don't perform tasks, don't need pathfinding or behavior trees. They sleep in beds until a player takes over.

**Upgrade path to Agent Smithing:** When CIG eventually implements NPC crew, the Imprint Shell system evolves naturally. Instead of buying a blank organic clone and placing it in a bed, the ship has actual NPC crew members who walk around, perform tasks, and fill functional roles. A player transferring in takes over that NPC's body — full Agent Smithing. The Shell system becomes the stepping stone: ship it now with inert clone bodies, upgrade later to living NPCs. The underlying mechanic (consciousness transfer via Relay Beacon) stays the same. The only thing that changes is whether the body you're taking over was inert or active.

### Scoring Breakdown

| Axis | Score | Reasoning |
|------|-------|-----------|
| Physicalization | 5/5 | Shells are physical objects in beds. Your real body is physical at the terminal. Shell corpses persist with gear. Nothing vanishes, nothing phases, nothing pops in or out of existence. At every moment, every body and every item exists somewhere physical in the universe. |
| Persistence | 5/5 | Shells persist in beds when unoccupied. Real bodies persist at terminals. Shell corpses persist when vacated. Gear on corpses persists for the owner to recover. The coke-can rule is fully satisfied — drop a Shell in a bed on a random moon, come back a week later, it's still there. |
| Lore Compatibility | 5/5 | Every component is grounded in existing lore: FTL comms for transmission, cloning tech for the bodies, military need for the application. No new physics required — consciousness is information, and information can already travel faster than light in this universe. |
| Effectiveness | 5/5 | Near-instant grouping for ship crewing: owner pre-places Shells, crew transfers in from any port, wakes up, gears up, ready to go. Combined with Layer 1 (Commercial Flights / Bed Log Transit) for cross-system relocation, this covers every grouping scenario from "casual Tuesday night session" to "Saturday org fleet op." |
| Exploitability | 4/5 | Layered anti-abuse: expensive consumables, one-use, degradation timer, no gear transfers (structurally prevents item duplication), real body vulnerability, combat lockout, cooldown, Contractor Shell restrictions for instances. Minor deduction for edge cases CIG would tune during implementation (exact timer length, cooldown duration, Beacon range values). |
| Feasibility | 4/5 | No NPC AI required. Core mechanics (beds, components, consumables, terminals, party systems) all exist. Needs new items, a new component, transfer UI, and timer logic — real engineering work but nothing that depends on systems CIG has delayed. Clear upgrade path to Agent Smithing when NPC crew arrives. |
| Versatility | 5/5 | One mechanic — consciousness transfer into a pre-placed physical vessel — covers ship crewing, open world grouping, and instanced content. Layer 1 covers cross-system relocation. Together, every use case Thorston described ("fast travel to party leader, or party hangar") is addressed by a single unified system. |

### Why This Scores Higher Than Any Individual Idea

The top individual ideas each had one or two weak spots:

- **C.I.V. (31/35):** Cybernetic bodies clash with SC's organic aesthetic. Range limitation reduces effectiveness.
- **Agent Smithing (30/35):** Depends on NPC crew tech that's delayed past 1.0.
- **Commercial Flights (28/35):** Relocation only, not grouping. Low versatility.

The hybrid solves each of these:
- **Organic clone bodies** instead of cybernetic drones — fits SC's flesh-and-blood aesthetic.
- **No NPC dependency** — Shells are inert objects, shippable before 1.0, with a clean upgrade path to Agent Smithing.
- **Two-layer design** — Commercial Flights handle the long haul, Shells handle the last mile. Full coverage.

---

## Current Rankings

| Rank | Idea | Score | Best At |
|------|------|-------|---------|
| ★ | **Imprint Shell Network (Hybrid)** | **33/35** | **Full coverage: physicalization, persistence, lore, versatility, anti-duplication** |
| 2 | C.I.V. / I.R.C. | 31/35 | Physicalization, persistence, anti-exploitation |
| 3 | Agent Smithing | 30/35 | Versatility, effectiveness, leverages existing systems |
| 4 | Commercial Flights (Starliner) | 28/35 | Lore compatibility, physicalization, unexploitable |
| 4 | Bed Log Transit | 28/35 | Unexploitable, trivial to implement, lore-perfect |
| 6 | Transfer Transit | 27/35 | Built-in time limit, consequence mechanics |
| 6 | Crew Quarters Registry | 27/35 | Highest feasibility, gives crew quarters purpose |
| 8 | Rare Alien Structures | 25/35 | Physicalization purity, exploration content |
| 8 | Formalized Medbed Clone-In | 25/35 | Zero new engineering, formalizes existing behavior |
| 10 | Group Launch | 24/35 | Session-start grouping, unexploitable |
| 11 | Paid NPC Transport (Fade-to-Black) | 23/35 | Lore-friendly concept, economically balanced |
| 12 | Teleport to Docked Ship | 22/35 | Simplest implementation, strong problem statement |
| — | Fix the Friction First | N/A | Data shows ~96% of time lost is bugs/friction, not travel |

---

*This document is a living compilation. More ideas will be added as the community submits them. All ideas are scored against the same rubric for fair comparison.*

*The goal is to give CIG a quick-reference resource of community solutions that solve the grouping problem without breaking the persistent, physicalized universe.*
