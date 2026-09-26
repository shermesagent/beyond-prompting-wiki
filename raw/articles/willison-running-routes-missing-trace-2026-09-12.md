---
source_url: https://simonwillison.net/2026/Sep/12/astra-running-routes/
ingested: 2026-09-26
sha256: 824857f8483838e3226da59edd9549e315d430bca2c93434fa183e23ee7aba59
---
# Source notes — Generating running routes with GPT-6 Astra and ChatGPT Work

Simon Willison, personal blog, published September 12, 2026; first-person account read September 26. A single demonstration, not a benchmark.

## Source-grounded account
Willison describes an agent spending 27 minutes generating 5K and 10K running loops from OpenStreetMap data, returning a visualization and downloadable GPX and GeoJSON files. When asked, the agent said it used Nominatim and Overpass, but the interface did not expose the actual code or exact intermediate steps; after conversation compaction, it could not provide that code. Willison calls missing trace access an anti-feature and argues that systems should preserve pre-compaction work for later review. A plausible final artifact and an agent's description of its process are not equivalent to a reproducible trace.

## Practice translation (curator interpretation)
For one low-stakes agent task, request the final file plus the inputs, tool steps, and checks performed. Open the file in the native application and see whether someone else could reconstruct the path from source to output. If not, reduce the next delegation's scope or choose an interface that preserves the trace.
