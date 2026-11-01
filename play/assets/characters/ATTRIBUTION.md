# Animated characters

## Detailed adult character

Gorgehold Scout by **3D Assets**, adapted from MakeHuman CC0 anatomy, eyes and
rig weights with fitted clothing and original animation. CC0 1.0 Universal.

https://3dassets.dev/assets/gorgehold-survivor-gallery-and-operations-gorgehold-sc-5418288a

Immutable source: https://cdn.3dassets.dev/assets/32901/v1/model.glb

SHA256: 4870994d7b56e7240e8c6b58c007e190992f64c9a9bf4099cb6362915f2d4fa0

Adaptations: reduced from 98,536 to 33,792 triangles with UVs, normal seams,
skin weights and authored animation retained; fitted to 1.78 m standing height;
clothing colour variants; game locomotion crossfades; skeleton remapping and
a shared facial/clothing texture atlas for one draw call per person. Used for
Danny's roster slot. Source supplies idle, walk, run and grasp clips; additional
jump, punch, aim and falling poses are authored in the game. These action poses
still need a polish pass, particularly hand/grip placement with held weapons.

Reproduce with `npm run ingest:characters` then `npm run optimize:characters`.

## Detailed female pedestrian

**Female character** by **Matterrazti (Matias Benjamin Errazti Lopez)**, licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Original: https://sketchfab.com/3d-models/female-character-1146f75113764b1e826b5884ada9df2f
Source mirror: https://huggingface.co/datasets/allenai/objaverse/resolve/main/glbs/000-118/1146f75113764b1e826b5884ada9df2f.glb
Source SHA256: `205866692fcf47c0cfac6f142e0a1808bd2c7023e845015bbbebcc03a74b611a`.

Adaptations: corrected mixed centimetre/metre geometry and body orientation; fitted shoulder pivots to the sleeve seams; rebound the original weighted mesh; retargeted CC0 MakeHuman Scout idle/walk/run; grounded locomotion; compressed textures to 512px WebP; retained hair alpha masks and merged runtime materials into one texture atlas. The original 26,426 triangles remain. Used for nearby female pedestrians, within the shared four-person detailed crowd budget. Not a playable roster character.

Reproduce with `npm run optimize:female-character` (downloads and verifies the original if absent).

## Stylized pack

Ultimate Animated Characters by **Quaternius**, CC0 1.0 Universal.
https://quaternius.com/
https://creativecommons.org/publicdomain/zero/1.0/

Adaptations: shared skinned mesh, everyday skin/clothing palettes, standing
height fitting, head proportions, animation crossfades, and stride playback.

## Photo-scanned people (Phase 17)

Files in `scanned/`. Staff and customers in the walk-in rooms. Desktops load them after start; phones load them when the player first walks up to a door.

### Eric_Business

**Eric Rigged 001 - Rigged 3D Business Man** by **Renderpeople**, licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Original: https://sketchfab.com/3d-models/eric-rigged-001-rigged-3d-business-man-a46bc9f67aaa415bb4f3241eef900e7f
Source SHA256: `5fd39ba813c5c5f40bc2ec1ccb29a81f80c703bec0c863847f3beea99ba8ae5e`.

Adaptations: converted from centimetres to metres; joints posed at their bind pose and names simplified; CC0 MakeHuman Scout idle/walk/run retargeted and grounded; textures compressed to 512px WebP. The original 20,542 triangles, UVs and skin weights remain.

### Carla_Business

**Carla Rigged 001 - Rigged 3D Business Women** by **Renderpeople**, licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Original: https://sketchfab.com/3d-models/carla-rigged-001-rigged-3d-business-women-acf520f450d14dd799f98a6fede3edf5
Source SHA256: `703c65fe8ac02134d6ad189f7c78be12780f24b23c72808d9fefe4fee8f03ec7`.

Adaptations: converted from centimetres to metres; joints posed at their bind pose and names simplified; CC0 MakeHuman Scout idle/walk/run retargeted and grounded; textures compressed to 512px WebP. The original 19,988 triangles, UVs and skin weights remain.

### Claudia_Business

**Claudia Rigged 002 - 3D Rigged Business Women** by **Renderpeople**, licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Original: https://sketchfab.com/3d-models/claudia-rigged-002-3d-rigged-business-women-c659bd0accab47c6bbe390cf822a2b92
Source SHA256: `4567aaaf7338b98ff2e057ecb1269c9ee2147ae298f7133a2170eba7714fabf0`.

Adaptations: converted from centimetres to metres; joints posed at their bind pose and names simplified; CC0 MakeHuman Scout idle/walk/run retargeted and grounded; textures compressed to 512px WebP. The original 21,492 triangles, UVs and skin weights remain.

### Sophia_Casual

**Sophia Animated 003 - Animated 3D Woman** by **Renderpeople**, licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Original: https://sketchfab.com/3d-models/sophia-animated-003-animated-3d-woman-dc448c3be0e74f96a55fb475a13433cf
Source SHA256: `63a8c9ddea1ed9999470ba3ef48febf762b8298a51b319ca9de690f3e3e37dfb`.

Adaptations: converted from centimetres to metres; joints posed at their bind pose and names simplified; CC0 MakeHuman Scout idle/walk/run retargeted and grounded; textures compressed to 512px WebP. The original 16,475 triangles, UVs and skin weights remain. The source's own motion-capture clip is kept as `idle_mocap`.

