# Using the wardrobe in three.js

Every glb has the same `game_engine` skeleton as `public/assets/people`. `people-anims.glb` plays on
the body unchanged: same bone names, same order.

1. Load `<sex>_body.glb`. This is the hairless body, with eyes, eyebrows and eyelashes. It holds `<sex>_Body` (LOD0),
   `<sex>_Body_LOD1` and `<sex>_BrowsLashes`. Keep its skeleton as THE skeleton and run the AnimationMixer on its scene.
2. For each worn piece (`<sex>_<id>.glb`), take its SkinnedMesh (LOD0 is `<id>`, LOD1 is `<id>_LOD1`), add it to
   the body's root and rebind it by bone name:
       const bones = piece.skeleton.bones.map(b => bodyBonesByName[b.name]);
       mesh.bind(new THREE.Skeleton(bones, piece.skeleton.boneInverses), mesh.bindMatrix);
3. Slots: body, hair, top, bottom, shoes, hat. Wear one piece per slot. The jackets (`top_suit_jacket`,
   `top_tux_jacket`, `top_casual_jacket`) already include the shirt under them, so they are tops, not layers.
4. Covered skin. The body geometry has `attributes._hidemask` (a float that holds an integer bitmask; read it with `getX(i)`, since after gltf-transform it can be interleaved). Take
   `worn = OR of (1 << item.hideBit)` over the worn items that have a hideBit, then rebuild the body index
   buffer without each triangle whose three vertices all have `(mask & worn) != 0`. Do the same for LOD1, which
   carries its own `_hidemask`. Recompute this only when the outfit changes.
5. Hats sit over the hair. With a hat on, use a short hair piece (or none).
6. Textures are WebP (EXT_texture_webp): 1024 px for the body (an RGBA atlas whose alpha only drives the
   brows and lashes), 512 px for pieces. Hair is alpha-tested (alphaTest about 0.5, double-sided).
7. If you meshopt-compress these files, keep `_HIDEMASK` out of the quantize pattern.
