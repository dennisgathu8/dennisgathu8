# Dennis Gathu — Football Data Engineer

[![X](https://img.shields.io/badge/X-@Zigzagzila-000000?style=flat&logo=x)](https://x.com/zi6za6zi6la) [![Location](https://img.shields.io/badge/Based_in-Nairobi,_Kenya-006400?style=flat)](https://github.com/dennisgathu8) [![Focus](https://img.shields.io/badge/Focus-African_Football_Infrastructure-FF6B00?style=flat)](https://github.com/dennisgathu8)

I build open source data infrastructure for African football, in Clojure, from Nairobi — the kind a club owns and runs itself, not a SaaS subscription. A technical director should be able to see, before the team sheet is submitted, which players came back from international duty still fatigued. That's the class of problem this solves: not a talent gap, a plumbing one. CAF D licenced coach; my father is a FIFA agent and we run a scouting company in Kenya that's produced players like Softi Ndirangu (Gor Mahia, AFC Leopards) and Peter Thiongo (AFC Leopards captain) — so the football side of this isn't secondhand.

---

## Projects

| Project | What it does | Category | Status |
| --- | --- | --- | --- |
| [pitch-pipe](https://github.com/dennisgathu8/pitch-pipe) | StatsBomb ingestion + transducer pipeline. Spec-validated at the boundary. | Core | ✅ Live |
| [temporal-squad](https://github.com/dennisgathu8/temporal-squad) | Bi-temporal player state (XTDB) — what the system knew at selection time, not just now. | Core | ✅ Live |
| [press-logic](https://github.com/dennisgathu8/press-logic) | Tactical pressing rules as auditable EDN data, fatigue-aware via temporal-squad. | Core | ✅ Live |
| [formation-stream](https://github.com/dennisgathu8/formation-stream) | 25Hz tracking pipeline via core.async, explicit backpressure. | Core | ✅ Live |
| [dugout](https://github.com/dennisgathu8/dugout) | Full-stack analytics workbench unifying all four projects above via shared `.cljc` logic. | Core | ✅ Live¹ |
| [thorold](https://github.com/dennisgathu8/thorold) | Canonical entity register — one `reep_` ID per player/team/coach, mapped across 40+ data providers. | Extended | ✅ Live |
| [twenty-two_sixty-seven](https://github.com/dennisgathu8/twenty-two_sixty-seven) | Decision support for World Cup 2026 hydration breaks, same stack lineage. | Extended | 🚧 In progress |

<sub>¹ Feature-complete with a passing JVM + ClojureScript test suite; public fly.io demo deployment in progress.</sub>

---

## Background

- 1.5 years as a BI Analyst managing data infrastructure across 8+ betting products in Ethiopia — real-time fraud detection, Grafana dashboards, production reconciliation pipelines under load.
- CAF D licenced coach — this isn't data built at a distance from the game.
- Self-taught, Nairobi. Everything above is built and documented in public.

## Stack

Clojure · ClojureScript · XTDB · core.async · core.logic · clojure.spec · Grafana · Fly.io · GitHub Actions

## Open to

- Clubs and federations across CAF competitions ready to own their data infrastructure instead of renting it
- Data infrastructure roles, freelance contracts, and open source collaborators who care about African football

📧 dennisgathu8@gmail.com

---

> *"Data isn't just numbers; it's the 12th player on the pitch."* — Dennis Gathu