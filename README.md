# Fly.io deployment

This repository is a single-file HTML app. The Dockerfile serves it with Nginx; no Node, Linux desktop, or build step is required. ChromeOS users access it in Chrome as a normal website.

## Deploy

This app is configured with `fly.toml` and a Dockerfile. The current repository provides a static website deployment only; it does not add a remote Chromium service or an HTTP proxy. The in-app iframe remains subject to browser and destination-site embedding restrictions.

To deploy without using a terminal, connect this GitHub repository to Fly.io's dashboard and select the `private-chromium-browser` branch. Fly builds the Dockerfile and reads `fly.toml` automatically. If the dashboard asks for an app name, use `bib-l5e-eq`; set the primary region to `iad`.
