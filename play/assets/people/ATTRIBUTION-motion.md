# people-anims.glb — motion sources

## New clips (motion capture)

Idle, Idle2, Idle3, Talk, Phone, Wait (body), Sit, SitTalk, Walk, Jog, Run

- Source: Carnegie Mellon University Graphics Lab Motion Capture Database
  - Site: http://mocap.cs.cmu.edu/
  - Terms (from the site's front page): "This dataset of motions is free for all uses." "You may include this data in commercially-sold products, but you may not resell this data directly, even in converted form."
  - Requested acknowledgment: The data used in this project was obtained from mocap.cs.cmu.edu. The database was created with funding from NSF EIA-0196217.
- BVH conversion of the CMU data: Bruce Hahne ("cgspeed" BVH release), mirrored at https://github.com/una-dinosauria/cmu-mocap (same CMU terms).
- Retargeted to the MakeHuman game_engine skeleton in Blender (retarget_cmu.py), with knee straightening, stance narrowing, clavicle damping, procedural relaxed finger curls and seamless loop blending applied.

| Clip | CMU trial | Description in CMU index | Window (s) | BVH URL |
|---|---|---|---|---|
| Idle | 82_08 | stand still; casual walk forward | 1.25–7.25 | https://raw.githubusercontent.com/una-dinosauria/cmu-mocap/master/data/082/82_08.bvh |
| Idle2 | 40_10 | wait for bus | 0–6 | https://raw.githubusercontent.com/una-dinosauria/cmu-mocap/master/data/040/40_10.bvh |
| Idle3 | 113_21 | Standing Still | 6–11 | https://raw.githubusercontent.com/una-dinosauria/cmu-mocap/master/data/113/113_21.bvh |
| Talk | 18_08 | conversation - explain with hand gestures (2 subjects - subject A) | 3.75–9.75 | https://raw.githubusercontent.com/una-dinosauria/cmu-mocap/master/data/018/18_08.bvh |
| Phone | 80_25 (mirrored) | answering a phone | 3–7 | https://raw.githubusercontent.com/una-dinosauria/cmu-mocap/master/data/080/80_25.bvh |
| Wait (body) | 82_08 | stand still; casual walk forward | 0.75–6.9166 | https://raw.githubusercontent.com/una-dinosauria/cmu-mocap/master/data/082/82_08.bvh |
| Sit | 13_04 | sit on stepstool, chin in hand | 33.5–36.5 | https://raw.githubusercontent.com/una-dinosauria/cmu-mocap/master/data/013/13_04.bvh |
| SitTalk | 86_15 | walking, sitting, hand motions | 48.5–52.5 | https://raw.githubusercontent.com/una-dinosauria/cmu-mocap/master/data/086/86_15.bvh |
| Walk | 35_01 | walk | 0.6–1.73 | https://raw.githubusercontent.com/una-dinosauria/cmu-mocap/master/data/035/35_01.bvh |
| Jog | 35_18 | run/jog | 0.05–0.8 | https://raw.githubusercontent.com/una-dinosauria/cmu-mocap/master/data/035/35_18.bvh |
| Run | 09_02 | run | 0.2–0.95 | https://raw.githubusercontent.com/una-dinosauria/cmu-mocap/master/data/009/09_02.bvh |

Wait: torso, legs and head from CMU 82_08; folded arms (clavicle to hand) from the previous Wait clip (Quaternius Universal Animation Library, CC0), looped twice.

Sit / SitTalk: upper body from CMU 13_04 / 86_15; pelvis and leg pose from the previous Sit clip (Quaternius, CC0) so the seat fit is unchanged.

All new clips: shoulder (clavicle) set taken from the previous Idle clip (Quaternius, CC0), arm directions from the mocap.

## Clips copied unchanged from the previous people-anims.glb

WalkFormal, No, Yes, Bump, HitHead, Knockback, Death, Interact, Carry, JumpStart, JumpLoop, JumpLand, PistolIdle, PistolAim, PistolShoot, PistolReload, PunchJab, PunchCross, Drive, CrouchIdle, CrouchWalk, Roll, Dance

- Source: Quaternius, Universal Animation Library — CC0 1.0 (https://creativecommons.org/publicdomain/zero/1.0/). https://quaternius.itch.io/universal-animation-library and https://quaternius.itch.io/universal-animation-library-2
