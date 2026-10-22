# Goalie Points

Public dashboard for goalie goals and assists in our ESPN fantasy hockey league. ESPN doesn't score them, so a bot finds them and applies the points as score adjustments.

- `index.html`: the whole site (Tailwind + Alpine.js from CDNs, no build step).
- `data.json`: generated and pushed by the bot hourly during game hours. Don't edit it by hand; the next run will overwrite your changes.

## Preview locally

```
python3 -m http.server 8000
```

Then open http://localhost:8000. Opening `index.html` directly from disk won't work, because browsers block `fetch()` of local files.
