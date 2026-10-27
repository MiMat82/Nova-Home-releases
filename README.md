# Novalon House Studio

**Current Windows release: 0.1.23** · [Release and downloads](https://github.com/MiMat82/Nova-Home-releases/releases/tag/v0.1.23)

An offline, account-free Windows x64 house planner with measured layouts, 3D exploration and coordinated A3 drawings. This release adds persistent opening tags and linked door/window schedules.

## See the application

![Final 0.1.23 desktop with persistent door/window tags beside the 3D avatar view](https://raw.githubusercontent.com/MiMat82/Nova-Home-releases/v0.1.23/assets/0.1.23/overview.png)

The finished two-floor 10 × 8 metre house is open in **2D + 3D**. Tags identify the original openings. Choose **Doors & windows** to inspect their linked schedules.

![A window schedule row and its measured opening editor in the final build](https://raw.githubusercontent.com/MiMat82/Nova-Home-releases/v0.1.23/assets/0.1.23/linked-schedule.png)

Click a tag under **Tag / edit** to change the original opening's size or specification. This example shows W-101 at **2.10 m** wide, with its Danish note retained. **Show in plan** selects the same object beside 3D; review notes remain visible for incomplete rows.

![A3 door schedule exported from the exact final package with tags, room sides, dimensions and quantities](https://raw.githubusercontent.com/MiMat82/Nova-Home-releases/v0.1.23/assets/0.1.23/A3-schedule.png)

The saved **A-401** table lists the five example doors. Opening dimensions and declared clear passage occupy separate columns. Use **Drawing set** to export plans, sections, facades and schedules together; larger tables create continuation pages with repeated headers.

## What this release can do

- **Draw and edit measured houses:** connected straight walls, hosted doors/windows, room areas and referenced dimensions, with metres/millimetres or US feet/inches input.
- **Coordinate a building:** multiple levels, supported following roofs, straight/L/U stairs with derived slab openings and rails, furniture groups, placement review, rear-avatar and immersive views.
- **Identify and schedule openings:** persistent project-wide tags, live dimensions, sill heights, quantities, specification notes and explicit room-side/passage declarations.
- **Export drawings and data:** scaled A3 floor plans and composed drawing sets, paginated schedule tables and protected Unicode CSV. Drawing geometry and table text remain vector; the optional product mark is raster.
- **Work locally:** .novahouse save/open, undo/redo, local recovery and local reference import. The application runs offline without an account, subscription or cloud database.

## What's new in 0.1.23

- **Stable visible tags:** D01/D02 and W01/W02 are saved on openings. **Assign missing tags** upgrades older projects explicitly. New openings get marks automatically; deleted objects do not renumber survivors. Copied floors get fresh tags and remapped chosen room references.
- **Linked schedule editing:** click a row's tag to edit opening dimensions, sill, specifications, custom tag or declared passage. **Show in plan** selects that original object in 2D + 3D. Geometry, measurements and schedules share one validated transaction and normal undo/redo.
- **Room-side review:** A/B mean left/right of the host wall from start to end. Reversing a swing does not swap them. Missing or ambiguous detected rooms need review; **Outside** is an explicit declaration. Stale or inconsistent choices remain visible after edits.
- **Schedule quality checks:** missing/duplicate tags block affected schedule export. Other incomplete specifications and associations stay visible as review notes in the table, PDF and CSV. Opening width is never substituted for declared clear passage.
- **A3 schedule sheets:** standalone tables or saved drawing-set schedules, level/kind filters, measured text wrapping, repeated headers and automatic continuation pages. Each opening counts once in totals. Schedule sizes are labelled data, not scaled drawings.

This follows [0.1.22](https://github.com/MiMat82/Nova-Home-releases/releases/tag/v0.1.22), which added referenced dimensions, straight-wall split/trim, bounded joins and shared A3 styles. Those workflows remain available.

## Get started

1. Download [Novalon-House-Studio-0.1.23-windows-x64.zip](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.23/Novalon-House-Studio-0.1.23-windows-x64.zip) and extract the **complete archive** into a separate folder. Keep the executable's neighboring files together.
2. Run **Open-tagged-house.cmd** for the two-floor 10 × 8 m example. Alternatively, start **Novalon House Studio.exe** inside the **Novalon House Studio** folder and open your .novahouse file with Ctrl+O.
3. Choose **Doors & windows**. For an older file choose **Assign missing tags**. Filter by level or by doors/windows; click a tag under **Tag / edit**.
4. Change **Schedule opening width**, height, sill or specification. Lengths use the project's units. **Show in plan** highlights the same opening beside 3D. Undo restores an edit; **Save project** preserves the model and schedule metadata.
5. Confirm room associations where needed. **Room A** is left of the wall start-to-end direction; **Room B** is right. Choose automatic detection, a room or **Outside · declared**. A door's clear passage is an independent declaration.
6. Choose **Export A3 schedule** or **Export opening CSV** for the selected level/kind. **Only reviews** is a table-inspection filter; exports include all rows in the selected level/kind.
7. Choose **Add schedule to drawing set**, then select the saved sheet in **Drawing set**. Set its name, number, revision, orientation or filter. **Schedule continuation page** previews each page. **Export complete A3 drawing set** includes model views and schedules together.

The example contains two floor-plan pages, two schedule pages and a six-page coordinated set. Model views use **1:75**; tables are **not to scale**. Print plans at **100% / Actual size** and measure a 100 mm calibration bar on a physical test print.

## How to update safely

1. In the old app, save designs to .novahouse files and make an independent backup. Local recovery is not a project-file backup.
2. Close the old app. Extract the complete new package into a separate versioned folder; keep the previous working release and original projects for rollback.
3. Open a **copy** of your saved project in the new app. Older files are loaded without rewriting their geometry or assigning tags automatically; **Assign missing tags** is an explicit edit.
4. Inspect 2D, 3D and A3 output, then save under a new filename. **49 synthetic projects** passed current validation/save-reload; all **48 prior examples** remained unchanged. Older apps are not promised to preserve or interpret the new opening metadata and schedule definitions.

Updating is **manual**. There is no automatic updater or cloud synchronization. The example launcher uses a separate local profile for this version; save an older recovered draft to a project file before switching. Local styles/preferences stay in their profile.

## Included downloads and verification

- **Windows x64 ZIP:** complete application, dependency notices, launcher, tagged project and the three PDFs below.
- [10x8-tagged-plans-A3.pdf](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.23/10x8-tagged-plans-A3.pdf): **2 A3 landscape floor plans at 1:75**.
- [10x8-opening-schedules-A3.pdf](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.23/10x8-opening-schedules-A3.pdf): **2 A3 tables**, five doors and five windows.
- [10x8-coordinated-set-A3.pdf](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.23/10x8-coordinated-set-A3.pdf): **6 A3 sheets**, including both schedules.
- [VERIFICATION.json](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.23/VERIFICATION.json), [release-manifest.json](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.23/release-manifest.json) and [SHA256SUMS.txt](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.23/SHA256SUMS.txt): sanitized evidence, package identity and asset checksums.
- **Package source commit:** `30957c263030f542caa5757e337f2da7910d46b5`. Later documentation commits do not change the binary's source identity.
- **Verified on Windows 11 x64:** **1,679 automated tests**, **24 release-guide tests**, **99 packaged desktop checks**, **49 saved projects**, and **11 PDFs / 35 A3 pages**. Native checks include linked schedules, validation/undo, save/reopen, pagination and precision/placement regressions.
- **Pagination:** all 75 window tags appeared exactly once across a four-page test schedule, with repeated headers and correct totals. Bundled floor plans and the six-page set match exact-package exports in text, images and drawing operators within 0.0000001 PDF point numeric tolerance.
- **Preservation/offline:** 34 prior package/example artifacts and all 48 prior saved examples remained unchanged. No remote requests occurred during the packaged desktop exercises.

SHA-256 checksums:

```text
e8bc851fd99790b1d570edeb88b5271e5e9501b10bd467b9e798c00f132c30ae  Novalon-House-Studio-0.1.23-windows-x64.zip
57f38fec1ece8b9499ce08c514c11203759659160e08654f86031dc4d6a4a47a  10x8-tagged-plans-A3.pdf
bd200bc8f9d50144432075efa6735aef7491b8c435508b825f1fac2f0e79d95e  10x8-opening-schedules-A3.pdf
772fb2d4da76ed44f003a5ff225a965b068c0fa89cdf909858895416a1ce07a9  10x8-coordinated-set-A3.pdf
10ed2dae09bdceec5681ec297213c3a9bee5b1f3153c403265eac53b192a9d00  VERIFICATION.json
```

## Current limits

- Concept planning; not certified BIM, supplier approval, permit documentation or complete regulatory compliance. Specifications and clear passage are user declarations. The offline Denmark review covers only its explicitly listed checks.
- Room associations rely on current modeled room polygons and bounded sampling. Verify unusual junctions, missing room boundaries and manual declarations. Dense plan tags may need their model offsets adjusted in Properties.
- One schedule row represents one placed opening; no supplier pricing, material takeoff, type catalog or procurement integration is included. A schedule/complete drawing-set export is capped at 256 pages. Narrow filters or export fewer sheets for larger projects.
- Standard PDF fonts substitute unsupported characters; arbitrary Unicode typography is not implemented. CSV retains Unicode and neutralizes spreadsheet formula prefixes in user text.
- Native checks use synthetic projects and programmed file-dialog choices. Physical A3 printing, clean-machine deployment and long-duration operation remain unverified. The Windows package is **unsigned**. **APK and IPA builds are not implemented or included.**
