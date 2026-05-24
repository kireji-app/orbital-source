# Orbital Artwork Source Files

This repository provides the source files of the artwork in the WebGPU game **Orbital.**

<h3><a href="https://orbital.glowstick.click"><img src="https://raw.githubusercontent.com/kireji-app/demo/refs/heads/main/src/click/glowstick/orbital/part.png" style="width:1.25em"/>&nbsp;&nbsp;<sup>Orbital</sup></a><sup></h3>

- Click this link to play the game.

<h3><a href="https://github.com/kireji-app/demo/tree/main/src/click/glowstick/orbital"><img src="https://raw.githubusercontent.com/kireji-app/kireji/refs/heads/main/src/parts/abstract/part/part.png" style="width:1.25em"/>&nbsp;&nbsp;<sup>Code Repo</sup></a><sup></h3>

- Click this link to see the game's source code in the demo ecosystem repo.

## Creating Assets
### Levels
- Created in Blender (4.5.3)
- Saved as `.blend` files
- Exported as **separate `.gltf` + `.bin` + textures**
### Textures
- Created in GIMP (3.0.6)
- Saved as `.xcf` files
- Exported as `.png` files
- Compressed further using TinyPNG
## Naming Convention
```
▼ orbital-source
┊  
╰──▼ example-name    ⎫
┊  ┊                 ⎪  Assets
┊  ╰─ ≡ level.gltf   ⎩  Packed
┊  ┊                 ⎧  Into
┊  ╰─ ▣ level.bin    ⎪  Game
┊  ┊                 ⎪
┊  ╰─ ▣ foo.png      ⎪
┊  ╰─ ▣ bar.png      ⎪
┊  ╰─ ▣ ...          ⎪
┊  ┊                 ⎭
┊  ╰─ ▼ src              ⎫
┊  ┊  ┊                  ⎪  Source
┊  ┊  ╰─ ▣ level.blend   ⎩  Files
┊  ┊  ┆                  ⎧  Not
┊  ┊  ╰─ ⬚ level.blend1  ⎪  Packed
┊  ┊  ┆    (ignored)     ⎪
┊  ┊  ┊                  ⎪ 
┊  ┊  ╰─ ▣ foo.xcf       ⎪
┊  ┊  ╰─ ▣ bar.xcf       ⎪
┊  ┊  ╰─ ▣ ...           ⎪
┊  ┊  ┊                  ⎭
```