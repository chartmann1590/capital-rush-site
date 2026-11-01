# Street scenery

Maple Tree by evolveduk, [original model](https://sketchfab.com/3d-models/maple-tree-b5e945e7abcc471da6547c04e314774c), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Retrieved through Objaverse. Modified by merging meshes, simplifying bark and distant foliage, compressing textures and fitting the model to 7.62 metres. The authored foliage alpha mask is retained. Source SHA-256: `fcc45a1669886931ca8f3a92d27ba16aaec8f9f675927fa1dde0a0a7bc855450`. Runtime files and checksums are listed in `maple-manifest.json`.

## Lamps and benches — Powered by Poly Haven

Both models are released under CC0 1.0 Universal by Poly Haven.

- Street Lamp 01: https://polyhaven.com/a/street_lamp_01
- Painted Wooden Bench: https://polyhaven.com/a/painted_wooden_bench
- License: https://polyhaven.com/license

The import uses their glTF models and authored PBR color, normal and packed material textures. The lamp geometry is simplified from 30,610 to 7,820 triangles; the bench retains 630 triangles. Textures are resized to 512 pixels and encoded as WebP, and resources are embedded in local GLB files. The source URLs, download MD5 checksums and runtime SHA256 hashes are recorded in manifest.json.

Reproduce with `npm run ingest:street-assets`. Source downloads stay in the ignored data/cache/street directory. Runtime meshes are grouped by material and instanced on sidewalks, with nearby collision boxes.
