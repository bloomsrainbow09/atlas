# Atlas

The website for Atlas, a search over 400,100,434 people.

This repository holds **no application code and no data**. It contains one
workflow, which checks out the application from its private repository with a
read-only deploy key, builds the frontend, and publishes it to GitHub Pages.

* **App:** https://bloomsrainbow09.github.io/atlas/
* **API:** `https://3-236-111-101.sslip.io:47991` — the backend runs on a
  GitHub Actions runner and is reached through Caddy on a small EC2 instance,
  which is the one address that does not change.

The app is password-gated. The lake itself — 116 GiB of Parquet — is on Google
Drive and is never served from here.
