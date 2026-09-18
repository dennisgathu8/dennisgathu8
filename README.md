Dennis Gathu | Football Data Engineer | CAF D
What I'm building
African football produces players the world covets.
It has never had the infrastructure to see itself clearly.
I'm building that infrastructure — open source, in Clojure, from Nairobi. The goal is a data foundation that clubs across the continent can own, inspect, and extend. Not licensed tools built for other contexts by people who have never watched football in Accra, Lagos, Nairobi, or Dar es Salaam.
🏗️ Clojure Sports Data Engineering Roadmap
Five projects. Each solves a real infrastructure gap that Python cannot address structurally.
#
Project
What it solves
Status
1
[pitch-pipe](https://github.com/dennisgathu8/pitch-pipe)
StatsBomb ingestion + transducer pipeline. Zero-copy transformation, spec validation at the boundary. Hardened with CI, dependency vulnerability scanning, and documented architecture decisions.
✅ Live
2
[temporal-squad](https://github.com/dennisgathu8/temporal-squad)
XTDB bi-temporal player state. Answers what your system knew at selection time — not just what it knows now.
✅ Live
3
[press-logic](https://github.com/dennisgathu8/press-logic)
Tactical pressing rules as EDN data. core.logic evaluation with fatigue-aware pressing via temporal-squad XTDB. First cross-project integration in the roadmap.
✅ Live
4
[formation-stream](https://github.com/dennisgathu8/formation-stream)
25Hz tracking data pipeline via core.async. Explicit backpressure monitoring. Compactness and pressing intensity metrics.
✅ Live
5
[dugout](https://github.com/dennisgathu8/dugout)
Full-stack analytics workbench. Clojure backend + ClojureScript frontend + shared .cljc logic across all four projects above.
✅ Live*
<sub>*dugout is feature-complete with a passing JVM + ClojureScript test suite; public fly.io demo deployment is in progress.</sub>
🌍 Beyond the Roadmap
Two more projects, built outside the five-project arc, that extend the same infrastructure to problems the roadmap didn't originally cover.
Project
What it solves
Status
[thorold](https://github.com/dennisgathu8/thorold)
The football entity register. Canonical reep_ IDs that map player, team, coach, competition, and season identities across Transfermarkt, FBref, UEFA, Sofascore, Opta, and 40+ other data providers — so every project in this portfolio can talk about the same player without an identity-matching problem.
✅ Live
[twenty-two_sixty-seven (break-window-response)](https://github.com/dennisgathu8/twenty-two_sixty-seven)
Decision support for FIFA World Cup 2026's mandatory hydration breaks (22' and 67'), expressed as auditable, inspectable rules on the same pitch-pipe → temporal-squad → press-logic → formation-stream stack. Server-rendered Clojure/XTDB, built to run and be defended on one box you own.
🚧 In progress
The infrastructure gap across African football
The problem is the same whether you are in the KPL, NPFL, CAF interclub, PSL, or the Ethiopian Premier League:
Decisions made on data that arrived after the fact
Pipelines that silently corrupt data for months before anyone notices
Models coaches cannot interrogate or challenge
Tools that live on one analyst's laptop and disappear when they leave
This is not a talent problem. It is a plumbing problem. And it is solvable.
Why Clojure for football analytics
Problem
Python
Clojure
Pipeline memory
Each Pandas step allocates a new DataFrame
Transducers compose into a single pass — zero intermediate collections
Data integrity
Silent NaN coercion on bad data
clojure.spec validates at the boundary — bad data throws before it touches the pipeline
Temporal queries
Postgres overwrites history
XTDB stores valid-time and transaction-time on every fact, automatically
Tactical rules
Neural net confidence scores coaches can't interrogate
core.logic encodes rules as readable data — auditable, modifiable without retraining
Full-stack
Python backend + JS frontend = two codebases
.cljc shared logic runs on JVM and in the browser — one codebase
Identity resolution
Fragile string/fuzzy matching per project
thorold's reep_ IDs give every project a single, stable identity layer
Background
1.5 years as BI Analyst at a capital group in Ethiopia managing data infrastructure across 8+ betting products
Built real-time fraud detection, Grafana dashboards, and reconciliation pipelines under production pressure
CAF D licenced football coach. My understanding of the game is not just from a data perspective.
Football is in the family — my father is a FIFA licensed agent and we run Infoot Technique, a scouting company in Kenya. Our work has produced players including Softi Ndirangu (Gor Mahia, AFC Leopards) and Peter Thiongo who captained AFC Leopards
Self-taught. Nairobi. Building in public.
Stack
Primary: Clojure · ClojureScript · XTDB · core.async · core.logic Data: StatsBomb · SQL · DuckDB · clojure.spec BI & Viz: Grafana · Streamlit · Matplotlib Infra: GitHub Actions · Fly.io · Leiningen · Shadow-cljs
🌍 Open to
Football analytics roles across Africa and globally
Clubs in CAF competitions serious about data infrastructure
Federations building analytics capacity from the ground up
Academies tracking player development over time
Any league — KPL, NPFL, PSL, EPL, wherever the problem is real and the will to solve it exists
Freelance data infrastructure contracts
Open source collaborators who care about African football
📧 dennisgathu8@gmail.com
"Data isn't just numbers; it's the 12th player on the pitch." — Dennis Gathu
