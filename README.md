# IntelliSketch — Online Drawing & Diagram Tool

> UI/UX Design Screens — Figma Prototype

A browser-based drawing and diagramming tool that combines the simplicity of a paint canvas with the power of structured UML diagramming — no installation required.

---

## About This Project

This repository contains the Figma design screens for IntelliSketch, a web-based application concept developed as part of a Software Design & Architecture course. The designs cover the full user journey — from authentication through advanced UML diagramming — and reflect a deliberate design philosophy: **the canvas is the product, everything else serves it.**

These are UI/UX design mockups only. No code or functional implementation is included.

---

## Screens Overview

## Screens

| Screen | Description |
|--------|-------------|
| **Login / Sign Up** | OAuth (Google, GitHub) and email/password auth. Shared card with tab-switch navigation. |
| **Dashboard** | Template gallery and drawing history (Recent, Favorites, Shared). |
| **Canvas — Basic Shapes** | 21-shape searchable panel, dot-grid canvas, right-side Design & Layers panel. |
| **Canvas — UML Activity** | OMG UML 2.x Activity shapes: Action, Decision, Fork, Join, Swimlane, and more. |
| **Canvas — UML Component** | Component, Provided/Required Interface, Dependency, Package, and connectors. |
| **Canvas — UML State Machine** | State, Composite State, Submachine, Initial/Final State, Choice, and more. |
| **Save As** | Backstage-style file panel with OneDrive and local storage locations. |

---

## Design Principles

- **Canvas-first layout** — Panels are collapsible; the drawing area is never compromised
- **Context-aware toolbar** — Controls shift based on what is selected or which library is active
- **Familiar patterns** — Backstage file panel (MS Office), OAuth login (Google/GitHub), dot-grid canvas (Figma/Miro)
- **Zero friction access** — Designed for a browser environment; no install-dependent UI elements

---

## Intended Tech Stack *(for reference)*

| Layer | Technology |
|-------|-----------|
| UI Framework | React.js + TypeScript |
| Canvas Rendering | HTML5 Canvas API + SVG overlay |
| Styling | Tailwind CSS |
| State & Commands | Redux Toolkit |
| Backend | Node.js + Express.js |
| Database | PostgreSQL via Sequelize ORM |
| Auth | JWT + bcrypt + OAuth (Google, GitHub) |
| Cloud Storage | OneDrive API |
| Export | html2canvas + SVG serializer 
