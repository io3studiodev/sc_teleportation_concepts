# "Teleportation" Ideas Megathread — Help Me Build the Best Possible Submission for CIG

Thorston said "it's not signed off yet." Jared reiterated "it's not a signed off feature... we have to explore those things, even if we never do it." That means we have a small window to get this right.

Over the last 48 hours, this community has generated dozens of threads with ideas, counterarguments, and heated debate about fast travel. Instead of letting all of that scatter across Spectrum, I've been curating the strongest proposals, scoring them against SC's own design pillars, and synthesizing what I think might be the strongest possible solution.

**Full transparency:** I used AI (Claude) to help analyze, score, and synthesize these ideas. It's never played Star Citizen. That's exactly why I'm posting this here first — **this needs to be stress-tested by people who actually play the game** before I submit a final version to CIG's Ideas section.

**Here's what I need from you:**
- Did I miss an idea? Post it or link it and I'll score it and add it.
- Did I score something wrong? Tell me why — I'll adjust.
- Can you break the proposed hybrid solution? Find an exploit I missed? Please try.
- Do you have a better idea entirely? Post it.
- Do you think this whole effort is misguided? Tell me that too. The counterarguments section exists for a reason.

Keep in mind, Thorston said "fast travel to party leader, or party hangar." So ideas have to solve several scenarios: getting to someone's ship, to party leader, to a leader's hangar, and to instanced content entrances like Municipal Works or Siege of Orison.

**Once this has been pressure-tested by the community, I'll synthesize all feedback into a final document and post it in the Ideas section as a formal submission to CIG — complete with an AI-ready handoff doc their design team can use for implementation planning.**

I've only got so much time in the day so this will only be updated once or twice per day.

📄 **[Full detailed analysis with scoring breakdowns, anti-exploitation mechanics, and edge case discussion →](https://github.com/io3studiodev/sc_teleportation_concepts/blob/main/fast_travel_megathread.md)**

---

## A Critical Data Point Before We Start

Community analysis shows that **actual travel time accounts for roughly 4% of total time lost** when grouping up. The other 96% is bugs and friction — loading ships with vehicles (30 min), server switching (15 min), ASOP bugs (10 min), broken jump points (10 min). We may be asking for teleportation to skip bugs, not travel. ([Source](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/the-teleport-debate))

---

## Scoring

Every idea is scored 1-5 across seven criteria: Physicalization, Persistence, Lore Compatibility, Effectiveness, Exploitability Resistance, Feasibility, and Versatility (does one system cover ship crewing, open world grouping, AND instanced content?). Full rubric in the detailed doc. A score of 1 on Physicalization or Persistence is effectively disqualifying — we funded a physicalized, persistent universe.

---

## The Synthesized Hybrid: Imprint Shell Network — 33/35

After analyzing all 11 community ideas, I had the AI synthesize a hybrid pulling the strongest elements from the top proposals. **This is the thing I most want you to stress-test.** Can you break it? Is there an exploit? Does it violate a design pillar I'm not seeing?

### Layer 1 — Long Haul (Cross-System Relocation)

**Physicalized Commercial Flights:** Board a real Genesis Starliner at a spaceport, ride it to your destination. Scheduled departures, accelerated QT, no loading screens. For real-time relocation during a session.

**Bed Log Transit:** For repositioning between sessions. Walk to a transit hub, select your destination, lie down, log out. A real-world countdown starts (travel time = ~0.75x manual QT time, 30-minute minimum). Your body is physically aboard a transport — asleep in a sleeper cabin. When you log back in after the timer completes: "You slept through your commercial flight." If you log in early, you can wait or cancel and wake up where you started. Routes only serve major spaceports along commercial lanes.

### Layer 2 — Last Mile (Ship Crewing, Grouping, Instanced Content)

**Imprint Shells.** Purpose-grown organic clone bodies, purchased at ports as physical consumables (torpedo-priced), transported to a ship, and placed in crew quarter beds. Ship needs a Relay Beacon component installed. Your consciousness transfers via FTL comms (Dr. Betel's breakthrough) into the Shell from any Imprint Terminal at a port. You wake up in a medical gown — no gear, no items, nothing transfers in either direction. Your real body stays in stasis at the terminal, physical and vulnerable. You gear up from the ship's armory. When done or the Shell's biological degradation timer expires (4-8 hours), consciousness snaps back, Shell dies, leaves a corpse with its gear for the owner to recover.

**Item duplication is structurally impossible** — consciousness crosses the transfer boundary, matter never does, period.

**For instanced content:** Contractor Shells at mission entrances. Can't pick up loot, can't carry anything out, despawn on mission complete.

**Anti-exploitation:** Expensive one-use consumables, Relay Beacon with capacity/range limits, degradation timer, combat lockout (can't transfer into a ship under fire), cooldown between transfers, real body vulnerability at terminal, Contractor Shell loot restrictions.

**Upgrade path:** When NPC crew arrives, Shells evolve into Agent Smithing. The inert clone becomes a living NPC you take over. Same mechanic, better body. CIG doesn't build two systems.

**Full detailed breakdown with lore justification, anti-exploit mechanics, and edge cases in the [complete document](https://github.com/io3studiodev/sc_teleportation_concepts/blob/main/fast_travel_megathread.md).**

---

## Community Ideas Ranked (11 Proposals Evaluated)

**★ Imprint Shell Network — 33/35** (Synthesized) — Full coverage, anti-duplication, upgrade path

**#2 — C.I.V. / I.R.C. — 31/35** ([Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/an-alternative-to-instant-pc-travel-teleportation-)) — Physicalization, persistence, anti-exploitation

**#3 — Agent Smithing — 30/35** (~2015 concept) — Versatility, effectiveness, existing systems

**#4 — Commercial Flights — 28/35** ([Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/fast-travel-done-right)) — Lore compatibility, physicalization

**#4 — Bed Log Transit — 28/35** ([Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-why-it-doesn-t-make-sense-now-but-coul)) — Unexploitable, trivial to implement

**#6 — Transfer Transit — 27/35** ([Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/maybe-transfer-transit-is-the-way)) — Built-in time limit, consequences

**#6 — Crew Quarters Registry — 27/35** ([Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/crew-quarters-an-alternative-to-teleportation)) — Highest feasibility, crew quarter purpose

**#8 — Rare Alien Structures — 25/35** ([Source](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-why-it-doesn-t-make-sense-now-but-coul)) — Endgame exploration content

**#8 — Medbed Clone-In — 25/35** ([Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-already-exist-and-how-to-implement-it)) — Formalizes existing behavior

**#10 — Group Launch — 24/35** ([Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/not-teleport-fast-travel-but-group-launch)) — Session-start grouping

**#11 — NPC Transport (Fade) — 23/35** ([Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-fast-travel-would-be-great-for-star-ci)) — Lore-friendly concept

**#12 — Teleport to Docked Ship — 22/35** ([Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-fast-travel-would-be-great-for-star-ci)) — Simplest implementation

---

## Fix the Friction First (Regardless of Fast Travel Decision)

**Sources:** [Before we try teleportation](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/before-we-try-teleportation) | [The teleport debate](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/the-teleport-debate) | [A calendar is the answer](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-is-not-the-answer-a-calender-is) | [Group bed log priority](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-is-stupid-group-bed-log-should-be-prio)

Data shows ~96% of lost time is bugs and friction, not travel. Fix the top issues first (vehicle loading, server switching, ASOP, jump points). Fix group bed logging so crews spawn together next session. Add an in-game calendar/event planner. Consider autopilot for AFK quantum travel. These are necessary regardless of which fast travel solution is chosen.

---

## Community Counterarguments Against Fast Travel

These posts aren't just opposition — they're substantive design arguments that shaped the scoring rubric:

- **["Without time, distance doesn't matter"](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/without-time-distance-doesn-t-matter)** — Travel time is a strategic resource. Logistics, troop movement, calling the banners — all evaporate with teleportation.
- **["Teleporting doesn't make sense"](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-why-it-doesn-t-make-sense-now-but-coul)** — Most comprehensive opposition post. Fast travel becomes mandatory once it exists. Breaks the economy (regional scarcity, hauling, support roles). Cites New World and EVE Online as cautionary tales.
- **["Teleporting is poorly conceived"](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-is-poorly-conceived-or-at-best-kind-of)** — Stress-tests teleportation with abuse scenarios. Endorses Agent Smithing. Raises NPC Crew Tinfoil Theory: if CIG is considering teleportation instead of Agent Smithing, does that mean NPC crew isn't coming?
- **["Please don't"](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/please-please-cig-don-t-implement-fast-travel-tele)** / **["Instant travel no"](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/instant-travel-please-no)** — Get social tools in first. The universe already feels too small. This game requires planning — that's a feature, not a bug.

---

## What Happens Next

This thread stays open for community feedback. I'll add new ideas, adjust scores if someone makes a compelling argument, and incorporate exploit vectors I missed. Once it's been properly pressure-tested, I'll compile the final version and post it in **CIG's Ideas section** as a formal submission — with a structured handoff document their design team can feed directly into AI tools for implementation planning.

We built this in 48 hours. Let's make sure it's bulletproof before we hand it over.

---

*All community contributors credited via links to original posts. If your idea is missing, post it or link it here.*
