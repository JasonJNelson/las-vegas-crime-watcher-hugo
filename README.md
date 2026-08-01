# Vegas Crime Watcher (Hugo)

Live-style Las Vegas crime map and incident feed, rebuilt as a **Hugo** static site.

## Features

- Interactive dark map (Leaflet + Carto)
- Color-coded markers by crime type
- Filterable crime feed
- Simulated live updates
- Stats bar (30-day aggregates)
- Login / Subscribe modals (demo)
- Three pricing tiers

## Project structure

```
.
├── archetypes/
├── content/
│   └── _index.md
├── data/
│   └── crimes.json          ← crime incidents (edit this to update data)
├── layouts/
│   ├── _default/
│   │   └── baseof.html
│   ├── index.html
│   └── partials/
│       ├── header.html
│       ├── stats.html
│       ├── map.html
│       ├── feed.html
│       ├── pricing.html
│       ├── modal.html
│       └── footer.html
├── static/
│   ├── css/style.css
│   └── js/crime-watcher.js
├── hugo.toml
└── README.md
```

## Requirements

- [Hugo](https://gohugo.io/) Extended (v0.120+ recommended)

## Local development

```bash
hugo server -D
# Open http://localhost:1313
```

## Build for production

```bash
hugo --minify
# Output is in public/
```

## Updating crime data

Edit `data/crimes.json`. After editing, restart `hugo server` or rebuild.

## Data notes

This is a **demo / educational** project.  
Incident data is illustrative and drawn from public LVMPD press releases and local reporting (July 2026).  
Not an official LVMPD product.

Always call **911** for emergencies.

## License

MIT
