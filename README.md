## Orbital Artwork Repo

This repository provides version control for the source files used to create the game levels for the webGPU game "Orbital" at orbital.glowstick.click.

The game is currently just starting development. For each level, only one final **glTF** binary file (`.glb`) is actually included in the final game. This repository provides raw textures and models as `Blender` files.

Current workflow:

- Each world has a dedicated folder where the final output assets are located.
- Each world folder has a subfolder called `src` where the larger, source files are located.
- The 3D world itself is created in Blender (4.5.3) and stored as a `.blend` file in `src` with the same name as the world folder.
- The layered texture files are created in GIMP (3.0.6) and stored as `.xcf` files in `src` with the same name as the texture.
- The world is exported from Blender into the world folder using the separate **`.gltf` + `.bin` + textures** option.
- The textures used in the Blender scene are the final `.png` files, exported from their GIMP project and maximally compressed.