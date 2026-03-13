# Enterprise Color Palettes

A curated set of color palettes for enterprise client applications. Each palette is designed for a specific use-case and tone, with consistent semantic roles (Canvas, Primary, Accent, Text, Success, Warning, Error).

## Preview

Open `color_palette.html` in a browser to see all palettes rendered as swatches.

## Palettes

| # | Name | Best For |
|---|------|----------|
| 1 | **Enterprise Blue** | Conservative B2B dashboards |
| 2 | **Navy & Cobalt** | Finance / consulting |
| 3 | **Teal & Slate** | Modern SaaS / AI tools |
| 4 | **Dark Theme Enterprise** | Power-user dashboards |
| 5 | **Warm Neutral + Royal Blue** | Internal tools / portals |

## Color Tokens

### 1. Enterprise Blue
| Role | Hex |
|------|-----|
| Canvas | `#F5F7FA` |
| Primary | `#2563EB` |
| Text | `#1F2933` |
| Success | `#16A34A` |
| Warning | `#F59E0B` |
| Error | `#DC2626` |

### 2. Navy & Cobalt
| Role | Hex |
|------|-----|
| Canvas | `#F4F5F7` |
| Primary | `#000080` |
| Primary Light | `#2563EB` |
| Accent | `#00B4D8` |
| Success | `#0F766E` |
| Error | `#B91C1C` |

### 3. Teal & Slate
| Role | Hex |
|------|-----|
| Canvas | `#F4F6F8` |
| Primary | `#0F766E` |
| Accent | `#3B82F6` |
| Text | `#111827` |
| Success | `#22C55E` |
| Error | `#EF4444` |

### 4. Dark Theme Enterprise
| Role | Hex |
|------|-----|
| Canvas | `#020617` |
| Surface | `#0B1120` |
| Primary | `#38BDF8` |
| Text | `#E5E7EB` |
| Success | `#22C55E` |
| Error | `#F97316` |

### 5. Warm Neutral + Royal Blue
| Role | Hex |
|------|-----|
| Canvas | `#FAFAF9` |
| Primary | `#4169E1` |
| Secondary | `#F5EDE3` |
| Accent | `#FFC857` |
| Success | `#2BA84A` |
| Error | `#E63946` |

## Usage

### CSS Variables

Import `tokens.css` and use the CSS custom properties:

```css
@import 'tokens.css';

/* Use Palette 1 – Enterprise Blue */
body {
  background: var(--palette-1-canvas);
  color: var(--palette-1-text);
}

button {
  background: var(--palette-1-primary);
}
```

### JSON

`tokens.json` contains all palettes in a structured format for use in design tools, build pipelines, or JS/TS applications:

```js
import tokens from './tokens.json';

const primary = tokens.palettes[0].colors.primary; // "#2563EB"
```

## Files

```
color-palette/
├── color_palette.html   # Visual preview of all palettes
├── tokens.css           # CSS custom properties for all palettes
├── tokens.json          # Machine-readable color tokens
└── README.md
```
