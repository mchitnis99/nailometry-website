# Nailometry — Brand & UI/UX Guide

> The definitive reference for app, marketing, website, and social. Keep this consistent everywhere.

---

## Identity

**Brand name:** Nailometry  
**Tagline:** *Nails that actually fit you.*  
**Voice:** Confident, fun, feminine, a little editorial. Never fussy. Speaks to nail techs and beauty-obsessed women who take their craft seriously.

---

## Color Palette

| Name | Hex | Usage |
|------|-----|-------|
| **Hot Pink** | `#E8478A` | Primary CTA buttons, active states, links, badges |
| **Deep Rose** | `#B0275A` | Button hover/pressed, dark accents |
| **Soft Pink** | `#F2A7C3` | Subtle highlights, tags, secondary indicators |
| **Pale Pink** | `#FDE8F2` | Card backgrounds, hero tints, surface washes |
| **Lilac** | `#D9C4F0` | Secondary accent, filters, alt highlights |
| **Cream** | `#F8F4EF` | App/page background — always the base |
| **White** | `#FFFFFF` | Cards, surfaces, modals |
| **Near Black** | `#0F0D0C` | All body text and headings |
| **Mid Tone** | `#4A3040` | Secondary/muted text |
| **Faint** | `#9A8090` | Placeholder text, disabled states |

### Do's
- Hot Pink `#E8478A` is the **only** primary action color. Use it sparingly and deliberately — buttons, active icons, key labels.
- Use Cream `#F8F4EF` as your background, White `#FFFFFF` for elevated surfaces (cards, sheets).
- Pale Pink `#FDE8F2` for hero section washes and empty states.
- Lilac `#D9C4F0` as a secondary accent (not competing with hot pink — complement it).

### Don'ts
- Don't use more than 2 accent colors on a single screen.
- Never put hot pink text on a pale pink background (low contrast).
- Avoid pure black `#000000` — always use Near Black `#0F0D0C`.

---

## Typography

Three fonts. No exceptions.

### 1. Syne — Display
**Use for:** Screen titles, section headings, button labels, navigation labels, eyebrow tags, bold UI elements  
**Weights:** `Syne_700Bold`, `Syne_800ExtraBold`  
**Google Fonts:** `Syne`  
**Character:** Geometric, bold, modern, strong personality. The workhorse of headings.

```
Clients          ← Syne 700 Bold, 32px
BRANDS           ← Syne 700 Bold, 32px
Get Sized ✦      ← Syne 700 Bold (button label)
✦ your studio   ← Syne 500/700, 11px, tracking 0.4
```

### 2. Cormorant Garamond — Editorial Serif
**Use for:** Hero titles, romantic accents, app name/logo, client names in profiles, brand names  
**Weights:** `CormorantGaramond_700Bold_Italic`, `CormorantGaramond_400Regular_Italic`  
**Google Fonts:** `Cormorant Garamond`  
**Character:** Elegant, feminine, editorial. The emotional hook. Use for moments that should feel special.

```
NailFit                        ← CormorantGaramond 700 Bold Italic, 48px
Welcome back                   ← CormorantGaramond 700 Bold Italic, 26px
your studio, beautifully organized  ← CormorantGaramond 400 Italic, 15px
```

### 3. DM Sans — Body
**Use for:** Body copy, form fields, input text, descriptions, sub-labels, tab bar labels, footnotes  
**Weights:** `DMSans_400Regular`, `DMSans_500Medium`  
**Google Fonts:** `DM Sans`  
**Character:** Humanist, clean, very readable at small sizes. Invisible but essential.

```
3 size sets        ← DM Sans 400, 13px
you@example.com    ← DM Sans 400, 15px
Email              ← DM Sans 500, 11px, tracking 0.8 (form label)
Clients (tab bar)  ← DM Sans 500, 10px
```

### Type Scale

| Token | Size | Use |
|-------|------|-----|
| `fontSizeXS` | 11px | Eyebrow tags, badges, micro labels |
| `fontSizeSM` | 13px | Secondary text, captions, sub-labels |
| `fontSizeMD` | 15px | Body, inputs, default UI |
| `fontSizeLG` | 18px | Sub-headings, card titles |
| `fontSizeXL` | 22px | Section headings |
| `fontSize2XL` | 26px | Card/modal headings |
| `fontSize3XL` | 32px | Screen titles |
| Hero | 48px | Login/splash hero title |

---

## Spacing

| Token | Value | Use |
|-------|-------|-----|
| `xs` | 4px | Icon gaps, micro padding |
| `sm` | 8px | Tight internal padding |
| `md` | 14px | Default component padding |
| `lg` | 18px | Section padding |
| `xl` | 24px | Card/screen padding |
| `xxl` | 36px | Section gaps |
| `xxxl` | 52px | Bottom safe area, page ends |

---

## Border Radius

| Token | Value | Use |
|-------|-------|-----|
| `sm` | 10px | Small chips, table rows |
| `md` | 16px | Inputs, small cards |
| `lg` | 22px | Main cards |
| `xl` | 30px | Modals, large cards |
| `xxl` | 40px | Hero sections |
| `full` | 9999px | Pills, avatars, icon buttons, CTAs |

**Rule:** Buttons always use `full` (pill shape). Cards use `lg` or `xl`. Inputs use `md`.

---

## Components

### Primary Button
- Shape: **pill** (border-radius full)
- Background: `#E8478A` Hot Pink
- Label: **Syne_700Bold**, white, 15px, letter-spacing 0.6
- Height: ~52px (padding 16px vertical)
- Example: *"Sign In"*, *"Save Changes"*, *"Get Sized ✦"*

### Outline Button
- Shape: pill, border 1.5px `#E8478A`
- Background: white
- Label: **Syne_700Bold**, hot pink, 15px, letter-spacing 0.6
- Example: *"See How ↓"*

### Ghost Button
- No border, no background
- Label: **Syne_700Bold**, hot pink, 13px
- Example: *"Cancel"*, *"Learn more"*

---

## Screen Headers

```
✦ your studio              ← DM Sans 500, 11px, Hot Pink, tracking 0.4
Clients                    ← Syne 700, 32px, Near Black, tracking -0.5
```

- Eyebrow (✦ label): DM Sans 500 Medium, 11px, Hot Pink
- Screen title: Syne 700 Bold, 32px, Near Black
- Background: White surface with 1px cream border at bottom

---

## Cards

- Background: `#FFFFFF`
- Border: 1px `#E8D8E0`
- Border radius: `lg` (22px)
- Client name in card: DM Sans 500 Medium, 15px
- Sub-label: DM Sans 400, 11px, italic, Faint color

---

## Avatars

- Shape: circle
- Initials: **Syne_700Bold**
- Colors rotate through: hot pink/deep rose, lavender, plum, honey, teal, sage
- Size: 44–76px depending on context

---

## Tone of Voice

| Context | Tone | Example |
|---------|------|---------|
| Empty states | Warm + encouraging | *"no clients yet — tap + to add your first"* |
| Error messages | Direct, not scary | *"That email isn't right. Give it another go."* |
| Success states | Celebratory | *"Saved! ✦"* |
| CTA labels | Action-forward, punchy | *"Get Sized ✦"*, *"Find My Fit"* |
| Section labels | Editorial, all-lowercase or small caps | *"✦ your studio"*, *"✦ reference guide"* |

### Signature touches
- Use **✦** (sparkle star) as a brand punctuation mark — in eyebrow labels, CTAs, section dividers
- Use **→** for navigation links (not >)
- All lowercase for eyebrow/tag text
- Sentence case for headings and body (not title case)

---

## Marketing & Website Application

Apply the same system:

- **Web background:** `#F8F4EF` cream
- **Hero text:** Cormorant Garamond Italic Bold for the romantic italic word, Syne ExtraBold for the bold display line
- **Nav links:** DM Sans 400/500, uppercase, letter-spacing 1–2px
- **CTA button:** Hot Pink pill, Syne 700 Bold label
- **Section dividers:** 1px `#E8D8E0` line
- **Marquee/ticker text:** Syne 700 Bold, uppercase, Hot Pink + Near Black alternating

---

## Social Media

- **Primary palette:** Hot Pink + Cream + Near Black
- **Accent:** Lilac for secondary posts/Stories
- **Font on graphics:** Syne Bold for headlines, Cormorant Garamond Italic for romantic sub-lines
- **Emojis to use:** 💅 🌷 ✦ 🎀 💎 (not 🔥 💥 — keep it feminine/editorial)

---

*Last updated: May 2026 · Matches nailometry.app design system*