# Dennis Gathu | Football Data Engineer

[![X](https://img.shields.io/badge/X-@Zigzagzila-000000?style=flat&logo=x)](https://x.com/zi6za6zi6la)
[![Location](https://img.shields.io/badge/Based_in-Nairobi,_Kenya-006400?style=flat)]()
[![Focus](https://img.shields.io/badge/Focus-African_Football_Infrastructure-FF6B00?style=flat)]()

---

## What I'm building

African football produces players the world covets.

It has never had the infrastructure to see itself clearly.

I'm building that infrastructure — open source, in Clojure,
from Nairobi. The goal is a data foundation that clubs
across the continent can own, inspect, and extend.
Not licensed tools built for other contexts by people
who have never watched football in Accra, Lagos,
Nairobi, or Dar es Salaam.

---

## 🏗️ Clojure Sports Data Engineering Roadmap

Five projects. Each solves a real infrastructure gap
that Python cannot address structurally.

| # | Project | What it solves | Status |
|---|---------|---------------|--------|
| 1 | [pitch-pipe](https://github.com/dennisgathu8/pitch-pipe) | StatsBomb ingestion + transducer pipeline. Zero-copy transformation, spec validation at the boundary. | ✅ Live |
| 2 | [temporal-squad](https://github.com/dennisgathu8/temporal-squad) | XTDB bi-temporal player state. Answers what your system knew at selection time — not just what it knows now. | ✅ Live |
| 3 | press-logic | Tactical rules as data via core.logic. Rules coaches can read, challenge, and modify — not opaque model weights. | 🔨 Building |
| 4 | formation-stream | 25Hz tracking data via core.async. Backpressure handling, real-time compactness metrics. | 📋 Planned |
| 5 | dugout | Full-stack analytics workbench. Clojure backend + ClojureScript frontend + shared .cljc logic. | 📋 Planned |

---

## The infrastructure gap across African football

The problem is the same whether you are in the KPL,
NPFL, CAF interclub, PSL, or the Ethiopian Premier League:

- Decisions made on data that arrived after the fact
- Pipelines that silently corrupt data for months
  before anyone notices
- Models coaches cannot interrogate or challenge
- Tools that live on one analyst's laptop and disappear
  when they leave

This is not a talent problem. It is a plumbing problem.
And it is solvable.

---

## Why Clojure for football analytics

| Problem | Python | Clojure |
|---------|--------|---------|
| Pipeline memory | Each Pandas step allocates a new DataFrame | Transducers compose into a single pass — zero intermediate collections |
| Data integrity | Silent NaN coercion on bad data | clojure.spec validates at the boundary — bad data throws before it touches the pipeline |
| Temporal queries | Postgres overwrites history | XTDB stores valid-time and transaction-time on every fact, automatically |
| Tactical rules | Neural net confidence scores coaches can't interrogate | core.logic encodes rules as readable data — auditable, modifiable without retraining |
| Full-stack | Python backend + JS frontend = two codebases | .cljc shared logic runs on JVM and in the browser — one codebase |

---

## Background

- **1.5 years** as BI Analyst at a capital group in Ethiopia
  managing data infrastructure across 8+ betting products
- Built real-time fraud detection, Grafana dashboards,
  and reconciliation pipelines under production pressure
- Football is in the family — my father was a professional
  player and development coach
- Self-taught. Nairobi. Building in public.

---

## Stack

**Primary:** Clojure · ClojureScript · XTDB · core.async · core.logic
**Data:** StatsBomb · SQL · DuckDB · clojure.spec
**BI & Viz:** Grafana · Streamlit · Matplotlib
**Infra:** GitHub Actions · Fly.io · Leiningen · Shadow-cljs

---

## 🌍 Open to

- Football analytics roles across Africa and globally
- Clubs in CAF competitions serious about data infrastructure
- Federations building analytics capacity from the ground up
- Academies tracking player development over time
- Any league — KPL, NPFL, PSL, EPL, wherever the
  problem is real and the will to solve it exists
- Freelance data infrastructure contracts
- Open source collaborators who care about African football

📧 dennisgathu8@gmail.com

---

> *"Data isn't just numbers; it's the 12th player
> on the pitch."*
> — Dennis Gathu
