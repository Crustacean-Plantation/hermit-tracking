# Problem brief

Status: open. Field result so far: tags ping along streets. We do not yet have a fix that shows where the crab is when the nearest Apple device is on the road.

## Species and place

- Species: *Coenobita clypeatus*, Purple Pincher. Only land hermit crab in the Florida Keys.
- Place: Upper Keys, around Tavernier, including yard habitat near Harry Harris Park and nearby transfer stations.
- Behavior that matters: nocturnal, walks between cover and the coast, changes shells as it grows, can drop a shell and leave a mount behind.

## What the current map shows

Points line up with streets. That matches Find My's design. The report is the finder's position, not a GPS fix from the tag. Wi-Fi near the crab does not locate the tag. A phone on the road with Find My enabled does.

Useful fields to store, if a logger is built:

- tag id (opaque, not a street address)
- timestamp of the report
- latitude and longitude of the report
- horizontal accuracy radius
- battery state if the cache provides it

Do not store owner names, Apple IDs, or precise home coordinates in this repository.

## Constraints

| Constraint | Why it matters |
| --- | --- |
| A few grams, not 11 | AirTag weight is too much for a small crab |
| Salt, rain, heat | Keys weather |
| Jettison by shell change | Crab must be able to leave the device |
| No live public map | Protect the animals and the sites |
| No handling for repo tests | Field protocol stays with the existing tracking project |

## Success looks like

Either an honest map: circles, gaps, and a label that a point was heard from the road.

Or a design someone can build: weight, battery life, how the fix is recovered, and how the crab takes it off.

A pull request that only redraws the same roadside points as a line is not a solution.
