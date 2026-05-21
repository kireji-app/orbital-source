## Orbital Artwork Repo

This repository provides version control for the source files used to create the game levels for the webGPU game "Orbital" at orbital.glowstick.click.

The game is currently just starting development. For each level, only one final **glTF** binary file (`.glb`) is actually included in the final game. This repository provides raw textures and models as `Blender` files.

Current workflow:

- Each world has a dedicated folder.
- The 3D world itself is created in Blender (4.5.3) and stored as a `.blend` file with the same name as the folder.
- The world is exported from blender as a self-contained `.glb` file, including all textures.
- The layered texture files are created in GIMP (3.0.6) as `.xcf` files named after their material.
- The textures are flattened into same-named PNG files.
- The PNG files are maximally compressed and given the `*-tiny.png` suffix.
- The `*-tiny.png` files are what are ultimately bound to the materials in the Blender scene. They are included in the `.glb` package.