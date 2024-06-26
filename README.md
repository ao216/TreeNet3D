# TreeNet3D
TreeNet3D is the first large-scale, multi-type synthetic tree model dataset. The dataset comprises 13,000 models of ten common tree species: camphor tree, small-leaved olive,  agarwood, flooded gum, lemon tree, lombardy poplar ,tibetan cherry, flamboyant tree, fir tree and ajang olive, with each species represented by 1,300 samples. Each tree model offers a 3D point cloud with hierarchical structure and precise parameters, along with information on tree skeletons and volume.  The 3D point cloud is divided into original and noise-added variants, with a distinct separation structure for branches and leaves.  Each branch is differentiated and assigned a branch number attribute based on its sequence.  The tree skeleton abstracts the tree branches into node information, with each skeleton node containing hierarchical relationships and accurate tree radius information.  
<img src="/alltrees.png" width="800">

## TreeNet3D Data
If you would like to download the TreeNet3D data, please fill out an agreement to the [TreeNet3D Terms of Use](https://github.com/ao216/TreeNet3D/blob/main/TreeNet3D%20Terms%20of%20Use.pdf), using your institutional email addresses, and send it to us at shengjuntang@szu.edu.cn.

## Data Organization
The directory has the following structure:
```shell
|-- Flamboyant Tree
| |-- Flamboyant Tree00_01
| | |-- meshmodel
| | | |-- leavesmesh.obj
| | | |-- trunkmesh.obj
| | |-- pointcloud
| | | |-- branchPointClouds.txt
| | | |-- leafPointClouds.txt
| | | |-- mergePointClouds.txt
| | |-- pointcloudnoise
| | | |-- branchPointClouds.txt
| | | |-- leafPointClouds.txt
| | | |-- mergePointClouds.txt
| | |-- skeleton
| | | |-- skeleton.txt
| | |-- TreeVolum.txt
| |-- Flamboyant Tree00_02
| |-- ...

|-- Small-leaved Olive
|-- Camphor Tree
|-- ...
```
## Data Formats
The following are overviews of the data formats used in TreeNet3D:

***.obj**: Mesh in various parts of trees.

***PointClouds.txt**: Point clouds in various parts of trees. Contains attributes as follows：
```shell
[ X, Y, Z, Point Cloud-Branch Index, Point Cloud-Branch Hereditary Relations]
```
***skeleton.txt**: tree skeleton points. Contains attributes as follows：
```shell
[ X, Y, Z, Skeleton-Radius, Skeleton-Branch Hereditary Relations, Skeleton-Branch Index]
```
## Citation
If you use the TreeNet3D data please cite:
```shell
@article{tang2024treenet3d,
  title={TreeNet3D: A large scale tree benchmark for 3D tree modeling, carbon storage estimation and tree segmentation},
  author={Tang, Shengjun and Ao, Zhuoyu and Li, Yaoyu and Huang, Hongsheng and Xie, Linfu and Wang, Ruisheng and Wang, Weixi and Guo, Renzhong},
  journal={International Journal of Applied Earth Observation and Geoinformation},
  volume={130},
  pages={103903},
  year={2024},
  publisher={Elsevier}
}
```
## License
The data is released under the [TreeNet3D Terms of Use](https://github.com/ao216/TreeNet3D/blob/main/TreeNet3D%20Terms%20of%20Use.pdf), and the code is released under the MIT license.

## Help
If you have any questions, please contact us at shengjuntang@szu.edu.cn


