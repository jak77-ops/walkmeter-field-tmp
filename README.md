# walkmeter-field-tmp

**TEMPORARY — EXPERIMENT INFRASTRUCTURE ONLY.**

This repository exists for one purpose: to serve frozen, self-contained HTML tools over HTTPS,
unmodified, so they can be opened on a phone. A secure context is required because the browser
Geolocation API refuses to run over `file://` or plain HTTP.

- `walkmeter-1.1.0.html` — frozen measurement instrument, served byte-for-byte unmodified.
  SHA-256 `a60bd9169ee87593f15e545199ff6c038349cd90cf136bb1fb930f126d59f8a4`
- `speedprobe-1.0.0.html` — frozen capability probe. Reads only `coords.speed`,
  `coords.accuracy` and `timestamp`; never reads latitude or longitude; computes no distance.
  SHA-256 `66a9cd57607ff38e4862dffe04969c79108d0a2e0074f4539666c2dcedc95c3f`
- `.nojekyll` — disables Jekyll processing so files are served exactly as committed.

No analytics. No additional JavaScript. No service worker. No external resources.
Neither page makes a network request of any kind.

Contains no application source, records, results, secrets or data of any kind.

Do not reuse this repository for anything else. Delete once the field experiments and their
records are complete.
