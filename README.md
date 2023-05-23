# Pano3DLayout 
## Dataset description

The dataset consists of 107 scenes containing mostly special indoor cases not included in commonly available datasets, such as sloped ceilings, stepped ceilings, arched ceilings, curved walls and curved floors.

Those scenes provide the ground truth data as watertight meshes, so that they are compatible with common 3D mesh reconstruction pipelines. Besides, they are a mirrored version of meshes to comply with the adopted equirectangular convention (reflected in the X axis).

To virtually compose rendered shots, we have used a panoramic camera to obtain an equirectangular projection covering 360x180 degrees with the Z axis being the up axis (along gravity direction). For that, the camera object was set its rotation at (90º, 0º, 0º) and location at (0, 0, 0) with respect to the world coordinate system (x, y, z). Each rendered image has a height of 512 and width of 1024.

## Updates
* 2021-12-10 Code release

## This dataset is the material that belongs to the following publication

Giovanni Pintore, Eva Almansa, Marco Agus, and Enrico Gobbetti. 2021. **Deep3DLayout: 3D reconstruction of an indoor layout from a spherical panoramic image**. ACM Trans. Graph. 40, 6, Article 250 (December 2021), 12 pages. DOI:https://doi.org/10.1145/3478513.3480480

> Released Source Code

[SIGGRAPH Asia 21] [Deep3DLayout - Pytorch Implementation](https://github.com/crs4/Deep3DLayout)

> Dataset Split

In this publication, we used this dataset split as follows: 
| Split | Number of samples |
|:-----------|:--------------|
[train](https://github.com/EvaAlmansa/Pano3DLayout/blob/master/assets/split_dataset/train.txt) | 72
| [test](https://github.com/EvaAlmansa/Pano3DLayout/blob/master/assets/split_dataset/test.txt) | 35

## An example of content of each folder in [dataset](https://github.com/EvaAlmansa/Pano3DLayout/tree/master/dataset)

| img | label_cor |
|:-----------|:--------------|
360º image (512x1024 pixels) ![equi_img](/assets/figures/living_room4_1.jpg) | Boundary Mesh (3D obj) ![mesh](/assets/figures/living_room4_1_mesh.png)

## References of how the dataset was made 

The shape of each room, which is a watertight mesh and the ground truth, was made for us, using [Blender](https://www.blender.org/). In order to have the interior rooms filled with furniture and objects, we have used several freely accessible and non-commercial libraries (as we are using these libraries for research purpose only), such as:

* [Blender: Interior design with blender](https://www.blender.org/user-stories/e-interiores-next-generation-interior-design-with-blender/)
* [Chocofur: Create 360 panorama rendering in blender](https://learn.chocofur.com/create-360-panorama-rendering-in-blender)
* [Sweet Home 3D](https://www.sweethome3d.com/)

## Citation
Please cite our paper for any purpose of usage.
```
@Article{Pintore:2021:D3R,
    author = {Giovanni Pintore and Eva Almansa and Marco Agus and Enrico Gobbetti},
    title = {{Deep3DLayout}: {3D} Reconstruction of an Indoor Layout from a Spherical Panoramic Image},
    journal = {ACM Transactions on Graphics},
    volume = {40},
    number = {6},
    pages = {250:1--250:12},
    month = {December},
    year = {2021},
    doi = {10.1145/3478513.3480480},
    note = {Proc. SIGGRAPH Asia 2021. To appear},
    url = {http://vic.crs4.it/vic/cgi-bin/bib-page.cgi?id='Pintore:2021:D3R'},
}
```

