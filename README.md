# Novalon House Studio

**Current Windows release: 0.1.21** · [Versioned release page and downloads](https://github.com/MiMat82/Nova-Home-releases/releases/tag/v0.1.21)

*Release guide refreshed 26 October 2026. The application remains version 0.1.21; this documentation refresh does not change the download.*

**Offline home planning for Windows — draw measured plans, arrange rooms and furniture, explore the building in 3D, and export scaled A3 drawings.**

Novalon House Studio is an independent desktop concept-planning application. It runs locally without an account, subscription or Internet connection. This release adds furniture groups and a more flexible 2D/3D workspace.

[**Download Windows x64 ZIP**](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.21/Novalon-House-Studio-0.1.21-windows-x64.zip) · [**View the example A3 plans**](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.21/10x8-grouped-kitchen-A3.pdf)

## See the application

![Measured two-floor house in the 2D plan and live 3D workspace](https://raw.githubusercontent.com/MiMat82/Nova-Home-releases/main/assets/0.1.21/overview.png)

**Plan and model together.** Select and edit in 2D; the 3D view follows the same measured geometry. The included example is a two-floor, 10 × 8 metre house.

## What's new in 0.1.21

- **Furniture multi-selection:** Shift-click items or use Box select to build a selection.
- **Named furniture groups:** save a kitchen or other arrangement; clicking one member selects the whole group.
- **Shared movement and rotation:** use the centre handle, rotation handle, keyboard nudges or exact Properties values. Rotation uses 15° steps; hold Alt for a free angle.
- **One undo per gesture:** undo a complete move or rotation; Escape cancels an unfinished drag.
- **Group protection:** lock a group or a member to block changes to the entire selection.
- **Coordinated duplication:** copied groups receive new IDs and retain their internal spacing and valid intentional-overlap acknowledgements.
- **Adjustable workspace:** drag the 2D/3D divider; expand Controls when you need person-height and movement settings.

![Furniture selected as a named kitchen group with shared editing handles](https://raw.githubusercontent.com/MiMat82/Nova-Home-releases/main/assets/0.1.21/groups.png)

**Move a complete arrangement.** Select one member of the saved Kitchen group, then move or rotate all six members together. Sizes, spacing and intentional sink/hob overlaps stay coordinated.

## What this release can do

- **Draw measured layouts:** connected straight walls, rectangular rooms, hosted doors/windows, room names, areas, text and dimensions. Supported connected-wall edits update adjoining geometry, rooms and openings together.
- **Work in familiar units:** metres, millimetres or US feet/inches, including fractional input, without changing the stored measurements.
- **Build across floors:** create and duplicate levels; inspect lower-floor guides and place straight, L-shaped or U-shaped stairs with derived slab openings and railings.
- **Shape supported roofs:** rectangular gable, hip, shed and flat roofs; joined gable or flat roofs for supported L/U/T outlines. Supported roof footprints follow exterior-wall edits.
- **Furnish precisely:** place original catalog items, resize and rotate furniture/fixtures, set solid colours, lock objects, create groups and inspect a cross-floor inventory.
- **Align and review placement:** smart wall-face/furniture snapping, live wall gaps, wall-overlap warnings, furniture-overlap review, drawn single-door-swing warnings and user-chosen access spaces.
- **Explore the model:** live 3D, four facade views, measured section cuts, Orbit, rear-avatar and immersive eye-height navigation.
- **Trace local references:** import PNG/JPEG/WebP images, local PDF pages or supported ASCII DXF linework as calibrated passive backgrounds. References guide manual tracing rather than becoming walls automatically.
- **Draw electrical intent:** place generic, Danish or American symbols; draw and reshape coloured cable routes with labels and measured 2D lengths; include a legend in electrical sheets.
- **Compose A3 sets:** combine scaled plan, section and facade views with drawing numbers, titles and revisions. Oversize views are refused instead of silently shrunk; layout review can be appended as separate pages.
- **Save and exchange work:** local `.novahouse` projects, undo/redo, recovery storage, vector PDF/SVG plans, flattened 2D DXF, room-area/inventory CSV and geometry-only OBJ.
- **Review a bounded Denmark profile:** a local layout-review panel explains its supported checks, missing inputs and unassessed cases. It does not certify a building or replace professional review.

## Walk through the building

![Avatar walking on the modeled stair and landing](https://raw.githubusercontent.com/MiMat82/Nova-Home-releases/main/assets/0.1.21/walkthrough.png)

**Explore at person height.** Switch between Avatar view, Walk inside and Orbit. Straight, L-shaped and U-shaped stairs support walking in both directions and automatic floor changes.

## Scaled A3 output

![Measured A3 floor-plan output with dimensions and title information](https://raw.githubusercontent.com/MiMat82/Nova-Home-releases/main/assets/0.1.21/a3.png)

**Export measured drawings.** The supplied PDF contains two A3 landscape floor plans at 1:75. Exported sheets include dimensions, titles, scale information and a 100 mm print-calibration bar.

## Get started

1. Download the **Windows x64 ZIP** above and extract the complete archive into a writable folder. Keep the files inside the **Novalon House Studio** directory together.
2. Run **Open-grouped-kitchen.cmd** from the extracted top-level folder to try the supplied house. To start the app directly, open **Novalon House Studio/Novalon House Studio.exe**.
3. In **2D + 3D**, click a kitchen member to select its saved group. Drag its centre handle to move; drag the round arrow to rotate. Use **Ungroup** before resizing a member individually.
4. To make your own group, Shift-click furniture or use **Box select**, then choose **Group** / **Ctrl+G**. Rename or lock it in Properties; **Ctrl+Shift+G** ungroups.
5. For a new design, use **W** for walls, **R** for a rectangular room, **D/G** for doors/windows, and the object library for furnishings. Select an element to enter exact dimensions in Properties.
6. Choose **Avatar view** or **Walk inside**, click the model, then use **WASD / arrow keys** to move and **Q/E** to turn. Drag the background to look; expand **Controls** for person settings.
7. Save your design as a **.novahouse** file. Configure **A3 sheets** or a **Drawing set**, review the preview and export. Print at **Actual size / 100%** and measure the calibration bar on a physical test sheet.

## How to update safely

Updates are manual: download and extract the complete ZIP for each new version.

- Save every open design as a `.novahouse` file and keep a separate backup before updating. Local recovery is not a project-file backup.
- Close the older app. Download 0.1.21 and extract it into a **new versioned folder**; retain the previous working folder for rollback.
- Run the new executable and open a **copy** of your saved project with **Ctrl+O**. Earlier projects without groups are supported. Review floors, openings, furniture and sheets, then save the updated copy under a new name.
- The example launcher uses its own version-specific local profile. Your existing work may need to be opened explicitly from its saved project file.
- Keep the original project and older executable together for rollback. Backward compatibility of new group metadata with older app versions is not verified.

## Package and verification

- **Target:** portable Windows x64; tested on the development Windows 11 machine. The executable is unsigned.
- **Included:** complete app directory, editable two-floor example, example launcher, quick-start text and two-page A3 PDF.
- **Recorded release checks:** 1,619 automated tests passed; 159 packaged native checks passed; 47 saved synthetic projects checked; three PDFs containing seven A3 pages checked.
- **Release files:** [verification receipt](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.21/VERIFICATION.json), [manifest](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.21/release-manifest.json) and [SHA-256 checksums](https://github.com/MiMat82/Nova-Home-releases/releases/download/v0.1.21/SHA256SUMS.txt).
- **Application source revision:** `079d68bf07203bd09f590c169502a97a093b73a4`. Presentation/documentation updates do not change the packaged application.
- **Windows ZIP SHA-256:** `5decb45a2a6a4fc0b3cb9721df35abb00dd467684066a5c1afd5a361187f332e`.

## Current limits

- Groups are flat furniture/fixture arrangements; nested groups, group scaling and grouping stairs/structural/site/electrical objects are not included.
- The model is for concept planning. It does not provide complete BIM, structural engineering, electrical calculations, automatic code approval, photorealistic rendering or arbitrary roof construction.
- Placement warnings use bounded geometric checks, not a complete accessibility, circulation or detailed-mesh assessment. Electrical routes show planning intent; lengths exclude vertical runs and allowances.
- Physical printing, clean-machine installation and prolonged use remain unverified. PDF scale checks do not establish real-printer calibration.
- **Android APK and iOS IPA builds are not available.** This release contains Windows software only.

## Release archive

[All published versions](https://github.com/MiMat82/Nova-Home-releases/releases). Retain earlier working releases and their matching project backups when updating.

The repository stores small release guides, curated screenshots and verification records. Download the application ZIP from Releases; GitHub's source-code archives are not runnable application packages.
