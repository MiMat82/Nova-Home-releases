# Novalon House Studio

**Current Windows release: 0.1.22** · [Release and downloads](https://github.com/MiMat82/Nova-Home-releases/releases/tag/v0.1.22)

An offline, account-free house-planning application for measured plans, furnished interiors, 3D exploration and A3 drawings. Built and tested for **Windows x64**.

## See the application

![Final 0.1.22 desktop: measured 10 × 8 metre house beside the rear avatar view](https://raw.githubusercontent.com/MiMat82/Nova-Home-releases/v0.1.22/assets/0.1.22/overview.png)

The two-floor synthetic house is open in **2D + 3D**. Select an element in the plan to edit it; use **Orbit**, **Avatar view** or **Walk inside** to inspect the same building.

![Referenced window measurement selected with separate line and label offsets](https://raw.githubusercontent.com/MiMat82/Nova-Home-releases/v0.1.22/assets/0.1.22/dimensions.png)

Select a window, choose **Measure opening width**, then drag its line or text. Properties show the two jamb references and the true measured width while the label moves independently.

![A3 floor-plan preview from the final desktop build with inside chains and product mark](https://raw.githubusercontent.com/MiMat82/Nova-Home-releases/v0.1.22/assets/0.1.22/A3-plan.png)

Open **A3 plan** to inspect inside bedroom chains, exterior measurements and the optional product mark. This example uses **1:75**; export the floor plans or use **Drawing set** for the four saved floor, section and facade sheets.

## What this release can do

- **Measured plans:** connected straight walls, hosted doors/windows, room names and areas, metric or US feet/inches input, referenced or fixed dimensions and text.
- **Floors, roofs and stairs:** multiple levels, lower-floor guides, supported following rectangular/L/U/T roofs and straight/L/U stairs with derived slab openings, handrails and upper guardrails.
- **Furniture:** direct movement, edge resizing, rotation, locks, named groups, smart alignment and a bounded placement review.
- **3D exploration:** Orbit, rear-avatar and immersive eye-height views; articulated walking and automatic floor transitions on supported stairs.
- **Electrical planning:** one catalog with Danish/American symbol choices, editable coloured cable paths and optional A3 legends. Routes represent drawing intent, without electrical engineering calculations.
- **Local references and projects:** calibrated image/PDF/supported ASCII DXF tracing backgrounds; offline .novahouse save/open, undo and local recovery. No account or subscription is required.
- **Drawings:** scaled A3 floor plans and composed plan/section/facade sets, three plan styles, selectable measurement content, dimension text height, line weight and reusable local appearances. Oversize output is refused rather than silently shrunk.

## What's new in 0.1.22

- **Measurements follow named features:** wall axes/faces, opening jambs and supported rectangular-room corners now have explicit references. Inside chains include opening jambs; duplicating a level remaps its references. Older point dimensions remain supported.
- **Direct annotation editing:** drag the dimension line or its text independently, cancel with Escape, and undo a complete gesture once. Manual label position and exact offsets save with the project. A removed host raises **Measurements need review** and stops affected output until reviewed.
- **Cleaner straight-wall editing:** bounded two-wall miters share geometry across plans, 3D and collision checks. **Split at point** and **Trim start/end at crossing** preserve openings and surviving references, with complete undo. Unsafe cuts are refused.
- **Shared A3 appearance:** choose authored/automatic measurements, paper text height and line weight; save/apply named local sheet styles. Applied appearance saves in the project, separately from client/revision metadata. Section markers identify related drawing sheets.
- **Supplied branding applied:** original main mark in the workspace and optional A3 title blocks, original banner in Help, and the approved Windows icon family. Old projects without a branding setting keep unbranded output.
- **Precision shortcut fix:** Windows Alt menu activation no longer interrupts precision dragging; the app retains its toolbar and editing shortcuts.

This follows [0.1.21](https://github.com/MiMat82/Nova-Home-releases/releases/tag/v0.1.21), which introduced furniture groups and adjustable workspace controls.

## Get started

1. Download [Novalon-House-Studio-0.1.22-windows-x64.zip](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.22/Novalon-House-Studio-0.1.22-windows-x64.zip) and extract the **complete** archive into its own folder. Keep the executable's neighboring files together.
2. Run **Open-precision-house.cmd** for the finished two-floor 10 × 8 m example. Alternatively, start **Novalon House Studio.exe** in the **Novalon House Studio** folder and open a saved project with Ctrl+O.
3. In **2D plan**, select a window → **Measure opening width**. Select Bedroom in the room list → **Add inside measurement chains**. Drag a dimension line, then drag its label; change the window width to see the reference update.
4. Select a wall → **Measure centreline**, **Measure left face** or **Measure right face**. For a cut, choose **Split at point** and click outside openings; for a trim, choose the end and click a crossing wall. Use Undo to restore the complete edit.
5. In **A3 plan**, set **Dimension text height / paper mm**, **Drawing line weight**, **Measurements on plan** and **Product logo on A3 sheets**. Enter a **Sheet style name**, then **Save current sheet style**. Applied appearance saves with the project; the named style library stays on this computer.
6. Use **Save project** for a .novahouse file. **Export all levels** writes the two floor pages; **Drawing set** → **Export complete A3 drawing set** writes the four saved sheets. Print at **100% / Actual size** and measure the floor-sheet 100 mm calibration bar on a test print.

## How to update safely

1. In the old app, save each design to a .novahouse file and make an independent backup. A recovered draft in a local profile is not a project-file backup.
2. Close the old app. Extract the new Windows ZIP into a separate versioned folder; retain the previous working release and its files for rollback.
3. Start the new app and open a **copy** of a saved project. Inspect its 2D plan, 3D model and A3 output, then save under a new filename.
4. All **48 synthetic saved examples** passed current validation and semantic save/reload. The **47 prior examples** were hash-checked unchanged. Older releases are not promised to understand new measurement-reference or appearance fields; keep the original project backup for rollback.

Updating is **manual**; there is no automatic updater or cloud synchronization. The bundled example launcher uses a separate local profile for this version and does not transfer an older example's recovered draft. Named sheet styles and workspace preferences are local to the profile.

## Included downloads and verification

- **Windows x64 portable ZIP:** complete application, dependency notices, example launcher, .novahouse house and both A3 PDFs.
- [10x8-floor-plans-A3.pdf](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.22/10x8-floor-plans-A3.pdf): **2 A3 landscape pages at 1:75**.
- [10x8-drawing-set-A3.pdf](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.22/10x8-drawing-set-A3.pdf): **4 A3 landscape pages at 1:75**: ground, upper, section A-A and north facade.
- [VERIFICATION.json](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.22/VERIFICATION.json): sanitized verification receipt.
- [release-manifest.json](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.22/release-manifest.json) and [SHA256SUMS.txt](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.22/SHA256SUMS.txt): asset sizes, source revision and SHA-256 values.
- **Package source commit:** `282e8f008432f82e826ef7831f2b0d05562c5d2e`. Later guide-only commits do not change the binary's source identity.
- **Verified on Windows 11 x64:** **1,661 automated tests**, **24 release-guide tests**, **176 packaged desktop checks**, **48 saved projects**, and **7 PDFs / 19 A3 pages**. The bundled plans were compared with exports from the exact final package: matching text, images and drawing operators within 0.0000001 PDF point numeric tolerance.
- **Preservation:** 27 prior package/example artifacts and all 47 prior saved examples remained unchanged. The application made no remote requests during the packaged native exercises.

SHA-256 checksums:

```text
11b81378a4603bfe78b23fac1cda4f888082474e7c79b38d2e5ba62d5b2101c1  Novalon-House-Studio-0.1.22-windows-x64.zip
23c7c00a4c20e3c83203ec32072079878a899ad43108fdbc861d0d95eb43cfb1  10x8-floor-plans-A3.pdf
7c3e24078dcc4c021f70d92d0240a1493da07014514f7ad25ffd46dc4c595ea3  10x8-drawing-set-A3.pdf
c08cec98fb2196ad5309a3b576ea7ceb391e2b419346e439ba441dd276fcbe22  VERIFICATION.json
```

## Current limits

- Concept planning, rather than certified BIM, permit documents or complete regulatory/electrical compliance. The offline Denmark review covers only its explicitly listed checks.
- Wall joins are bounded two-wall miters, with conservative butt geometry at unsupported junctions. Split/trim use straight walls and actual bounded crossings; trim does not extend a wall. Inside chains require axis-aligned rectangular rooms, including collinear partition vertices. Dimensions measure geometry; they do not drive it.
- Dense drawings and manual text placements need review. The logo is an optional raster image; drawing geometry remains vector. Standard PDF fonts substitute unsupported characters. Styles are local preferences, without cross-computer synchronization.
- Native checks use synthetic projects and programmed file-dialog responses. Physical A3 printing, clean-machine installation and long-duration operation are unverified. Verify paper scale on a physical print.
- The Windows package is **unsigned**. **Android APK and iOS IPA builds are not implemented or included.**
