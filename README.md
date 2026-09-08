# Stop Re-Explaining Yourself

An HTML presentation for a bi-weekly AI accountability group: a live Claude Cowork demo
built around a real interview-prep workflow.

**Live deck:** https://caesarb-34.github.io/cowork-demo-deck/

## Presenting

| Key | Action |
| --- | --- |
| `→` `space` `PageDown` | Next slide |
| `←` `PageUp` | Previous slide |
| `N` | Toggle speaker notes |
| `D` | Toggle dark / light |
| `F` | Fullscreen |
| `Home` / `End` | First / last slide |

The theme choice is remembered in the browser. The URL hash tracks the slide, so
`#7` opens straight to slide 7 — useful if you need to rejoin mid-session.

Speaker notes carry the run of show, the exact demo prompts in order, and what to say
while Claude is working. They are visible only to whoever presses `N` on their own screen.

## Editing

Everything is in `index.html` — one file, no build step, no dependencies.
Each slide is a `<section class="slide">`; its notes are the `<script type="text/plain" class="note">`
block inside it. Add a slide by copying a section; the counter and navigation pick it up automatically.

Colors live in the two `:root` blocks at the top of the stylesheet — light first, then
`[data-theme="dark"]`. Change a token in both places and it propagates through the deck.

## Also in this session

A PowerPoint version of the same 14 slides exists separately, with the same speaker notes.
Use that one if you need to hand the file to someone who wants to edit it in PowerPoint.
