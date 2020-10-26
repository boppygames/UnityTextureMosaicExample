# Welcome!

Checkout my game on Steam! https://store.steampowered.com/app/1384030/Boppio/

## FAQ

### What does this do?

This texture mosaics implementation tries to hide texture tiling. Typically when you tile a texture more than a couple of times, you'll be able to see a clear pattern in the texture.

Here is a before/after:

![Before Image](https://github.com/boppygames/UnityTextureMosaicExample/blob/main/ReadmeImg/Before.png?raw=true)

![After Image](https://github.com/boppygames/UnityTextureMosaicExample/blob/main/ReadmeImg/After.png?raw=true)

### What version of Unity is supported?

This should work on any version of Unity that support URP/HRDP. This shader is implemented as a shadergraph shader so it will not work with the built in pipeline. If you are still using the built in pipeline, consider switching to [URP](URP) :)

If you aren't using Unity 2019.4.11f1 and you are having problems with this shader, just copy the shader files within `Shader/` into another project and it should work just fine.

### What kinds of textures does this work for?

This shader works great with any texture that doesn't really have a pattern to it. This shader should even work with textures that aren't seamless.

This shader will not work well with anything that has a pattern to it like tiles, panels, bricks, etc.

### What do the shader properties do?

MainTexture: The albedo texture
Normal: The normal map
Tiling: Base tiling for the texture (before mosaics)
Offset: Base offset for the texture (before mosaics)
MosaicScale: The tiling to apply in the U and V directions for the mosaic
MosaicNoise: This helps reduce seams between blocks, keep this value small (~0.1)
MosaicRotation: The amount of mosaic rotation to apply.
NormalStrength: The strength of the normal.

### Can I use this texture for school, personal projects, or commercially?

Yes! This software is licensed under an MIT license. Check the LICENSE file if you want to see the specifics. All textures included in this projet are part of the public domain (see texture credits).

## Texture Credits

All textures were obtained from opengameart.org. All textures fall under public domain and are free to be redistributed.


