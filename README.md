# walkmeter-field-tmp

**TEMPORARY — EXPERIMENT INFRASTRUCTURE ONLY.**

This repository exists for one purpose: to serve a single frozen, self-contained HTML
measurement tool over HTTPS, unmodified, so it can be opened on a phone. A secure context is
required because the browser Geolocation API refuses to run over `file://` or plain HTTP.

- `walkmeter-1.1.0.html` — frozen instrument, served byte-for-byte unmodified.
  SHA-256 `a60bd9169ee87593f15e545199ff6c038349cd90cf136bb1fb930f126d59f8a4`
- `.nojekyll` — disables Jekyll processing so the file is served exactly as committed.

No analytics. No additional JavaScript. No service worker. No external resources.
The page makes no network request of any kind.

Contains no application source, records, results, secrets or data of any kind.

Do not reuse this repository for anything else. Delete once the field experiment and its
record are complete.
