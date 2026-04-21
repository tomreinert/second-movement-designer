# Second Movement Designer

> All credit goes to **Joey Castillo** and the [Sensor Watch](https://www.sensorwatch.net/) project, and to the contributors of [second-movement](https://github.com/joeycastillo/second-movement). This here is a small tool that reuses their work to sketch watch faces visually.

<img width="1219" height="891" alt="Bildschirmfoto 2026-04-21 um 15 35 02" src="https://github.com/user-attachments/assets/f4f77bf1-ab9b-44f8-b64d-385e20ce80d3" />

---

A small browser tool for designing Sensor Watch faces segment-by-segment. Toggle individual LCD segments, type characters into digit positions, and export as `watch_set_pixel(com, seg)` C calls ready to paste into a Movement face.

Supports both chassis skins (F-91W / A158WEA-9) and both LCD types (Classic / Custom Pro), switched independently.

## Run

Open `index.html` in a browser.

## Controls

- **Click** a segment to toggle it.
- **Cmd/Ctrl + click** a digit position or icon to select it.
  - While holding Cmd/Ctrl, hover shows a preview of what you'd select.
- When a digit is selected: type any character, Space toggles the whole digit on/off.
- When an icon is selected: Space toggles it.
- **Arrow keys** navigate 2D to the nearest neighbor. **Tab / Shift+Tab** walk reading order.
- **Esc** exits selection.

Copy the C snippet from the Export panel into your face's `_face_activity` to reproduce the design on hardware.

## Attribution

The F-91W SVG is © 2020 Alexis Philip ([repo](https://github.com/alexisphilip/Casio-F-91W)), used under the MIT license. The A158WEA-9 chassis and custom LCD were contributed to the [Sensor Watch second-movement](https://github.com/joeycastillo/second-movement) project (also MIT).
