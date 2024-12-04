## Forked from [Raylib](https://github.com/raysan5/raylib.git)

### Local Changes:
  
- Modified the stock Makefile to allow for multiple build directories and relative source locations.  I may back this out and provide it as part of [raylib-builder](https://github.com/robknopf/raylib-builder.git)
- Exposed the 'extras' properties that are part of the GLTF/GLB models.  FWIW, I use the user properties of Blender to populate it (like 'isHidden')
- Add a 'isHidden' property to Meshes.  If true, the mesh rendering will be skipped. I needed geometry (like camera attachments or collision boxes) that wouldn't be visible. Is there a better way?  Almost certainly!  I just don't know it.
