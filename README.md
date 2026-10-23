# Tote Math

Event market peach tote, week, cost and time arithmetic. The 262 peaches at 6 peaches a tote take 44 totes, the last tote holding 4 peaches.

## Named constants

None. Every number is the owner's own entry.

## What it computes

- **The totes truth** - the peaches (1 to 1000000) divided by the peaches a tote (1 to 1000), rounded up, with what the last tote holds.
- **The weeks truth** - the peaches divided by the peaches used a week (1 to 100000), with the peaches left for the next week.
- **The cost truth** - the totes (1 to 100000) times the tote price ($0.01 to $999.99) to the cent, and spread over the peaches, half rounded up.
- **The time truth** - the peaches divided by the peaches packed a minute (1 to 100), rounded up, in minutes and in hours and minutes.

## Boundary

Arithmetic only. Counting applied as written. It has not seen any peach, tote or venue and does not know whether peaches will really stay fresh, a supplier will run out or a price will hold, and it gives no verdict that a tote is worth its price or a peach is right for an event. Every number is the owner's own entry.

## Files

- `index.html` - landing page with the boundary and starting examples.
- `app.html` - the calculator; every tote recomputes on each keystroke.
- `engine.js` - the four truths, shared by the page and the tests.
- `oracle.py` - an independent Python re-implementation; writes `expected.json`.
- `test.js` - runs the engine against `expected.json` (99 cases, 20 error cases).

## Tests

```
python3 oracle.py
node test.js
```
