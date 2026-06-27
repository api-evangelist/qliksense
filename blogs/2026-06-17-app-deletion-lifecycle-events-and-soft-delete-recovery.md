---
title: "App deletion lifecycle events and soft-delete recovery"
url: "https://qlik.dev/changelog/225-restore-deleted-apps/"
date: "2026-06-17"
feed_url: "https://qlik.dev/rss.xml"
---
Analytics apps now emit granular deletion events and can be recovered from soft-delete state via a new REST endpoint. Apps deleted after 45 minutes of creation enter a soft-delete recovery window with automatic purge within 14 days.
