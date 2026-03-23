# Routing Planner – Visual Branching With Stepped Placement -

A web-based drag-and-drop routing flow designer for IVRs, call queues, smart routers, and other call flow systems. Supports multiple IVR node types (3, 5, or 10 output paths) and rich node types with a visual, configurable interface.

## Features
- Visual editor for creating and branching routing plans
- Node types: Tracking Number, IVR (3/5/10 paths), Queue, Smart Router, Receiving Number, Voicemail, No Answer
- Flexible output branching for IVR nodes (3, 5, or 10 outputs)
- Click and drag interface powered by [Drawflow](https://github.com/jerosoler/Drawflow)
- Node in-place renaming (double-click label)
- Keyboard Delete/Backspace removes selected nodes
- Save/load routing flows as JSON files

## Installation & Usage

1. **Clone/download this repository**
2. **Start a local webserver** from the project folder (required for local JS file loading):
   
   ```bash
   python3 -m http.server 8000
   ```
3. **Open the app in your browser:**
   
   Go to [http://localhost:8000/routing_planner.html](http://localhost:8000/routing_planner.html)

4. **Create your flow:**
   - Add nodes using the node type dropdown and '+ Add Standalone Node' button
   - Click an output port to branch/connect new nodes
   - Double-click labels to rename nodes
   - Delete selected nodes with Delete/Backspace
   - Save/load flow with JSON files

## File Overview

- `routing_planner.html` – Main app, all core logic (requires the files below)
- `drawflow.min.js` – Drawflow drag-and-drop visual editor (bundled, no extra install needed)
- `drawflow.min.css` – Styling for visual node editor
- `README.md` – This documentation

## Attribution

Powered by [Drawflow](https://github.com/jerosoler/Drawflow) (MIT License). 

---

*Created by Jacob Meyers*

