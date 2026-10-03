# Hermit tracking

Open problem from [Crustacean Plantation Inc.](https://www.crustaceanplantation.org), a Florida Keys 501(c)(3) conserving wild land hermit crabs.

**The map is following the road, not the crab.** We need a way to record where *Coenobita clypeatus* (Purple Pinchers) actually go, or an honest picture of how wrong the current dots are.

This repository is a problem statement and a call for help. It is not a finished tracker.

## What we are trying to learn

Native Purple Pinchers in the Florida Keys are not born with shells. They spend adult life on land near water, and they can live 40 years or more. Shells returned to the wild are marked and placed at transfer stations. The missing piece is movement: how far a crab goes after it takes a shell, whether it stays in the yard or crosses to the mangroves, and whether a roadside pin is the animal or the phone that heard the tag.

Partner work already underway: Emma Palazzo / Tattered Rat's Crafts, [Hermit Crab Tracking Project](https://tatteredratscrafts.square.site/hermit-crab-tracking-project). Crabs in that study are not handled. Do not repeat field work without that kind of help.

## Why AirTag trails hug the street

An AirTag has no GPS and no Wi-Fi radio. It broadcasts a Bluetooth beacon. The dot on a Find My map is the location of the Apple device that heard the beacon, plus that phone's own accuracy radius.

In the Upper Keys, Apple devices are mostly in cars and on shoulders. A crab 30 meters into the mangroves can be plotted on the pavement. A single network report is often only good to about 50–100 meters. If no Apple device passes, there is no new point. Busy roads update. Empty habitat does not.

Dog-tracking repos such as [trackmyairtag](https://github.com/trackmyairtag/trackmyairtag) and [findmy-api](https://github.com/zyx1121/findmy-api) scrape the Find My cache on a Mac and draw the trail. They do not remove the roadside bias. Apple does not offer a public Find My API.

AirTags also alert nearby iPhones and can play a sound if they travel away from the owner. That is a poor fit for an animal left in the field. An AirTag is about 11 grams. A small Purple Pincher will not carry it, and a crab that changes shells leaves the tag behind.

## Two tracks

**A. Make the tags we already have honest.** Log every report with time and accuracy. Draw the circle, not a fake precise pin. Drop points that jump to a road and snap back. Label a roadside ping as "heard from this road."

**B. Use a different instrument.** Weight has to stay low enough for a shell, the mount has to survive salt and rain, and the crab has to be able to abandon it by changing shells. Candidates: a recoverable GPS logger at a transfer station, a VHF ping walked with a receiver, marked shells plus camera traps. A 2025 harness study on *Coenobita* showed a payload the crab can jettison by switching shells ([RSC Advances](https://doi.org/10.1039/d5ra03509k)).

## What we will not do

- Glue or permanently attach anything to a crab.
- Publish live or precise locations of wild animals.
- Handle crabs for this repo's experiments. Field work stays with people already doing it carefully.
- Ask anyone to break Apple's terms or bypass anti-stalking alerts.

Raw points stay off this public repo. Methods and blurred tracks are fine.

## How to help

Open issues are the ask. Start here:

1. Log Find My reports with the accuracy radius.
2. Filter roadside bias on a map.
3. Propose a tag under a few grams.
4. Design a shell mount the crab can leave.

Read [docs/problem.md](docs/problem.md) before opening a pull request.

## Organization

Crustacean Plantation® is a registered mark, USPTO registration 8194307. Motto: Leave the Shell, Take the Memory. Site: [crustaceanplantation.org](https://www.crustaceanplantation.org). Address for shell donations, not for hardware: 200 Canal Street, Tavernier, FL 33070.
