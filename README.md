# Engineering Simulation Plugins (Industry Project)

This repository documents the architecture and functionality of two plugins
developed during a Software Engineering Internship to extend an engineering
simulation platform.

The original system integrates with proprietary simulation software; this
repository focuses on design, behavior, and engineering decisions rather than
full reproducibility.

---

## Overview

The goal of this work was to improve how engineers analyze and report simulation
results by providing:
- Interactive visualization tools
- Automated, customizable report generation

Both plugins were designed to integrate cleanly with an existing application
while remaining modular and extensible.

---

## Plugin 1: Interactive Charting Tool

An interactive charting application built using **ScottPlot** and **WinForms**
in **C# (.NET)**.

### Key Features
- Multi-series plotting of simulation data
- Per-series simulation and playback by element index
- Runtime series visibility toggling
- Dynamic color customization
- Interactive series selection with a real-time tracking marker that follows
  the selected data series
- Point insertion and manual data annotation

### Engineering Focus
- Coordinating UI events with plot state
- Managing dynamic updates without re-rendering entire plots
- Maintaining responsiveness for large datasets
- Clear separation between data, visualization logic, and UI controls

---

## Plugin 2: Modular PDF Report Generator

A report-generation plugin built using **QuestPDF**, designed to produce
structured simulation reports directly from user-selected elements in the host
application.

### Key Features
- Modular report composition (tables, images, notes)
- Configurable layout (portrait / landscape)
- Dynamic inclusion of simulation artifacts
- Clean, extensible document pipeline

### Engineering Focus
- Strong separation of concerns between data selection, layout, and rendering
- Reusable document components
- Maintainable architecture to support future report types

---

## Technologies Used
- C#
- .NET
- WinForms (UI)
- ScottPlot (interactive visualization)
- QuestPDF (document generation)

---

## My Contributions
- Designed and implemented both plugins end-to-end
- Owned architecture and software design decisions
- Built interactive UI behavior and plotting logic
- Developed a modular PDF generation system
- Collaborated with engineers to refine APIs and workflows

---

## Developer Enablement

In addition to implementing the plugins, I created internal documentation and a
step-by-step tutorial to help future developers build new plugins using the
framework.

The tutorial covered:
- Plugin lifecycle and interfaces
- Recommended project structure
- Common extension points
- Best practices for visualization and reporting plugins

This documentation was used to onboard additional developers and ensure
consistent plugin design.

---

## Demonstrations

Short demo and tutorial videos are available in
[`videos.md`](videos.md).

---

## Notes

This repository emphasizes architecture and behavior over full execution.
Integration with proprietary simulation software is intentionally omitted.
