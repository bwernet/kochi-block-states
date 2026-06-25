# Block state → interface behavior

An auto-cycling, self-contained case-study prototype showing how a published
shared block's state drives a prompt editor's interface behavior — in sync →
optional update → deferred → required update — with the real product UI reacting
to each state.

It's a single static file (`index.html`) — no build, no dependencies, no
framework. Open it directly, or host it anywhere.

## Live demos

Served via GitHub Pages:

- **Block lifecycle** — one shared block through its states:
  `https://bwernet.github.io/kochi-block-states/`
- **Editor + Cowork (conclusion)** — the whole product, resolving a shared-block update:
  `https://bwernet.github.io/kochi-block-states/editor-chrome/`
- **Design system → agent-built, designer-audited** — an agent reads a component's
  machine-readable spec to build it, and a designer audits the result against the same source:
  `https://bwernet.github.io/kochi-block-states/pixel-workbench/`

Each is a single static file (`index.html` / `editor-chrome/index.html` / `pixel-workbench/index.html`) — no build, no dependencies.

## Embedding (e.g. Framer)

GitHub Pages serves static HTML with no frame restrictions, so it embeds
cross-origin without any header changes:

```html
<iframe
  src="https://bwernet.github.io/kochi-block-states/"
  title="Block state → interface behavior"
  loading="lazy"
  scrolling="no"
  style="width:100%; height:900px; border:0; border-radius:16px;"
></iframe>
```

Size to ~900px tall (fits the tallest modal beats; shorter beats simply show more
of the canvas). Best viewed at tablet/desktop widths.

## Notes

- Auto-cycles continuously; a Pause/Play control and clickable state labels allow
  manual stepping. Respects `prefers-reduced-motion`.
- The product UI (the dark "northwind-support" panel) reproduces Kochi's real
  components, tokens, icons, and copy. The surrounding canvas is the case study's
  own visual identity.
