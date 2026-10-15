---
name: Stuy Town Assassin
description: A night mission app that deals one secret target to each phone.
colors:
  night-navy: "#070b14"
  panel-navy: "#0d1424"
  raised-navy: "#121b2e"
  ink: "#e6edf3"
  muted-steel: "#8a98aa"
  hairline: "#1f2a3d"
  signal-cyan: "#00e5ff"
  signal-cyan-hi: "#6ff2ff"
  hot-red: "#ff2e63"
  field-edge: "#2f6f86"
  field-edge-hover: "#3f8faa"
typography:
  display:
    fontFamily: "Rajdhani, Arial Narrow, Helvetica Neue, sans-serif"
    fontSize: "clamp(30px, 11.5vw, 48px)"
    fontWeight: 700
    lineHeight: 0.92
    letterSpacing: "0.06em"
  display-sigil:
    fontFamily: "Rajdhani, Arial Narrow, Helvetica Neue, sans-serif"
    fontSize: "clamp(20px, 6.4vw, 26px)"
    fontWeight: 700
    lineHeight: 0.92
    letterSpacing: "0.06em"
  code-display:
    fontFamily: "Rajdhani, Arial Narrow, Helvetica Neue, sans-serif"
    fontSize: "clamp(36px, 15vw, 64px)"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "0.32em"
  target-name:
    fontFamily: "Rajdhani, Arial Narrow, Helvetica Neue, sans-serif"
    fontSize: "clamp(30px, 10vw, 46px)"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "0.06em"
  code-input:
    fontFamily: "Rajdhani, Arial Narrow, Helvetica Neue, sans-serif"
    fontSize: "28px"
    fontWeight: 700
    letterSpacing: "0.45em"
  headline:
    fontFamily: "Rajdhani, Arial Narrow, Helvetica Neue, sans-serif"
    fontSize: "24px"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "0.08em"
  number:
    fontFamily: "Rajdhani, Arial Narrow, Helvetica Neue, sans-serif"
    fontSize: "22px"
    fontWeight: 700
    letterSpacing: "0.06em"
    fontFeature: "tnum"
  button:
    fontFamily: "Rajdhani, Arial Narrow, Helvetica Neue, sans-serif"
    fontSize: "18px"
    fontWeight: 700
    letterSpacing: "0.1em"
  panel-title:
    fontFamily: "Rajdhani, Arial Narrow, Helvetica Neue, sans-serif"
    fontSize: "15px"
    fontWeight: 700
    letterSpacing: "0.2em"
  tagline:
    fontFamily: "Rajdhani, Arial Narrow, Helvetica Neue, sans-serif"
    fontSize: "clamp(11px, 3.4vw, 14px)"
    fontWeight: 600
    letterSpacing: "0.16em"
  signal:
    fontFamily: "Rajdhani, Arial Narrow, Helvetica Neue, sans-serif"
    fontSize: "13px"
    fontWeight: 700
    letterSpacing: "0.24em"
  tag:
    fontFamily: "Rajdhani, Arial Narrow, Helvetica Neue, sans-serif"
    fontSize: "12px"
    fontWeight: 700
    letterSpacing: "0.16em"
  body-large:
    fontFamily: "Inter, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.5
  body:
    fontFamily: "Inter, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.5
  body-small:
    fontFamily: "Inter, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.5
  hint:
    fontFamily: "Inter, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "13px"
    fontWeight: 500
    lineHeight: 1.5
  label:
    fontFamily: "Inter, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "12px"
    fontWeight: 600
    letterSpacing: "0.14em"
rounded:
  sm: "2px"
  full: "50%"
spacing:
  hair: "4px"
  tight: "8px"
  inline: "12px"
  stack: "16px"
  group: "24px"
  section: "32px"
  zone: "48px"
  tap: "48px"
components:
  button-primary:
    backgroundColor: "{colors.signal-cyan}"
    textColor: "{colors.night-navy}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: "12px 16px"
    height: "48px"
  button-primary-hover:
    backgroundColor: "{colors.signal-cyan-hi}"
    textColor: "{colors.night-navy}"
  button-alt:
    backgroundColor: "transparent"
    textColor: "{colors.hot-red}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: "12px 16px"
    height: "48px"
  button-default:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: "12px 16px"
    height: "48px"
  button-default-hover:
    backgroundColor: "{colors.raised-navy}"
    textColor: "{colors.ink}"
  button-danger:
    backgroundColor: "{colors.hot-red}"
    textColor: "{colors.night-navy}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: "12px 16px"
    height: "48px"
  input:
    backgroundColor: "{colors.night-navy}"
    textColor: "{colors.ink}"
    typography: "{typography.body-large}"
    rounded: "{rounded.sm}"
    padding: "12px 16px"
    height: "48px"
  input-code:
    backgroundColor: "{colors.night-navy}"
    textColor: "{colors.ink}"
    typography: "{typography.code-input}"
    rounded: "{rounded.sm}"
    padding: "6px 16px"
    height: "48px"
  panel:
    backgroundColor: "{colors.panel-navy}"
    textColor: "{colors.ink}"
    rounded: "{rounded.sm}"
    padding: "clamp(16px, 6vw, 24px)"
  tag-host:
    backgroundColor: "transparent"
    textColor: "{colors.hot-red}"
    typography: "{typography.tag}"
    rounded: "{rounded.sm}"
    padding: "1px 8px"
  target-reveal:
    backgroundColor: "{colors.night-navy}"
    textColor: "{colors.ink}"
    typography: "{typography.target-name}"
    rounded: "{rounded.sm}"
    padding: "32px 16px"
    height: "184px"
---

# Design System: Stuy Town Assassin

## Overview

**Creative North Star: "The Night Op"**

The phone becomes a mission terminal for exactly one secret. The system is the spy-app category standard played straight, at the polish of a competitive shooter's client: a night-navy ground under faint scanlines, hairline panels whose corners are marked by cyan brackets, condensed capitals for anything the player must read at a glance, and a crosshair reticle that opens the app full-size and shrinks to a sigil once the player is inside a room. Two signals carry all meaning: cyan says go, codes and focus; red says host, waiting and danger.

Density is low and the column is narrow (440px at most), built for one phone in one hand in a noisy room. Light is rationed: only the reticle, the home title, the room code and the primary button glow, and everything else is flat hairline on navy. The system peaks in one place, the target box, where holding closes the brackets in, snaps a reticle over the redaction bar, decrypts the name by character scramble and runs a five-second cyan drain.

It refuses the hacker console (code rain, fake command lines, monospace prompts) and the paper dossier (cream sheets, rubber stamps, typewriter labels). The hatched cyan redaction bar is the one device carried forward from the original app.

**Key Characteristics:**
- One dark theme only (color-scheme dark); three navy steps for ground, panel and raised.
- Cyan and red are signals with fixed meanings, never decoration.
- Rajdhani 600/700 capitals for display, buttons, codes and numbers; Inter for every sentence.
- 2px corners, 1px hairlines, 16px cyan corner brackets on panels; circles only for reticles.
- 48px minimum touch targets throughout.
- Motion lives in the lock-on; reduced motion swaps instantly.

## Colors

A night-op palette: near-black navy layered in three close steps, cool steel neutrals, and two saturated signals that never trade jobs.

### Primary
- **Signal Cyan** (#00e5ff): the primary action fill (Join room, Start game), the room code, numbers on the host board, corner brackets, the reticle, the redaction bar, the drain bar, the text caret, selection and every focus ring. 12.8:1 on the ground.
- **Signal Cyan Hi** (#6ff2ff): hover fill for the primary button only.

### Secondary
- **Hot Red** (#ff2e63): the secondary action outline (Create a new room), the Host tag, the "waiting" roster heading, the target toggle row, the tagline, errors, notes (as a 45% edge and 8% tint) and the destructive Leave fill. 5.5:1 on the ground; dark navy text on its fill.

### Neutral
- **Night Navy** (#070b14): the page ground, the inside of inputs and the target box, and the text color on cyan and red fills.
- **Panel Navy** (#0d1424): bracketed panels and the target toggle row.
- **Raised Navy** (#121b2e): hover fill for default and toggle buttons.
- **Ink** (#e6edf3): all primary text. 16.7:1 on the ground.
- **Muted Steel** (#8a98aa): labels, helper text, placeholders, received names, the "or" divider, link buttons, default button edges. 6.7:1 on the ground.
- **Hairline** (#1f2a3d): panel edges, list rules, divider lines, the leave-zone rule.
- **Field Edge** (#2f6f86): input borders at rest, a dimmed cyan so fields read as part of the signal family. 3.5:1 on the ground, above the 3:1 non-text floor.
- **Field Edge Hover** (#3f8faa): input border on hover, between rest and the full cyan of focus.

### Named Rules
**The Two Signals Rule.** Cyan means go, codes and focus; red means host, waiting and danger. A color never borrows the other's job, and neither is used as an ornament.

**The Night Ground Rule.** There is one theme. Surfaces step up through night, panel and raised navy only; no light mode, no gray cards, no gradients other than the scanlines.

## Typography

**Display Font:** Rajdhani (with Arial Narrow, Helvetica Neue, sans-serif)
**Body Font:** Inter (with system-ui, -apple-system, Segoe UI, sans-serif)

**Character:** Rajdhani's squared, condensed capitals give the game-client voice to titles, buttons, codes and counts; Inter keeps every instruction calm and legible at phone sizes. Both faces load without blocking first paint.

### Hierarchy
- **Display** (700, clamp 30-48px, 0.92, 0.06em caps): the app title on Home, with a faint cyan glow.
- **Display Sigil** (700, clamp 20-26px, 0.06em caps): the same title inside a room, beside the 40px reticle, without glow.
- **Code Display** (700, clamp 36-64px, 1, 0.32em): the room code in the lobby, in cyan with glow.
- **Target Name** (700, clamp 30-46px, 1, 0.06em caps): the decrypted target name, and the height of the redaction bar.
- **Code Input** (700, 28px, 0.45em caps): the four-letter room code field.
- **Headline** (700, 24px, 1.1, 0.08em caps): screen headings such as Host panel.
- **Number** (700, 22px, 0.06em, tabular): host-board counts, in cyan.
- **Button** (700, 18px, 0.1em caps): every button label.
- **Panel Title** (700, 15px, 0.2em caps): the heading that names a panel when no larger heading exists, as on the target panel.
- **Tagline** (600, clamp 11-14px, 0.16em caps): the single red line under the Home title.
- **Signal** (700, 13px, 0.2-0.24em caps): the "or" divider and the Open/Close state on the target toggle.
- **Tag** (700, 12px, 0.16em caps): the Host tag.
- **Body Large** (Inter 400, 17px, 1.5): input text and the host-board sentence.
- **Body** (Inter 400, 16px, 1.5): default text.
- **Body Small** (Inter 400, 14px, 1.5): helper paragraphs, notes, errors, link buttons, definition values.
- **Hint** (Inter 500, 13px): the instruction inside the target box.
- **Label** (Inter 600, 12px, 0.14em caps, muted): field labels, definition terms and roster group headings.

### Named Rules
**The Caps Command, Inter Explains Rule.** Rajdhani capitals are for things you act on or read at a glance: titles, buttons, codes, counts, tags. Any full sentence is Inter in sentence case.

**The Wide Code Rule.** Room codes are always tracked wide (0.32em displayed, 0.45em in the field) so four letters can be read across a room.

## Layout

A single centered column, at most 440px, with 16px side gutters that grow with the safe-area insets; 32px top and 48px bottom padding. Screens stack their blocks with 24px gaps; inside panels the rhythm is 16px between fields and 8px between a label and its control. The spacing scale is 4, 8, 12, 16, 24, 32 and 48px, used by name (hair, tight, inline, stack, group, section, zone). Panel padding is fluid, clamp(16px, 6vw, 24px). Rows of buttons wrap with a 120px minimum per button. The leave action always sits apart from the main flow, below a hairline rule and at least 16px away.

On Home the masthead is a stacked, centered reticle (clamp 120-180px), title and tagline; on Lobby and Target it collapses to a single row with a 40px reticle and the smaller title, and the tagline is hidden so the room and the target lead.

## Elevation & Depth

Depth is tonal, not shadowed: three navy steps, 1px hairlines and corner brackets do the layering. Light replaces shadow in four sanctioned places only, all cyan and all part of the chosen world (recorded as detector exceptions in `.impeccable/config.json`). Faint horizontal scanlines (1px at 1.8% white every 4px) sit over the whole ground.

### Shadow Vocabulary
- **Primary lift** (`box-shadow: 0 8px 24px -10px rgba(0,229,255,.6)`): under the primary button only; removed when disabled.
- **Reticle glow** (`box-shadow: 0 0 28px -4px rgba(0,229,255,.45), inset 0 0 22px -6px rgba(0,229,255,.35)`): the Home reticle; dropped at sigil size.
- **Title glow** (`text-shadow: 0 0 18px rgba(0,229,255,.4)`): the Home title; dropped in-room.
- **Code glow** (`text-shadow: 0 0 22px rgba(0,229,255,.35)`): the lobby room code.

### Named Rules
**The Rationed Light Rule.** Glow appears only on the reticle, the Home title, the room code and the primary button. No panel, card, input or secondary button glows or casts a shadow.

## Shapes

Hard-cornered and technical. Every rectangle (panels, buttons, inputs, tags, notes, the redaction bar) uses 2px corners. Edges are 1px: hairline navy on panels, dimmed cyan on inputs, red or steel on outlined buttons. Bracketed panels carry four L-shaped cyan corner marks (16px arms, 2px thick) laid just over the hairline. The circle is reserved for reticles: the masthead crosshair (2px ring, inner 1px ring, center dot, gapped cross-hairs) and the lock reticle in the target box. The redaction bar is hatched: 2px cyan bands at 34% and 12% opacity under a 1px cyan inner edge, exactly one name-line tall.

### Named Rules
**The Bracket Rule.** A panel is marked by its corners, not by a heavier border or a fill change. Brackets are always cyan, 16px by 2px.

## Components

### Buttons
Decisive, flat and capitalized; color carries the whole hierarchy.
- **Shape:** sharp 2px corners, 48px minimum height, 12px by 16px padding.
- **Primary:** Signal Cyan fill, navy text, primary lift. One per screen (Join room, Start game).
- **Hover / Focus:** primary hover goes to Signal Cyan Hi; default hover fills Raised Navy and brightens the edge to ink; every button shows a 2px cyan outline at 3px offset on keyboard focus. Color transitions run 150ms.
- **Alt (secondary):** transparent with a Hot Red edge and red label (Create a new room); hover adds a 10% red tint.
- **Default:** transparent with a Muted Steel edge and ink label (Copy invite link, Cancel).
- **Danger:** Hot Red fill with navy text, only for the confirmed Leave.
- **Disabled:** 40% opacity, steel edge, no fill, no lift.
- **Link button:** Inter 14px, muted, underlined, no box; used only for Leave room / Leave this game.

### Chips
- **Host tag:** transparent, 1px Hot Red edge, red Rajdhani 12px caps, 2px corners. It is the only tag.

### Cards / Containers
- **Corner Style:** 2px.
- **Background:** Panel Navy.
- **Shadow Strategy:** none (see Elevation & Depth).
- **Border:** 1px Hairline plus cyan corner brackets.
- **Internal Padding:** clamp(16px, 6vw, 24px), with 16px between children.
- **Notes:** status notes (test mode, offline) are a lighter container: 1px red edge at 45%, 8% red tint, ink text, 8px by 12px padding.

### Inputs / Fields
- **Style:** Night Navy fill, 1px Field Edge border, 2px corners, 48px minimum, Inter 17px, cyan caret, muted placeholder. The room code field switches to Code Input type.
- **Hover:** border moves to Field Edge Hover.
- **Focus:** border turns Signal Cyan with a 2px cyan outline at 2px offset.
- **Error:** the field gets aria-invalid and points at a red Inter 14px error line below the form.

### Navigation
There is no navigation bar. The masthead (reticle, title, tagline) is the only persistent chrome; it shrinks to a reticle sigil and short title inside a room. Screen changes move focus to the new screen's heading, which shows a cyan focus outline.

### Lists
Player rosters are rule-separated rows: 1px Hairline above the list and under each row, 12px vertical padding, the name filling the row and tags at the end. Received names dim to muted; the waiting group's heading turns red. Definition lists (Agents, Status, Agent, Room) pair muted 12px caps terms with 14px Inter values in a two-column grid.

### Target Reveal (signature)
The one place the system performs.
- **At rest:** a Night Navy box, 1px Hairline, 2px corners, at least 184px tall, with cyan corner brackets inset 10px and the hatched redaction bar where the name will be, above a muted Inter hint.
- **Lock-on:** while held (or for 5 seconds after a tap) the brackets close in to frame the name line (220ms, cubic-bezier(.16,1,.3,1)); a 132px reticle (1px cyan at 55%) scales from 1.7 to 1 and fades in (260ms); the name decrypts left to right out of random glyphs over about 350ms; a 3px Signal Cyan drain bar along the bottom edge empties over exactly 5 seconds.
- **Above it:** when shown to the host, a full-width toggle row (Panel Navy, 1px red edge, 56px tall) with "Your target" and a red Open/Close state.
- **Reduced motion:** the name swaps in instantly; no scramble, no bracket or reticle snap, no drain animation. All transitions are disabled.

### Reticle Masthead (signature)
A cyan crosshair: 2px ring, a 1px inner ring at 34%, a 3px center dot and cross-hairs that extend 14px past the ring with a gap in the middle. clamp(120px, 46vw, 180px) with glow on Home; 40px, no glow, beside the title in a room; the size change eases over 300ms.

## Do's and Don'ts

### Do:
- **Do** keep cyan for go, codes and focus, and red for host, waiting and danger (The Two Signals Rule).
- **Do** set titles, buttons, codes, counts and tags in Rajdhani 700 capitals with positive tracking, and every sentence in Inter.
- **Do** give every control at least 48px of height and a 2px cyan focus outline.
- **Do** mark panels with 16px cyan corner brackets over a 1px hairline on Panel Navy.
- **Do** keep 2px corners on every rectangle and save circles for reticles.
- **Do** keep the hatched cyan redaction bar exactly one name-line tall so revealing never shifts the layout.
- **Do** honor prefers-reduced-motion with an instant swap and no scramble, snap or drain.

### Don't:
- **Don't** add glow beyond the reticle, the Home title, the room code and the primary button lift (The Rationed Light Rule).
- **Don't** drift toward a hacker terminal: no code rain, fake command lines or monospace prompts.
- **Don't** return to the paper dossier: no cream paper, rubber stamps or typewriter labels.
- **Don't** add a light theme or a fourth surface tone.
- **Don't** put a small tracked caps line above a heading as decoration; a panel gets a Panel Title only when it has no other heading.
- **Don't** round corners past 2px or soften panels with drop shadows.
- **Don't** let decoration slow joining: the name field, the code field and Join stay in the first viewport.
