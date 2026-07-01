# DroneController_Docs

Public documentation for **DronController**.

- **`slides.json`** (repo root) — the rotating tips shown in the DronController **launcher**'s documentation
  panel. The launcher fetches it from
  `https://raw.githubusercontent.com/miagton/DroneController_Docs/main/slides.json` on every launch, so edits
  here go live next launch (no app release). A slide's `url` opens the matching page; a slide without a `url`
  opens the wiki home.
- **[Wiki](https://github.com/miagton/DroneController_Docs/wiki)** — the full documentation pages
  (Overview, HUD, Map, General, Streaming, Connection, Control, WireGuard).

## Editing `slides.json`

```json
{
  "docsUrl": "https://github.com/miagton/DroneController_Docs/wiki",
  "background": null,
  "slides": [
    { "title": "Short heading", "text": "A sentence or two.", "url": ".../wiki/PageName", "image": null }
  ]
}
```

Keep `title` to one line and `text` to a sentence or two — the launcher panel is compact. `image` /
`background` are reserved for a future visual phase and ignored for now.
