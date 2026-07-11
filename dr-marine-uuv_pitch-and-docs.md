# Dr.Marine UUV

*An affordable drone system that watches over Zanzibar's reefs and seaweed farms — so the people who depend on them can act before the ocean turns.*

---

## The pitch

Along the coast of Zanzibar, roughly 25,000 people farm seaweed. More than eight in ten are women, and for many it is the most reliable independent income they have. It is now the third-largest source of income on the islands. That livelihood sits on top of a warming, changing ocean — and the same warm, still, low-salinity conditions that stress coral reefs also trigger *ice-ice*, the disease that whitens and breaks seaweed crops. In the dry season, ice-ice has reached nearly every plant in a farm.

Today, a farmer finds out something is wrong when the crop is already lost. A conservation team learns a reef bleached after it has bleached. The information arrives too late to act on.

Dr.Marine UUV is a small, low-cost pair of drones that closes that gap. A surface vehicle maps the whole zone from above — temperature, farm layout, reef outline. Then the system does something a satellite or a boat survey cannot: it adds a dimension. An underwater vehicle descends through the water column and inspects the reef and the farm up close, colony by colony, line by line. The two feeds combine into one picture, and that picture turns into plain-language advice: *move these lines north for better flow; harvest early here; this reef is under heat stress.*

It is built for the place it serves — runs on solar, works offline from a phone, repairable with local parts, labelled in Swahili as well as English. Not a vendor-locked box, but a tool a community can own.

**What we are showing you** is a working interactive simulation of that system. Every number in it is generated for demonstration and clearly marked *SIMULATION*. It is an honest preview of the concept, not a deployed product — and it exists so you can see, in ninety seconds, exactly what the real thing would do.

**What we are asking for** is support to move from this convincing demonstration to a first field-tested prototype.

---

## How it works — in plain words

Think of two robots working as a team.

The **surface robot** is like a small self-driving boat. It travels back and forth over the area in neat rows, the way you'd mow a lawn, measuring the sea surface and drawing a map: where the farm lines are, where the reef sits, where the water is unusually warm.

The **underwater robot** is the part that makes this different. Once the surface map shows where to look, it dives — down through the water, past the seaweed lines, to the reef and seagrass on the bottom. It carries a light and a camera and sensors, and it checks the health of things close-up: is this coral pale, is this seaweed line fouled, is the water down here short of oxygen.

Everything the two robots see is pulled together into one view and translated into advice a farmer or an officer can act on the same day. No marine-science degree required — the system says what it found and what to do about it.

---

## How it works — technical documentation

### System concept

A hybrid two-vehicle fleet feeding a single mission-control interface:

- **USV (uncrewed surface vehicle)** — broad-area mapping via a lawnmower survey pattern: sea-surface temperature, farm-line layout, reef and seagrass outlines, boat traffic, early warm-anomaly flags.
- **UUV (uncrewed underwater vehicle)** — depth-controlled water-column profiling and close-range inspection: per-colony coral health, per-line seaweed/frond condition, near-seabed water quality.

The interface serves three simplified dashboards off the same mission data — seaweed farmer, conservation team, fisheries officer — each asking a different question of one shared dataset.

### The demonstration build

The artifact under review is a single self-contained HTML file. It runs offline in any modern browser, with the 3D library vendored inline (no network calls). It has no backend and uses no browser storage.

- **SimEngine** — a fixed-timestep tick loop driven by a seeded random-number generator, so a recording is reproducible, with a live jitter layer so values visibly move.
- **State store** — vehicles, sensors, and derived risk scores in one object.
- **Renderers** — a 2D vector map (canvas), a 3D underwater scene (WebGL / Three.js), a telemetry HUD, and a recommendations layer.
- **DemoDirector** — a six-step state machine that scripts the ~90-second auto-play sequence with captions and a simulated cursor, then loops. The interface can also be driven manually.

### Simulated variables and thresholds

All values are generated client-side within plausible tropical-lagoon ranges. Two risk mechanics are anchored to published science:

- **Coral bleaching** — a compressed Degree Heating Week (DHW) accumulator, following NOAA Coral Reef Watch: risk at **4 °C-weeks**, likely bleaching with mortality at **8**, multi-species mortality at **12**. The on-screen gauge is labelled *illustrative* because real DHW accumulates over a 12-week window, not 90 seconds.
- **Ice-ice risk** — a score that rises with warm temperature, low salinity, and low circulation. The ~99 % dry-season prevalence figure for Zanzibar is well-documented; the clean causal link between any single variable and disease is not, so the demo presents these conditions as *associated with* outbreaks, not as proven cause, and the gauge is labelled *illustrative*.

Regional salinity (~34 ‰) is confirmed and matches the sim; the DO and turbidity ranges are plausible placeholders, not measured local data.

### Deployment concept (indicative, not costed)

- **USV** — small catamaran or kayak hull, brushless drive, solar + LiFePO4, open-source autopilot, GPS, phone/LoRa telemetry.
- **UUV** — open-frame or tethered mini-ROV as the affordable entry point; a tether avoids costly acoustic comms and eases recovery in shallow reef and farm work.
- **Shared sensors** — temperature/conductivity (salinity), pH, optical dissolved oxygen, optical turbidity, action-cam for photogrammetry, single-beam echo sounder for bathymetry.
- **Tropical hardening** — anti-biofouling on optical windows, UV-stable enclosures, sacrificial anodes, conformal-coated electronics, field-swappable modules.

Costs and specific models are not yet sourced and are out of scope until a real bill of materials exists.

---

## Ethics and honesty

We would rather under-claim than mislead, so the boundaries are stated plainly.

**This is a simulation.** Nothing in the demonstration talks to a real sensor, drone, or satellite. Every reading is generated for illustration and marked *SIMULATION* on screen. We show the concept convincingly; we do not pretend it is deployed.

**Claims are checked, and the uncertain ones are labelled.** The bleaching thresholds and the Zanzibar ice-ice prevalence are anchored to published sources. Where the science is more nuanced — such as how cleanly temperature or salinity predicts disease in the field — we say "associated with," not "caused by," and mark the relevant gauges illustrative. We do not present placeholder ranges as measured local data, and we do not quote hardware costs we have not sourced. One earlier claim — that dynamite fishing is an active threat on this coast — we corrected: Tanzania declared blast fishing eradicated in 2025, so we frame it as a recovery, not an ongoing crisis.

**It is built to be owned, not rented.** Solar power, offline operation, Swahili labelling, off-the-shelf and 3D-printable parts, and community-repairable design are deliberate. A monitoring tool that a community cannot afford, understand, or fix is not a solution for that community.

**The people come first.** The system's purpose is to give the farmers — most of them women — and the conservation and fisheries teams earlier, clearer information about their own waters. It is designed to inform their decisions, not to replace their judgement or surveil their work.

---

*Companion files: the interactive demonstration (`dr-marine-uuv.html`), the claims fact-check (`dr-marine-uvv_factcheck.md`), and the updated claims register (`concept-doc_section9_updated.md`).*
