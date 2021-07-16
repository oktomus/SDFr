# SDFr
a signed distance field baker for Unity

NOTE: Unity 2021.2 now has an SDF Baking tool packaged with Visual Effect Graph, which produces far better results, I recommend giving Unity's a try (you might also be able to manually backport it to prior editor versions).

about
-----

- Generates signed distance fields as Texture3D in RHalf format for use with ray marching or the Visual Effect Graph.
- Written distances are between -1 and +1, normalized to the bounding box magnitude.
- Takes advantage of Jobs and Burst + Unity Mathematics, comment out the #define in SDFVolume.cs if Burst & Mathematics should not be used.
- Tested in Unity 2018.3

Updates By NoiseCrime
-----

- Updated To include varity of visualisations of the raymarching ( distance, steps, heatmap ) to aid in learning.
- Some code change to improve performance and address some flaws in RayMarchExample Shader.
- Mainly being used as a testbed for learning more about rayMarching through SDF.
- Next step is a code refctor of rayMarch shaders to unify, simplify and improve overal performance.

License
-------
[MIT](LICENSE.md)
