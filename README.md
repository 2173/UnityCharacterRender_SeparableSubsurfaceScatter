![demo1](demo1.png)
![demo2](demo2.png)
# Unity Subsurface Scattering Skin
## Features:
* Realtime Post-processing SSS effects(Screen Space SSS)
* Custom Shader supported(Stencil based post-processing)
* Realtime color gradient calculations
## Guide:
* Add "SeparableSubsurfaceScatter.cs" to the rendering camera and transform the options provided.
* Add a custom shader material to your human skin renderer.
* The custom shader should have a Stencil marked with "Ref 5", the post-processing component will use this mark.
* Make sure the material's render queue is larger than any other material, for instance alphaTest or 2499 are suggested as queue.
* Currently the effects only support forward rendering path.
## Comming Soon:
* Screen Space SSS for deferred shading rendering path (more efficiency, more effects supported).
* Provide more High definition skin shaders with exciting features.