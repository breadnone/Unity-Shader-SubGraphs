These SubGraphs shaders were made for my personal projects in Unity3D. Mostly to get the picture perfect foliage.  

  
# 1. Object Pivot Normal  
Mostly used for foliage to get soft-shading looking. This is full normal reconstruction(Expensive).  

# 2. DoubleSidedNormals  
To get the equal amount of lightings on both sides on a two sided materials(back/front face). We don't have this ootb in URP.  
  
# 3.CameraNormal
A normal facing reconstruction to face the direction of a camera(Expensive).  
Use cases : For Trunks/branches, or to get stylized flat lighting on object that always facing the camera. 

# 4. HideFlatPlanes  
The most awesome trick to hide glancing angels on a fooliage leave planes to produce a very smooth fooliage based on Ben Cloward's UnrealEngine shader ported to Unity (Super-Mega-Expensive)  
Use cases : Perfectly shaped soft-shading foliage. Anime style foliage or fluffy tree 

# 5. MaskMap (AO-Red, SMOOTHNESS-Green, SPECULAR-Blue).  
A channel packed maps into single texture.  

# 6. SimpleWind  
We have this in UE but not in Unity and as the name implies, it's very simple.  

# 7. TrunkWindSway  
A trunk wind sway based on world origin of a mesh. Requires UV0 at the bottom-center (common for trees/foliage).  

# 8. WorldSpaceColorVariation  
A hue-shifted color variation based on it's world position. The smooth transition between colors are based on the min/max range in degree angle (the smaller, the softer transition).  

# 9. FoliageCustomOcclusion  
Custom sphere-shaped occlusion to add volumes to foliage based on Ben Cloward's UnrealEngine shader ported to Unity's ShaderGraph.  
