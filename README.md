# Intentional Focus
A distraction-free focus timer that helps you enter deep work states
through intention-setting, ambient themes, and a minimal session
environment — not just a countdown clock.

Live demo: https://m-chhay.github.io/pomodoro/

Best experienced on desktop.

---

## What it does

Users set an intention before each session, choose a duration, and
enter a focused environment designed to reduce cognitive friction.
The app structures each session across three phases:

- **Setup** — type what you're working on (required to start), pick
  a focus duration (15, 25, 45 min, or custom), set a break length,
  and choose an ambient theme
- **Focus session** — full-screen minimal view showing your intention,
  a circular countdown ring, and pause/end controls. The ring fills
  as the session progresses, color-matched to your theme
- **Break** — a separate, quieter countdown screen after each session,
  with the option to skip directly to a new session

A soft four-note chime plays when each session completes.

---

## Themes

Four ambient background themes, each with slow-drifting gradient
blobs and a matching ring accent color:

- **Sunset** — warm oranges, pinks, deep reds
- **Ice** — cool blues, cyan, light aqua
- **Deep** — dark indigo, navy, near-black
- **Forest** — muted greens, teal, dark sage

A motion toggle in the top-right corner lets users disable the
animated background and fall back to a static gradient — useful
for reducing distraction or saving battery.

---

## Why I built this

Most productivity timers treat focus as a mechanical problem: set
a number, start the clock, done. But the harder part is the
transition into focus — deciding what matters, removing visual
noise, and building a small ritual around the work.

This project is an attempt to design that transition intentionally.
The intention field isn't optional. The environment reacts to your
mood. The goal is to make starting feel deliberate rather than
arbitrary.

---

## Tech stack

Single-file HTML/CSS/JS — no build system, no dependencies, works
offline. Animated backgrounds built with CSS keyframe animations
and SVG radial gradients. Circular progress ring rendered with SVG
`stroke-dashoffset`. Completion chime generated with the Web Audio
API — no audio files required.
