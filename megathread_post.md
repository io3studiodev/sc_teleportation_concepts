# "Teleportation" Ideas Megathread

This thread is a collection of ideas/concepts to help CIG make the best game possible. Gathered directly from spectrum community posts, curated by me, organized by AI.

Thorston said "it's not signed off yet", and Jared reiterated "it's not a signed off feature... we have to explore those things, even if we never do it...", meaning they've still not finalized the concept/design behind teleportation/fast travel or even if it will be done.

This means we have a small window of time to come up with the best ideas for them so this can be done the right way, or not at all. The challenge is solving it without gutting the thing that makes Star Citizen Star Citizen.

Please post your best ideas below or write out an entire thread and post the link here, or argue against it. I'll just have AI summarize your idea into bullet points with a link to the original.

Keep in mind, Thorston said "fast travel to party leader, or party hangar". So our ideas have to solve several scenarios like "fast travelling/teleporting/agent smithing" to someone's ship, to party leader, or leaders hangar. And finally to instanced content entrances like the municipal works or Siege of Orison.

If they're going to implement it, let's at least try to help them out with the best ideas we can come up with. I've only got so much time in the day so this will only be updated once or twice per day.

📄 **[Full detailed analysis with scoring breakdowns, anti-exploitation mechanics, and edge case discussion →](https://github.com/io3studiodev/sc_teleportation_concepts/blob/main/fast_travel_megathread.md)**

---

## A Critical Data Point Before We Start

Community analysis shows that **actual travel time accounts for roughly 4% of total time lost** when grouping up. The other 96% is bugs and friction — loading ships with vehicles (30 min), server switching (15 min), ASOP bugs (10 min), broken jump points (10 min). We may be asking for teleportation to skip bugs, not travel. ([Source](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/the-teleport-debate))

---

## Scoring

Every idea is scored 1-5 across seven criteria: Physicalization, Persistence, Lore Compatibility, Effectiveness, Exploitability Resistance, Feasibility, and Versatility (does one system cover ship crewing, open world grouping, AND instanced content?). Full rubric in the detailed doc. A score of 1 on Physicalization or Persistence is effectively disqualifying — the community funded a physicalized, persistent universe.

---

## #1 — C.I.V. / I.R.C. (Cybernetic Imprint Vehicle) — 31/35

**[Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/an-alternative-to-instant-pc-travel-teleportation-)**

Your consciousness links into a cybernetic drone body (CIV) stored as physical cargo aboard the destination ship. Requires an Imprint Relay Core (IRC) ship component to operate. CIVs are inert without a player — no NPC AI needed. Destroying the IRC kills all linked CIVs instantly, creating tactical counterplay.

**Why it scores high:** Perfect physicalization and persistence — everything is a real, destructible object. Strongest anti-exploit design (expensive hardware, limited count, range caps, IRC as a high-value target). Zero dependency on NPC crew tech, so it's buildable before 1.0.

**Trade-off:** Range-limited by design. Cybernetic bodies may clash with SC's organic aesthetic.

---

## #2 — Agent Smithing — 30/35

**Concept from ~2015 community discussions**

Take over an existing NPC crew member's body on a friend's ship. Your consciousness moves — your original body stays behind asleep. You wake up in the NPC's uniform, gear up from the ship's armory. For instanced content, smith into hireable guard NPCs at the mission entrance. Crew hire tokens (purchased at ports, consumed on use) limit the number of smith-ins. No gear transfers in either direction — the NPC body drops with its gear when you smith out.

**Why it scores high:** Nothing teleports — the body was already there. Covers all three use cases (ship crewing, open world, instanced) with one mechanic. Every anti-exploit safeguard maps to systems that already exist in-game.

**Trade-off:** Depends on NPC crew tech (delayed past 1.0), though the "sleeping body in a bed" version is far simpler than full AI crew.

---

## #3 (tie) — Commercial Flights (Genesis Starliner) — 28/35

**[Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/fast-travel-done-right)** | Also supported by: [Why not use what's already there?](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/fast-travel-why-not-use-whats-already-there) | [YES! To Teleporting](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/yes-to-teleporting-in-star-citizen)

Buy a ticket at a spaceport kiosk, board a real Genesis Starliner, ride it to another major spaceport. The ship physically exists — food shops, seating, windows. Travels on rails at 2x+ QT speed, departs on a schedule. Lawless systems get rep-gated gang shuttles. No loading screens. Landing zones already have "Commercial Flights" areas built.

**Why it scores well:** Perfect physicalization (5/5) and highest lore compatibility (5/5). Near-impossible to exploit. Almost no new tech needed.

**Trade-off:** Relocation system, not a grouping system (Versatility: 2/5). Gets you to the same spaceport, not onto a friend's ship. Pairs naturally with Agent Smithing or CIV for the last mile.

---

## #3 (tie) — Bed Log Transit (Offline Commercial Travel) — 28/35

**[Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-why-it-doesn-t-make-sense-now-but-coul)** (extracted from point 4)

Go to a transit hub with beds, log out (minimum 30 min before your planned session, or days in advance). Next time you log in: "You slept through your commercial flight." Pick your destination. You scheduled travel while offline — your character rode a transport while you were cooking eggs.

**Why it scores well:** Virtually unexploitable (5/5) — can't abuse something that requires being logged out 30+ minutes. Trivial to implement (5/5). Perfect lore fit (5/5) — sleeper cabins on commercial flights.

**Trade-off:** Only solves pre-planned relocation (Effectiveness: 3/5). Great for "our org event is Friday," useless for "my friend just logged in."

---

## #5 (tie) — Transfer Transit (Temporary Clone) — 27/35

**[Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/maybe-transfer-transit-is-the-way)**

Inspired by Dark Matter. Enter a pod, consciousness transmits into a temporary clone at the destination. Clone has a built-in lifespan timer. When it expires or dies, memories sync back to your original body. If the clone dies before syncing, those memories are lost.

**Why it scores well:** The ticking clock is an elegant natural guardrail. You're always anchored to your real location. Memory loss on death adds meaningful consequence.

**Trade-off:** Generating a clone body from nothing is hard to justify in a physicalized universe. The poster acknowledged the lore would be "insanely hard."

---

## #5 (tie) — Crew Quarters Registry ("Agent Smithing Lite") — 27/35

**[Original Post](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/crew-quarters-an-alternative-to-teleportation)**

Pre-register to a bed on a friend's ship. When the captain issues "call to arms," you wake up aboard in your underwear. Gear up from pre-stocked suit lockers. Return to your last location via the bed when done. Cooldown timer prevents flip-flopping.

**Why it scores well:** Highest feasibility (5/5) — no NPC tech needed, every component exists today. Gives crew quarters, suit lockers, and armor racks actual gameplay purpose. Could ship before 1.0. Could evolve into full Agent Smithing once NPC crew tech exists.

**Trade-off:** Your body does teleport (Physicalization: 3/5, Persistence: 3/5). Pragmatic compromise.

---

## Also Documented

**Rare Alien Structures (25/35)** — ([Source](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-why-it-doesn-t-make-sense-now-but-coul)) Ancient alien bridges at the edges of space. Perfect physicalization, but barely solves grouping — endgame exploration content.

**Formalized Medbed Clone-In (25/35)** — ([Source](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-already-exist-and-how-to-implement-it)) Formalize what players already do: deliberately clone to a party member's medbed. Everything exists already. Tension: once DOAS is live, each use costs a clone life — the system works against its own use case as death penalties increase.

**Group Launch (24/35)** — ([Source](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/not-teleport-fast-travel-but-group-launch)) Spawn at party leader's station when logging in after 1+ hour offline. Pay QT fuel cost. UEE space only. Unexploitable but session-start only.

**Paid NPC Transport (23/35)** — ([Source](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-fast-travel-would-be-great-for-star-ci)) Fade-to-black shuttle. Good concept, weak implementation. See Commercial Flights for the physicalized version.

**Teleport to Docked Ship (22/35)** — ([Source](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-fast-travel-would-be-great-for-star-ci)) Strongest business case ("I log into something else instead") but still teleportation. "Docked only" limits when, not what.

---

## Fix the Friction First (Before Any Fast Travel)

**Sources:** [Before we try teleportation](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/before-we-try-teleportation) | [The teleport debate](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/the-teleport-debate) | [A calendar is the answer](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-is-not-the-answer-a-calender-is) | [Group bed log should be priority](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-is-stupid-group-bed-log-should-be-prio)

Data shows ~96% of lost time is bugs and friction, not travel. Fix the top issues first (vehicle loading, server switching, ASOP, jump points). Add an in-game calendar/event planner. Fix group bed logging so crews can spawn together on the same ship next session. Add autopilot for AFK quantum travel. These are necessary regardless of which fast travel solution is chosen.

---

## Community Counterarguments Against Fast Travel

Not every response needs to be a solution. These posts articulate *why* the community cares so deeply:

- **["Without time, distance doesn't matter"](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/without-time-distance-doesn-t-matter)** — Travel time is a strategic resource. Logistics, troop movement, calling the banners — all evaporate with teleportation.
- **["Teleporting doesn't make sense"](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-why-it-doesn-t-make-sense-now-but-coul)** — Most comprehensive opposition post. Fast travel becomes mandatory once it exists. Breaks the economy (regional scarcity, hauling, support roles). Cites New World and EVE Online as cautionary tales.
- **["Teleporting is poorly conceived"](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/teleporting-is-poorly-conceived-or-at-best-kind-of)** — Stress-tests teleportation with abuse scenarios. Endorses Agent Smithing. Raises NPC Crew Tinfoil Theory: if CIG is considering teleportation instead of Agent Smithing, NPC crew may never happen.
- **["Please don't" / "Instant travel no"](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/please-please-cig-don-t-implement-fast-travel-tele)** — ([also](https://robertsspaceindustries.com/spectrum/community/SC/forum/3/thread/instant-travel-please-no)) Get social tools in first. The universe already feels too small. This game requires planning — that's a feature, not a bug.

---

## Key Insight: These Ideas Aren't Mutually Exclusive

The strongest possible system might be a **layered approach**: Commercial Flights or Bed Log Transit for cross-system relocation (the "long haul") + Agent Smithing or CIV for ship crewing and instanced content (the "last mile") + Fix the Friction First as the foundation underneath everything. No single idea scored perfectly across all axes — but combining complementary strengths covers every use case.

---

*This is a living thread. More ideas will be added as they come in. All scored against the same rubric for fair comparison. If you have an idea, post it and link it here.*

*Full detailed analysis: **[Read the full document →](LINK_TO_GITHUB_FULL_DOC)***
