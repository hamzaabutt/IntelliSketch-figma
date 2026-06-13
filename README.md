# IntelliSketch — Online Drawing & Diagram Tool

> UI/UX Design Screens — Figma Prototype

A browser-based drawing and diagramming tool that combines the simplicity of a paint canvas with the power of structured UML diagramming — no installation required.

---

## About This Project

This repository contains the Figma design screens for IntelliSketch, a web-based application concept developed as part of a Software Design & Architecture course. The designs cover the full user journey — from authentication through advanced UML diagramming — and reflect a deliberate design philosophy: **the canvas is the product, everything else serves it.**

These are UI/UX design mockups only. No code or functional implementation is included.

---

## Screens Overview

### Authentication

| Screen | Description |
|--------|-------------|
| **Login** | Centered card with OAuth (Google & GitHub) and email/password login. Full-width primary CTA button with purple gradient. |
| **Sign Up** | Extends the login card with Full Name and Confirm Password fields. Terms of Service checkbox gates the primary action. |

Both screens share the same card container with a tab-switch component for seamless transitions between login and registration.

---

### Dashboard

A post-login landing page featuring:

- **Template Gallery** — Quick-start templates including Basic Diagram, Blank Drawing, Flowchart, Wireframe, Organization Chart, and Mind Map.
- **Drawing History** — Tabbed view for Recent, Favorites, and Shared with Me, each showing drawing name, storage path, and last modified date.

---

### Drawing Canvas — Basic Shapes

The core product screen, designed around three zones:

- **Left Panel** — Searchable grid of 21 Basic Shapes (Rectangle, Circle, Hexagon, Cube, Diamond, and more)
- **Canvas** — Light dot-grid on white for alignment cues without visual noise
- **Right Design Panel** — Context-aware controls for Position & Size (X, Y, W, H), Fill color, Opacity, Stroke, Shadow, and Blur. A Layers tab collapses into the same panel slot.

A page navigator at the bottom supports multi-page documents with Previous, Next, and Add Page controls.

---

### UML Shape Libraries

Accessed via **More Shapes**, three UML sub-libraries are available:

#### UML Activity Diagram
Shapes following OMG UML 2.x notation: Action, Decision, Merge Node, Initial Node, Final Node, Fork Node, Join Node, Swimlane, Note. Canvas switches to a ruled white-on-gray stage for precision placement.

#### UML Component Diagram
Structural modeling shapes: Component, Provided Interface (lollipop), Required Interface (socket), Association, Package, Note, Directed Association, Dependency. Toolbar context-shifts on selection to show text formatting and diagram tools.

#### UML State Machine Diagram
Behavioral modeling shapes: State, State with Internal Transitions, Composite State, Submachine State, Initial State, Final State, Choice, Note. Includes alignment tools, connector mode, and a zoom slider in the status bar.

---

### Save As

Backstage-panel layout modeled after Microsoft Office's file management:

- **Left Menu** — Full file operations list: Home, New, Open, Info, Save, Save As, Print, Share, Export, Close, Account, Options
- **Center Column** — Storage locations grouped into Personal (OneDrive) and Other Locations (This PC, Browse)
- **Right Panel** — Inline folder picker (Documents, Desktop) without triggering a native OS dialog

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
