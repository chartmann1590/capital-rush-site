# Realistic pedestrians (Phase 13)

22 adult pedestrians (12 men, 10 women, ages 21 to 69, five ancestry mixes,
casual / business / work / sport / elegant outfits), each with three body LODs
and three hair LODs on one shared skeleton.

## People

Built with **MakeHuman** base meshes, skins, eyes, eyebrows, eyelashes, hair
and clothing from the MakeHuman community asset packs (system assets, skins01,
skins02, hair01, eyebrows01, shirts01, pants01, shoes01, suits01, dress01).
All of these assets are **CC0 1.0 Universal**.

- https://static.makehumancommunity.org/assets/assetpacks.html
- https://www.makehumancommunity.org/content/license_explanation.html

The people were assembled headless with the MPFB 2.0.18 Blender add-on (the
tool is GPL; the CC0 assets it outputs stay CC0) using the `game_engine` rig.
Roster and body parameters: `tools/people/roster.json`. Builder:
`tools/people/build_people.py` (opaque 1024 px skin/clothes atlas, 512 px
alpha-tested hair atlas, LOD1/LOD2 by decimation).

## Animation

**Universal Animation Library** and **Universal Animation Library 2** by
**Quaternius**, **CC0 1.0 Universal**.

- https://quaternius.itch.io/universal-animation-library
- https://quaternius.itch.io/universal-animation-library-2

Retargeted onto the MakeHuman game_engine rig by
`tools/people/retarget_anims.py` (world-space rotation retarget, pelvis motion
scaled to hip height), trimmed and measured by `tools/people/pack_people.py`
(each clip's ground speed comes from its planted foot, so playback rate =
walking speed / clip speed and feet do not slide). Geometry compressed with
`tools/people/compress_people.mjs` (meshopt).

## Rebuild

    blender --background --factory-startup --python tools/people/build_people.py -- tools/people/roster.json <out>
    blender --background --factory-startup --python tools/people/retarget_anims.py -- <UAL1.glb> <UAL2.glb> <anims>
    python tools/people/pack_people.py <out> <anims> public/assets/people
    node tools/people/compress_people.mjs public/assets/people
