# Landmark material assets

These real PBR texture sets are licensed under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) by Poly Haven:

| Set | Creators | Source |
| --- | --- | --- |
| Japanese Cedar Planks | Charlotte Baglioni: scanning; Rico Cilliers: processing | [Poly Haven](https://polyhaven.com/a/japanese_cedar_planks) |
| Concrete Wall 005 | Dimitrios Savva: photography; Dario Barresi: processing | [Poly Haven](https://polyhaven.com/a/concrete_wall_005) |
| Sandstone Blocks 05 | Rob Tuytel | [Poly Haven](https://polyhaven.com/a/sandstone_blocks_05) |
| Roof Slates 03 | Rob Tuytel | [Poly Haven](https://polyhaven.com/a/roof_slates_03) |

Modified by resizing to 512 pixels and compressing as WebP. `material-manifest.json` records source URLs, verified source MD5 and SHA-256 checksums, runtime SHA-256 checksums, authors, and byte counts. The twelve runtime textures total 1,911,176 bytes. The cedar set is a visual material approximation, not a scan of EMPAC's own cladding.

The landmark geometry is authored in `src/render/LandmarkGeometry.ts`; these are exterior interpretations based on mapped OSM footprints and architectural references, not downloaded photogrammetry models or survey-accurate reproductions. Reference photos are not bundled in runtime assets. Existing OpenStreetMap attribution applies to the map data.

Nott Memorial's red dome sections also reuse the world material family's [Clay Roof Tiles 02](https://polyhaven.com/a/clay_roof_tiles_02), already included and credited in the existing texture asset pack. Its pale dome bands use sandstone; the slate set covers the lower roof skirt.

Architectural references: [The Egg](https://theegg.org/about/history-architecture/), [EMPAC](https://empac.rpi.edu/about/building), [Nott Memorial](https://www.union.edu/about/campus/nott).
