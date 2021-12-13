# Pano3DLayout 
## Dataset description

The dataset consists of 107 scenes containing mostly special indoor cases not included in commonly available datasets, such as sloped ceilings, stepped ceilings, arched ceilings, curved walls and curved floors.

Those scenes provide the ground truth data as watertight meshes, so that they are compatible with common 3D mesh reconstruction pipelines. Besides, they are a mirrored version of meshes to comply with the adopted equirectangular convention (reflected in the X axis).

To virtually compose rendered shots, we have used a panoramic camera to obtain an equirectangular projection covering 360x180 degrees with the Z axis being the up axis (along gravity direction). For that, the camera object was set its rotation at (90º, 0º, 0º) and location at (0, 0, 0) with respect to the world coordinate system (x, y, z). Each rendered image has a height of 512 and width of 1024.

### This dataset is the material related to:

Giovanni Pintore, Eva Almansa, Marco Agus, and Enrico Gobbetti. 2021. **Deep3DLayout: 3D reconstruction of an indoor layout from a spherical panoramic image**. ACM Trans. Graph. 40, 6, Article 250 (December 2021), 12 pages. DOI:https://doi.org/10.1145/3478513.3480480


## Content example of each folder

| img | label_cor |
|:-----------|:--------------|
360º image (512x1024 pixels) ![equi_img](/media/living_room4_1.jpg) | Boundary Mesh ![mesh](/media/living_room4_1_mesh.png)

