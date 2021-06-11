# Pano3DLayout 
## Dataset description

The dataset consists of 106 scenes containing mostly special indoor cases not included in common available datasets, such as sloped ceilings, stepped ceilings, arched ceilings, curved walls and curved floors.

Those scenes provide the ground truth data as watertight meshes, so that they are compatible to common 3D mesh reconstruction pipelines, also they are a mirrored version of meshes to comply with the adopted equirectangular convention (reflected in the X axis).

To virtually compose rendered shots, we have used a panoramic camera to obtain an equirectangular projection rendering the full 360° over the Y axis and 180° over the X axis. For that, the camera object was set its rotation at (90º, 0º, 0º) and location at (0, 0, 0) with respect to the world coordinate system (x, y, z). Each rendered image has a height of 512 and width of 1024.

This dataset is the material related to **"Deep3DLayout: 3D Reconstruction of an Indoor Layoutfrom a Spherical Panoramic Image"**

