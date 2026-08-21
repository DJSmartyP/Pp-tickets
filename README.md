# Can I Buy Phantom Peak Tickets Yet?

GitHub Pages-ready responsive ticket checker.

## How it works

The page uses two fixed master artworks:
- `Assets/booth-landscape.*` for landscape screens
- `Assets/booth-portrait.*` for portrait screens

HTML overlays only the live `NO`, `MAYBE`, or `YES` state into the blank parchment area, while the six countdown cards are fully live below the artwork.

## Main state

- Before 09:30 BST: **NO**
- 09:30–12:29 BST: **MAYBE**
  - Depends on whether you're in the Guild or on the waitlist.
  - Check the bar below for your specific ticket time.
- From 12:30 BST: **YES**

## Ticket windows — Monday 24 August 2026

- 09:30 — Guild Chroniclers with Ticket Packs
- 09:50 — Guild Chroniclers
- 09:55 — Guild Members
- 10:00 — Guild Initiates
- 11:00 — Early Waitlist
- 12:30 — Everyone Else

## GitHub Pages

Upload the contents of this ZIP to the root of the repository. Keep the `Assets` folder capitalised exactly as supplied.

The page is responsive:
- Landscape: hero + one-row six-slot access bar
- Portrait/tablet/mobile: portrait hero + 2×3 countdown grid
- Very narrow phones: countdowns switch to a single column


## Hidden test menu

Click the first **O** in the large `JONABOT` booth sign to reveal a hidden test menu.

- `AUTO` — uses the real ticket schedule
- `NO` — previews the NO state
- `MAYBE` — previews the MAYBE state and explanation
- `YES` — previews the YES state

The test menu changes only the main state display. The access countdowns continue to show the real live schedule.


## Open-state behaviour

When an access window reaches zero:
- that card gets a stronger green open-state treatment;
- the countdown disappears;
- it is replaced by a large Western-style **ACCESS OPEN** stamp;
- the original category border colour is retained.


## Access-window test controls

The hidden JONABOT menu now also includes an **Access windows** test row.

- `AUTO` — real live countdown behaviour
- `09:30` — previews the page immediately after the first access window opens
- `09:50` — first two windows are open
- `09:55` — first three windows are open
- `10:00` — first four windows are open
- `11:00` — first five windows are open
- `12:30` — all six windows are open

The main-sign test and access-window test work independently, so any combination can be previewed.


## Simplified hidden test menu

The hidden menu now has one set of preview times only:

- `AUTO`
- `09:30`
- `09:50`
- `09:55`
- `10:00`
- `11:00`
- `12:30`

Selecting a preview time drives the entire page from that simulated time. It updates both:
- the main `NO / MAYBE / YES` sign;
- which access cards have reached `ACCESS OPEN`.

`AUTO` returns the page to the real live clock.

- `CLOSED` previews the page immediately before 09:30: main sign **NO**, with all six access windows still counting down/closed.
