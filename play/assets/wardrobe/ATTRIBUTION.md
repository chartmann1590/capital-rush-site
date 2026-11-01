# Player wardrobe: credits

All meshes and textures in this folder were made from **MakeHuman** assets released as
**CC0 1.0 Universal** (public domain):

- MakeHuman system assets (base mesh, skins, eyes, eyebrows, eyelashes, hair short01-04,
  afro01, bob02, long01, ponytail01, braid01, male/female casual, sport and elegant suits,
  shoes01-06, fedora01, fedora_cocked) by the MakeHuman team (Data Collection AB,
  Joel Palmius, Jonas Hauquier), released to CC0 in September 2020.
- MakeHuman community asset packs (shirts01, pants01, shoes01, suits01, dress01, hair01;
  CC0 editions): garments by MRT ("toigo_" assets), Elvaerwyn (elvs_crude_t-shirt_male),
  Joel Palmius (joepal_crude_t-shirt_female), Namuhekam (namuhekam_male_polo_shirt) and
  cortu (cargo pants, jeans shorts, short messy hair).
- Each piece's source asset and author are listed in `manifest.json`.

Sources:
- https://static.makehumancommunity.org/assets/assetpacks.html
- https://www.makehumancommunity.org/content/license_explanation.html

Assets in those packs that carry a different licence (AGPL or CC BY) were left out.

Built headless with the MPFB 2.0.18 Blender add-on (the tool is GPL; the CC0 assets it
outputs stay CC0) on the `game_engine` rig, by `build_wardrobe.py` in this folder:

    set BLENDER_USER_RESOURCES=C:\tab-gta-cache\mh\bu
    blender --background --factory-startup --python build_wardrobe.py -- out all

Animation for these bodies is the game's existing `people-anims.glb`: Universal
Animation Library 1 and 2 by Quaternius, CC0 1.0.
