# Atlior — Brand Assets

Public delivery of Atlior's brand assets, served over a CDN at **https://assets.atlior.com**
(GitHub Pages). This is the single, central source every Atlior product references for logos,
favicons, OG images and the email-signature mark.

> Public by nature — these files are meant to be seen (logos on a site, an image in an email).
> Anything internal (the styleguide, design rationale, contact templates) lives in the private
> `Atlior/brand` repo, not here.

## Structure & URLs

| Path | URL |
|------|-----|
| `logo/atlior-logo.svg` | https://assets.atlior.com/logo/atlior-logo.svg |
| `logo/atlior-logo-full.svg` | https://assets.atlior.com/logo/atlior-logo-full.svg |
| `logo/atlior-app-icon.svg` | https://assets.atlior.com/logo/atlior-app-icon.svg |
| `favicon/` (full set + webmanifest) | https://assets.atlior.com/favicon/favicon.svg |
| `og/og-banner.png` | https://assets.atlior.com/og/og-banner.png |
| `email/atlior-mark.png` | https://assets.atlior.com/email/atlior-mark.png |

## Usage

**Favicon** — copy the `favicon/` set into each app's web root, or reference directly:
```html
<link rel="icon" href="https://assets.atlior.com/favicon/favicon.svg" type="image/svg+xml">
<link rel="apple-touch-icon" href="https://assets.atlior.com/favicon/apple-touch-icon.png">
```

**Open Graph** — per page:
```html
<meta property="og:image" content="https://assets.atlior.com/og/og-banner.png">
```

**Email signature** — the mark is a hosted PNG (SVG is blocked in most mail clients):
```html
<img src="https://assets.atlior.com/email/atlior-mark.png" alt="Atlior" width="80" height="70">
```

## Interim CDN (before DNS resolves)

Until `assets.atlior.com` is live, the same files are served by jsDelivr:
```
https://cdn.jsdelivr.net/gh/Atlior/assets@main/<path>
```

## Brand tokens

Primary blue `#0040FF` · Dark Navy `#0B1325` · White `#FFFFFF` · Light Neutral `#F5F7FA`.
Fonts: Plus Jakarta Sans (headings), Inter (body). Full token reference lives in `Atlior/brand`.
