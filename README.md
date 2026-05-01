# Safari Zen — Liquid Glass

A macOS Tahoe / Safari 26 inspired theme for Zen Browser. Applies Apple's Liquid Glass frosted translucent material to Zen's sidebar, toolbar, tabs, and menus while preserving your workspace gradient colors.

## Install via Sine

Paste this repo URL in Sine:

```
https://github.com/YOUR_USERNAME/safari-zen
```

## What it does

- **Sidebar**: Frosted glass overlay (`blur(40px) saturate(180%)`) layered on top of your workspace gradient with a specular rim highlight along the top edge
- **Tabs**: Glass pill tabs with inset specular shine on the active tab
- **URL bar**: Glass pill with centered text and blue focus glow
- **Toolbar**: Translucent glass layer
- **Menus & panels**: Glass popups with specular edges
- **Dark mode**: Fully adaptive

Your workspace/space gradient colors show through the glass — the mod never overrides the sidebar background.

## Recommended `about:config`

| Flag | Value |
|------|-------|
| `toolkit.legacyUserProfileCustomizations.stylesheets` | `true` |
| `zen.theme.gradient` | `true` |
| `browser.tabs.allow_transparent_browser` | `true` |

**macOS bonus** — for native system vibrancy under the glass:

| Flag | Value |
|------|-------|
| `zen.widget.mac-os.window-material` | `titlebar` or `sidebar` |

## Customization

Edit the CSS variables at the top of `chrome.css`:

- `--lg-glass-overlay` — glass opacity (lower = more gradient visible)
- `--lg-blur-heavy` — blur intensity
- `--lg-specular-strong` — top-edge highlight brightness
- `--lg-accent` — focus/selection color

## Credits

Liquid Glass effect informed by [Kube.io's refraction analysis](https://kube.io/blog/liquid-glass-css-svg/) and [archisvaze/liquid-glass](https://github.com/archisvaze/liquid-glass). True SVG displacement-map refraction requires Chromium; this mod uses CSS-only approximation compatible with Gecko/Firefox.
