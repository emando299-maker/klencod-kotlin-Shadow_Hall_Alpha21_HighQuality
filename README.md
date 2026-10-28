# Shadow Hall — Alpha 21 (source project)

Android Kotlin / OpenGL ES 2.0 horror-game prototype. Open the `ShadowHallKotlin` folder in KlencodIDE.

## Alpha 21 changes
- Starts with the monster in a side room, rather than directly in the central hall beside the player, to avoid an immediate opening attack.
- The monster's head/body silhouette has additional raised chest, jaw, limb, rib and claw details. Its facing direction updates toward the player instead of staying fixed in one direction.
- The visual-quality preset now defaults to **High detail**.
- Door interaction ranges are more forgiving so the Interact button is easier to use near the four room doors and the internal door.
- Material UVs are scaled by each object's dimensions, so wood/plaster/stone textures tile over large surfaces instead of stretching one copy across an entire wall or floor.
- Material images are enlarged to 512×512 with restrained sharpening and surface grain. This increases texture detail, but does not turn the existing box-based geometry into professionally sculpted assets.
- Existing puzzle, keys, fuse, flashlight, hiding, audio and game-state code is retained from the supplied Alpha 12 source.

## Important limits and verification
- The only source archive supplied for this session was `Shadow_Hall_MultiRoom_Alpha12.zip`. This Alpha 21 package is based on that archive, not on the later Alpha 20 package mentioned in conversation; changes made only in Alpha 13–20 are therefore not included.
- This environment does not have a configured Android build run for this project. The ZIP was checked for integrity and source edits, but APK compilation, installation and gameplay have **not** been verified. Build it in KlencodIDE before replacing your working copy.
- The renderer is still OpenGL ES 2.0 and uses box meshes. This is a visual improvement pass, not AAA photorealism; true cast shadows, a physically accurate flashlight cone, skeletal animation, and imported high-poly models are not implemented here.
