![audio, thing](./res/logo.png)

# AudioThings

<div style="display: flex; flex-direction: row;">
<img src="https://github.com/velvia-fifty/AudioThings/actions/workflows/jekyll-gh-pages.yml/badge.svg"> &nbsp;&nbsp;
<img src="https://img.shields.io/website?url=https%3A%2F%2Fgithub.com%2Fvelvia-fifty%2FAudioThings%2F"> &nbsp;&nbsp; <img src="https://img.shields.io/github/commit-activity/t/velvia-fifty/AudioThings"> &nbsp;&nbsp; <img src="https://img.shields.io/github/repo-size/velvia-fifty/AudioThings?style=flat&label=girth">
</div>


<sup>*I made this for me, maybe you find it helpful?*</sup>

>What is the meaning of life? Are we here only to eat hot chip, shitpost, and make the robot have orgasm?
>
>**No!**
>
>*We do audio, we do thing, we do audio things!*

## Getting the most out of your trip to Cleveland Ohio

When you download this as a ZIP open AudioThings.kicad_pro, this is a panopticon project that contains the main resources and exists to handle some references that are common. Use Kicad to drill down into other projects.

Or don't, I'm not a cop.

## Navigating this hot mess of a repo

This repo is poorly organized and so am I, here are the main non-project folders.

- [Art](./Art/)
  - Less-than-practical boards that are incomplete.
- [CRIB SHEET](./CRIB%20SHEET/)
  - Things I ~stole~ used for inspiration.
- [docs](./docs/)
  - Audio Things: The Manual: The Webpage: The Source
- [Modules](./Modules/)
  - The stuff that's mostly complete
- [OLD](./OLD/)
  - The trashcan, I sometimes use this to store things
- [res](./res/)
  - Central resource folder containing footprints, 3d models, and other assets.
  - Referenced at ${KIPROJMOD}/../../res/
- [Tools](./Tools/)
  - Hammers, Templates, etc.
- [Workshop](./Workshop/)
  - Half-baked and half-finished boards

### Project Resources

Footprint Library
${KIPRJMOD}/../../res/AT-Footprints.pretty

## I have opinions and they're loud

Opinions are for suckers, we're a big girl, we have convictions (and they're obtuse).

### Maximize Cheap

If we wanted to spend money, we wouldn't pay with our time!

- Boards stay within 100mm x 100mm to get the cheapest per-board costs for small orders
- BOM includes actively produced parts unless there are no other options
- Rely on someone else's scale and use the most common solution in the wrong way

See: [Fab Min-Max Notes](./FAB_NOTES.MD)

### Form Factor Agnostic

- Assume Eurorack
- Assume Backplane
- Assume Stacking
- Assume Standalone

### Your Licensing Model is Bad and You Should Feel Bad

- All work is under copyright, this is not public domain
- Its licensed to you under [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/)
- If you're not an individual, the words "copyright" and "NonCommercial" are very important.

For how I really feel, see: [LICENSE.MD](./LICENSE.MD)

## Core Features

- Eurorack Compatible
- Backplane preferred but optional
- Daughterboards are assumed (Minium PCB order is 5 after all)

# I took notes here, don't look

m.2
<https://github.com/timonsku/M.2-Card-Footprints/tree/main>

# Universal Faceplate

Universal 6mm opening for jacks and pots

11.5mm between board and face

SJ3-350103A 3.5mm Stereo
<https://www.digikey.com/en/products/detail/same-sky-formerly-cui-devices/SJ3-350103A/24627980>

PTV09 Pots
<https://www.bourns.com/docs/Product-Datasheets/PTV09.pdf>
