---
name: Stuy Town Assassin
description: A case file that deals secret targets, one phone at a time.
colors:
  signal-red: "#b4232f"
  signal-red-dark: "#ff5a63"
  on-signal: "#ffffff"
  on-signal-dark: "#1a0b0c"
  night-ink: "#141a24"
  night-ink-dark: "#e8edf3"
  cool-paper: "#eef1f4"
  cool-paper-dark: "#0f141c"
  blank-sheet: "#ffffff"
  blank-sheet-dark: "#18202b"
  pencil-gray: "#5b6576"
  pencil-gray-dark: "#93a0b2"
  rule-line: "#d5dbe3"
  rule-line-dark: "#2a3442"
  field-edge: "#7f8999"
  field-edge-dark: "#66738a"
  blush-note: "#f6e3e4"
  blush-note-dark: "#3a1d22"
typography:
  display:
    fontFamily: "Archivo Black, Arial Black, Impact, sans-serif"
    fontSize: "clamp(26px, 10vw, 46px)"
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "Archivo Black, Arial Black, Impact, sans-serif"
    fontSize: "22px"
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: "0.01em"
  title:
    fontFamily: "Archivo Black, Arial Black, Impact, sans-serif"
    fontSize: "clamp(22px, 9vw, 40px)"
    fontWeight: 400
    lineHeight: 1.05
  body:
    fontFamily: "Archivo, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.5
  body-small:
    fontFamily: "Archivo, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: "JetBrains Mono, ui-monospace, Menlo, Consolas, monospace"
    fontSize: "12px"
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: "0.1em"
  code:
    fontFamily: "JetBrains Mono, ui-monospace, Menlo, Consolas, monospace"
    fontSize: "clamp(28px, 10vw, 40px)"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "0.25em"
rounded:
  hair: "2px"
  tag: "3px"
  sheet: "4px"
spacing:
  hair: "4px"
  tight: "8px"
  inline: "12px"
  stack: "16px"
  group: "24px"
  section: "32px"
  zone: "48px"
components:
  button-primary:
    backgroundColor: "{colors.signal-red}"
    textColor: "{colors.on-signal}"
    rounded: "{rounded.sheet}"
    padding: "12px 16px"
    height: "48px"
  button-secondary:
    backgroundColor: "{colors.blank-sheet}"
    textColor: "{colors.night-ink}"
    rounded: "{rounded.sheet}"
    padding: "12px 16px"
    height: "48px"
  button-link:
    textColor: "{colors.pencil-gray}"
    typography: "{typography.body-small}"
    padding: "12px 0"
    height: "48px"
  input:
    backgroundColor: "{colors.cool-paper}"
    textColor: "{colors.night-ink}"
    rounded: "{rounded.sheet}"
    padding: "12px 16px"
    height: "48px"
  case-file:
    backgroundColor: "{colors.blank-sheet}"
    textColor: "{colors.night-ink}"
    rounded: "{rounded.sheet}"
    padding: "24px"
  stamp:
    textColor: "{colors.signal-red}"
    padding: "4px 12px"
  tag:
    textColor: "{colors.pencil-gray}"
    typography: "{typography.label}"
    rounded: "{rounded.tag}"
    padding: "2px 8px"
  note:
    backgroundColor: "{colors.blush-note}"
    textColor: "{colors.night-ink}"
    typography: "{typography.body-small}"
    rounded: "{rounded.sheet}"
    padding: "8px 12px"
---

# Design System: Stuy Town Assassin

## Overview

**Creative North Star: "The Case File"**

Every screen is a page in the same dossier: a sheet of paper with an ink frame, a rubber stamp in the corner, typed labels down the margin, and a redaction bar over anything secret. The tone is playful but serious. The spy-file theatre is played straight, the stamps and voice carry a wink, and the controls themselves never joke. The theatre is there to make secrecy feel real to a friend group standing in one room, each holding a phone.

The system is built for one narrow column on a phone held in one hand. Density is low and deliberate: one sheet per screen, one primary action per sheet, generous separation before anything destructive. Expression comes from the system's own few devices (stamps, frames, mono labels, redaction), never from added decoration. It is flat at rest, uses a single red, and works in light and dark from the same tokens.

**Key Characteristics:**
- One case-file sheet per screen, framed in 2px Night Ink with 4px corners.
- A rotated Signal Red stamp names each screen's state: Recruiting, Standby, Confidential.
- Typed-paperwork labels: uppercase JetBrains Mono at 12px, with 0.1em letter spacing.
- Heavy uppercase Archivo Black for the title, headings and the revealed name.
- Secrets are redacted by default and shown only on an explicit hold or tap.
- A 4px spacing scale with a 48px minimum control height.

## Colors

The palette is cool paper and night ink with a single signal red, and every role has a light and a dark value.

### Primary
- **Signal Red** (light `signal-red` / dark `signal-red-dark`): the only accent. It is used for the primary action (Join, Start, Leave), the stamps, the room code, the title kicker, focus rings, text selection, the caret and error text. It means "this matters now". On a red fill, text uses **On Signal** (white in light mode, near-black in dark mode).

### Neutral
- **Night Ink** (`night-ink` / `night-ink-dark`): body text, and the 2px frame around every case-file sheet and the host's "Your target" row.
- **Cool Paper** (`cool-paper` / `cool-paper-dark`): the page background, and the fill of inputs and the reveal box, so typed and secret content sits slightly recessed in the sheet.
- **Blank Sheet** (`blank-sheet` / `blank-sheet-dark`): the surface of case-file sheets.
- **Pencil Gray** (`pencil-gray` / `pencil-gray-dark`): secondary text, mono labels, hints and the Leave links. It passes 4.5:1 on every surface it sits on.
- **Rule Line** (`rule-line` / `rule-line-dark`): dividers and roster rules only. It is never used to outline an interactive control.
- **Field Edge** (`field-edge` / `field-edge-dark`): input borders, at 3:1 or better against the sheet in both themes.
- **Blush Note** (`blush-note` / `blush-note-dark`): the background of system notes (test mode, lost connection).

### Named Rules
**The One Signal Rule.** Signal Red is the only accent. There is no second hue for success, info or decoration; status is carried by words and grouping ("Waiting · 2", "Received · 6").

**The Ink Frame Rule.** Dividers use Rule Line, input borders use Field Edge, and containers use Night Ink. Never swap them: a Rule Line border on a control fails contrast, and a Night Ink divider shouts.

## Typography

**Display Font:** Archivo Black (fallback: Arial Black, Impact, sans-serif)
**Body Font:** Archivo (fallback: system-ui, -apple-system, Segoe UI, sans-serif)
**Label/Mono Font:** JetBrains Mono (fallback: ui-monospace, Menlo, Consolas, monospace)

**Character:** a heavy grotesque in capitals does the shouting, a plain sans carries the instructions, and a typewriter-style mono files everything under labels. Together they read as a stamped, typed document.

### Hierarchy
- **Display** (Archivo Black, `clamp(26px, 10vw, 46px)`, line height 0.95, uppercase, balanced wrapping): the app title. It steps down to `clamp(22px, 7.5vw, 28px)` once the player is in a room, so the room and the target lead.
- **Headline** (Archivo Black, 22px, uppercase): section headings such as "Host panel".
- **Title** (Archivo Black, `clamp(22px, 9vw, 40px)`, line height 1.05, uppercase): the revealed target name and the host's big count ("6 of 8"). These are the moments the eye must land on.
- **Body** (Archivo 400, 16px, line height 1.5): instructions and confirmations. Inputs use 17px so iOS doesn't zoom on focus.
- **Body small** (Archivo 400, 14px): helper copy, errors (500 weight) and the Leave links (500, underlined).
- **Label** (JetBrains Mono 700, 12px, 0.1em letter spacing, uppercase): field labels, the dossier's margin labels (Agent, Room, Rule, Saved), roster group headings and the title kicker.
- **Code** (JetBrains Mono 700, `clamp(28px, 10vw, 40px)`, 0.25em letter spacing, Signal Red): the 4-letter room code.

### Named Rules
**The Typed Label Rule.** Every label, margin title or field name is uppercase mono. Body copy is never set in mono, and mono is never a costume for "technical"; it marks what has been filed.

**The Capitals Are Loud Rule.** Archivo Black appears only in capitals and only for the title, headings, stamps, the revealed name and the host count. Never use it for running text.

## Layout

The page is a single centered column, at most 460px wide, with side gutters of at least 16px that respect safe-area insets. The header sits above `<main>`; each screen is one case-file sheet inside it. There are no breakpoints. Display sizes, the stamp and sheet padding scale with `clamp()`, so the layout holds without sideways scrolling from 195px (200% zoom on a phone) up to desktop, where the column simply floats in the center.

Rhythm runs on a 4px scale: hair 4, tight 8, inline 12, stack 16, group 24, section 32, zone 48. Use tight steps inside a group and generous steps between groups. On the Target screen, regions separate at the section step (32px). Anything destructive sits behind the zone step (48px) and a Rule Line divider.

Reading order follows the task:
- **Home:** fields first, then Join, then Create.
- **Lobby:** the code and the invite link, then status, then Start, then the roster, which comes last because it grows.
- **Target for the host:** the shareable board first, with their own dossier sealed below it.

### Named Rules
**The 48 Rule.** Every interactive control is at least 48px tall, links included. A small visible mark gets its tap height from padding.

**The Leave Zone Rule.** Leave and other irreversible actions live at the bottom, behind a 48px gap and a Rule Line divider, and confirm inline. Cancel comes first and takes focus.

## Elevation & Depth

The system is flat. Depth comes from frame weight (a 2px Night Ink sheet against 1px Rule Line dividers) and from paper tone (a Blank Sheet surface on a Cool Paper ground, with recessed Cool Paper fields). No shadows exist today. A shadow may be introduced only to express a state, such as a pressed or lifted control, and it must have a real offset and a soft blur.

### Named Rules
**The Flat At Rest Rule.** Nothing casts a shadow at rest. A shadow appears only in response to state, never as decoration, never as a zero-offset glow, and never as a hard offset block.

## Shapes

Corners are barely softened: 4px on sheets, buttons, inputs and the reveal box; 3px on tags; 2px on the redaction bar. Nothing is pill-shaped or circular. Frames are solid lines in Night Ink. The reveal box is the one dashed border in the system, a "cut here" edge that turns solid Signal Red while the name is showing. The stamp is the only element that breaks the grid: rotated -4° and bordered 3px in Signal Red.

## Components

Typed and orderly: every component reads like part of a form that's been filled in, labelled and filed.

### Buttons
- **Shape:** 4px corners, at least 48px tall, padding 12px × 16px, bold 16px Archivo.
- **Primary:** a Signal Red fill with On Signal text. Use exactly one per sheet: Join, Start game, or Leave (confirm).
- **Secondary:** transparent with a 1px Night Ink outline and Night Ink text: Create a new room, Copy invite link, Cancel.
- **Link:** an underlined 14px Pencil Gray text button, used only for Leave room and Leave this game. It is still 48px tall.
- **Focus:** a 3px Signal Red outline with a 2px offset (4px on headings that receive focus programmatically).
- **Disabled:** 45% opacity and a not-allowed cursor.
- **Busy:** the label names the operation ("Creating room…", "Joining…", "Sending targets…").

### Case File (sheet)
- **Corner Style:** 4px.
- **Background:** Blank Sheet.
- **Border:** 2px Night Ink.
- **Internal Padding:** `clamp(16px, 6vw, 24px)`, so it narrows at high zoom.
- **Content:** opens with a stamp, then its content grouped on the 4px scale.

### Inputs / Fields
- **Style:** a Cool Paper fill, a 1px Field Edge border, 4px corners, 17px text, a Signal Red caret, and Pencil Gray placeholders.
- **Label:** a mono label above the field, always visible; the placeholder is only an example ("e.g. Indra").
- **Room code variant:** mono, uppercase, 22px, with 0.3em letter spacing.
- **Focus:** a 3px Signal Red outline.
- **Error:** `aria-invalid`, plus a Signal Red error line below the field that is announced to screen readers.

### Stamp (signature)
- Archivo Black capitals in Signal Red, `clamp(11px, 3.9vw, 15px)`, inside a 3px Signal Red border, rotated -4°.
- One per sheet, naming its state: Recruiting (Home), Standby (Lobby), Confidential (Target).
- Hidden from screen readers.
- On the first reveal of a game, the Confidential stamp lands with a 0.35s scale-in ("thunk"). This only happens when the reduced-motion setting is off.

### Redacted Reveal (signature)
- **Hidden:** a dashed box on Cool Paper holding a solid Night Ink redaction bar of fixed width, so it never hints at the name's length, plus a hint line.
- **Showing:** holding shows the name in Title type; releasing hides it. A quick tap shows it for 5 seconds, and tapping again hides it. It also hides after 5 seconds, on app switch and on screen lock.
- **States:** the border turns solid Signal Red while the name shows, and `aria-pressed` reflects the state.

### Dossier Metadata
A two-column grid of uppercase mono labels (Pencil Gray) and plain values: Agent, Room, Rule, Saved on the target sheet; Agents and Status in the Lobby. This is how the system shows facts. Use it instead of chips or stat tiles.

### Sealed Row (host)
- A full-width 56px bar with a 2px Night Ink frame, reading "Your target" in Archivo capitals on the left and a mono Signal Red "Open / Close" on the right.
- It expands to show the host's dossier, and collapses after 30 seconds, on app switch, or on blur.

### Roster and Tags
- Rows are separated by Rule Line, at least 12px apart, with names wrapping anywhere.
- The host roster is grouped under mono headings "Waiting · N" then "Received · N"; received names are in Pencil Gray.
- **Tags:** mono 11px uppercase with a 1px border and 3px corners. "Host" is the only tag, shown in Signal Red. They are not interactive and are never used for status.

### Notes
Blush Note background, 14px text, 4px corners, padding 8px × 12px. They are only for system conditions (test mode, lost connection) and are never used for an ordinary wait.

## Do's and Don'ts

### Do:
- **Do** open every screen's sheet with a stamp that names its state, in Signal Red capitals rotated -4°.
- **Do** set every label, margin title and group heading in uppercase JetBrains Mono at 12px with 0.1em letter spacing.
- **Do** keep every control at least 48px tall, and put irreversible actions behind the 48px leave zone with an inline confirm that puts Cancel first.
- **Do** show facts as dossier metadata (mono label beside a value) rather than as chips, tiles or badges.
- **Do** scale display sizes, the stamp and sheet padding with `clamp()` so the column holds at 200% zoom without sideways scrolling.
- **Do** keep the system flat at rest; if a state needs lift, use an offset, soft-blur shadow for that state only.

### Don't:
- **Don't** show a target name unprompted. Redaction is the default state; a name appears only on an explicit hold or tap and seals itself again.
- **Don't** introduce a second accent hue. Signal Red carries all emphasis, and status is said in words.
- **Don't** use Archivo Black for running text, or mono for body copy.
- **Don't** add decorative shadows, glows, gradients or rounded pill shapes.
- **Don't** outline a control in Rule Line; controls use Field Edge or Night Ink.
