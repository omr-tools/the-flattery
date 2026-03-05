# ✦ The Flattery

**Where all your 3D models are flattered and flattened.**

A browser-based tool for converting 3D OBJ meshes into flat 2D sewing patterns — no installation, no server, no dependencies.

---

## What it does

Upload a Wavefront OBJ file with UV seams (exported from Blender or similar), and The Flattery will:

- Parse vertices, faces, and UV coordinates
- Detect UV seams to identify where the mesh should be cut
- Unroll each mesh piece into an accurate flat 2D pattern
- Let you name and label your pieces
- Export patterns as **SVG, DXF, PNG, or PDF** with optional seam allowance
- Generate an **assembly guide** showing how pieces connect

## How to use

**Live app:** [omr-tools.github.io/the-flattery](https://manyolives.github.io/the-flattery)

Or download `index.html` and open it directly in any modern browser — it runs entirely offline.

## Preparing your OBJ file

For best results, use Blender:

1. Select your mesh and enter **Edit Mode**
2. Select the edges you want as seam lines
3. **Edge → Mark Seam**
4. Unwrap: **UV → Unwrap**
5. Export: **File → Export → Wavefront (.obj)** with *Include UVs* checked

The Flattery uses the UV layout as the flat pattern, so your unwrap *is* your pattern.

## Workflow

| Tab | What happens |
|---|---|
| **Upload** | Drop in your OBJ file |
| **Review** | See the 3D model with seams highlighted alongside the unrolled flat pieces |
| **Label** | Name each pattern piece; see dimensions |
| **Download** | Set seam allowance, pack pieces onto a sheet, export files |
| **Assemble** | Arrange pieces into an assembly guide; export as PNG or PDF |

## Tech

- Vanilla JavaScript — no frameworks, no build step
- Single HTML file
- Canvas 2D rendering
- Runs entirely in the browser; nothing is uploaded anywhere

---

## License

© Olivia Robinson, 2025

- **Source code:** [AGPL-3.0](LICENSE) with non-commercial restriction
- **Design & assets:** [CC BY-NC 4.0](LICENSE)

Free for personal and non-commercial use. For commercial licensing, please get in touch.

See [LICENSE](LICENSE) for full terms.
