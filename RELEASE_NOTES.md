## Aviation API endpoints, snapshot 15 Nov 2026

- 25,002 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 2,574 services · 248 country codes · 23,300 keyless JSON rows

### Download

- `Aviation_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 25,002 rows, 886.6 kB gzipped (6.6 MB as CSV), SHA-256 `f294315212af4cb01b42bd1c531ec2c632a1f9644234266e5119dbd809496255`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Aviation_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Aviation_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 10,551 · Wrap the METAR and TAF URL patterns as a get_airport_weather tool: pass an ICAO code, return wind, visibility, cloud and the forecast periods with the report time; add a timeout.
- 📱 App features: 6,417 · Show airports, runways, controlled airspace, drone no-fly zones and noise contours near a place on a map card.
- 🧠 Grounding and data pipelines: 1,725 · Load airport lists, passenger and freight counts, flight movements and airport weather series on a schedule into your own store, so answers about an airport cite a dated source.
- 🧪 Evals and testing: 25,002 · Run your flight tool against a fixed set of URLs across formats; check that ICAO codes, report times, wind and visibility, positions and altitudes parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release
- Left out: 160 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 34 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 68 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 2 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Overlap: 10,061 of these URLs are also in 190k-weather-apis-for-agents.
- Overlap: 1,183 of these URLs are also in 270k-transit-apis-for-agents.
- Overlap: 254 of these URLs are also in 270k-water-apis-for-agents.
- Overlap: 22 of these URLs are also in 130k-finance-economy-apis-for-agents.
- Overlap: 319 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 31 of these URLs are also in 86k-oceans-apis-for-agents.
- Overlap: 14 of these URLs are also in 20k-air-quality-apis-for-agents.
- Overlap: 23,300 of these URLs are also in 2.5m-agent-ready-apis.
- Overlap: 12 of these URLs are also in 6.5k-wildfire-apis-for-agents.
- Overlap: 1,026 of these URLs are also in 24k-traffic-apis-for-agents.
- Overlap: 26 of these URLs are also in 12k-parking-apis-for-agents.
- Overlap: 8 of these URLs are also in 10k-earthquake-apis-for-agents.
- Overlap: 7 of these URLs are also in 5.2k-volcano-tsunami-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Aviation API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
