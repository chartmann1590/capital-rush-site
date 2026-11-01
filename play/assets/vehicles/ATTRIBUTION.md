# Generic Town Bus

By **own.guest**, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Original: https://sketchfab.com/3d-models/generic-town-bus-14fe03d792914d51b6c6250b393c44fd
Source mirror: https://huggingface.co/datasets/allenai/objaverse/resolve/main/glbs/000-154/14fe03d792914d51b6c6250b393c44fd.glb
SHA256: `a8750122cb211145706490e8fbd26ce821d6e8a4074f943974997b2331a02ab9`.
Adaptations: geometry welding, connected wheel extraction, texture compression, 10.8 m fitting, material batching, rolling wheel pivots and fleet instancing. Original body textures and interior retained. A generic bus for fictional local routes, not a reproduced CDTA vehicle.

Rebuild with `npm run ingest:bus-asset`.

# Ferrari 458 Italia

- Author: **vicent091036**
- Original: https://sketchfab.com/models/57bf6cc56931426e87494f554df1dab6
- License: Creative Commons Attribution 4.0 International
  https://creativecommons.org/licenses/by/4.0/
- glTF conversion distributed in the Three.js r169 examples:
  https://github.com/mrdoob/three.js/blob/r169/examples/models/gltf/ferrari.glb
- Adaptation in CAPITAL RUSH: real-world scale and pivot, instanced fleet,
  separate automotive paint/glass materials, paint variations and wheel animation.
  The driving variant is reduced from 358,788 to 55,611 triangles, retaining
  authored normals with attribute-aware simplification and Draco compression. Run `npm run optimize:vehicles`
  to reproduce it.
- SHA256: cafe3f48da6797aa9bde75ca768bc5b57db366575fd233e90df186ae988a876e

The source artist is also credited in the game's Credits panel.

## Everyday traffic and performance coupe

- **1991 Honda Civic EG6**, by **rifdanzz**: https://sketchfab.com/3d-models/1991-honda-civic-eg6-f81da34570b145deb463fa091604d251
- **Toyota Corolla KE80**, by **PHAC** (embedded source credit: **remtromol**): https://sketchfab.com/3d-models/toyota-corolla-ke80-2b30faa611e64177a94a69098d27d1fb
- **BMW M4 Competition M Package**, by **SRT Performance**: https://sketchfab.com/3d-models/bmw-m4-competition-m-package-5c0a2dafb1ad408d9fc9eeef9aee531b

All three source files embed CC BY 4.0 attribution: https://creativecommons.org/licenses/by/4.0/
Honda and Toyota source GLBs are distributed through AllenAI's Objaverse archive. The BMW source is mirrored at https://github.com/lukaizj/car-mod-saas (commit 2a4cbf3b06769d7dff84bfdd3d1f445ef672be1a).

Changes: physical scale and forward axis, Draco compression, 512px WebP texture conversion, normal-aware geometry reduction for the Corolla and BMW, instanced drawing, body paint variations, mirrored-face correction, and independently rolling wheels. Fixed BMW textures share a runtime atlas with the original UV repeat preserved. The Civic's source geometry is retained intact.

`npm run ingest:traffic-assets` verifies source SHA256 hashes and reproduces the three driving models. `traffic-manifest.json` records source URLs and hashes, artist credits, runtime SHA256 hashes, triangle counts and wheel/paint mapping. Source files stay in the ignored data/cache/vehicles directory. Source attribution remains embedded in each runtime GLB and is displayed in the game's Credits panel.
Draco decoder files in the adjacent `draco` directory are from Three.js's
vendored Google Draco decoder, licensed under Apache License 2.0:
https://github.com/google/draco/blob/main/LICENSE
