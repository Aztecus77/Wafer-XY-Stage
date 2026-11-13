# Wafer XY Stage

A standalone XY wafer positioning platform with computer control for the SPICE student lithography project at VUT FEKT.

**Status:** requirements and construction proposal under development. The technical assignment is draft v0.6; SPICE review and approval are pending. No completed platform or measured positioning performance is claimed.

## Project Documents

- [Technical assignment](docs/technical-assignment.md)
- [Proposed purchase list](hardware/purchase-list.md)
- [Mechanical concept — SVG](hardware/concept/wafer-xy-stage-labeled-en.svg)
- [Mechanical concept — PNG](hardware/concept/wafer-xy-stage-labeled-en.png)
- [Wafer motion-envelope sketch](hardware/figures/wafer-motion-envelope-user-sketch-2026-11-13.png)
- [Computer-side software](software/README.md)
- [Controller firmware](firmware/README.md)

## Current Scope

- Standalone device used with the lithography system.
- Initial control from a computer.
- Wafer diameter up to 100 mm, with wafer fragments also expected.
- Useful X and Y travel of 100 mm each, corresponding to centre displacement from -50 to +50 mm on each axis.
- Initial wafer fixation using double-sided adhesive tape.

The approximately 1-micrometre positioning-error target is provisional and subject to review and measurement. Other performance requirements and the lithograph interface remain to be agreed. Z motion, local controls, automatic stitching and multilayer alignment have not been adopted as initial implementation requirements.

## Working with Changes

`main` holds the current shared project state, including clearly marked drafts. Use a separate branch for a particular change, such as a requirements revision, component review or software feature, then review and merge it into `main`.

Keep documents in English. Maintain the technical assignment as one file; Git records revisions. Documentation milestones can later be marked with tags such as `docs-v0.6` and `docs-v1.0`.
