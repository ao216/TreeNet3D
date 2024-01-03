# TreeNet3D
TreeNet3D is the first large-scale, multi-type synthetic tree model dataset. The dataset comprises 13,000 models of ten common tree species: camphor tree, small-leaved olive,  agarwood, flooded gum, lemon tree, lombardy poplar ,tibetan cherry, flamboyant tree, fir tree and ajang olive, with each species represented by 1,300 samples. Each tree model offers a 3D point cloud with hierarchical structure and precise parameters, along with information on tree skeletons and volume.  The 3D point cloud is divided into original and noise-added variants, with a distinct separation structure for branches and leaves.  Each branch is differentiated and assigned a branch number attribute based on its sequence.  The tree skeleton abstracts the tree branches into node information, with each skeleton node containing hierarchical relationships and accurate tree radius information.  

## TreeNet3D Data
If you would like to download the TreeNet3D data, please fill out an agreement to the TreeNet3D Terms of Use, using your institutional email addresses, and send it to us at szszsz216@163.com.

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

***.obj**:


