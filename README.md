## GVCNN (Group-View Convolutional Neural Networks for 3D Shape Recognition)
![](assets/gvcnn_framework.png)

## Data
- Download 10-Class Orientation-aligned Subset from http://modelnet.cs.princeton.edu/
- Download [modelnet10-Class Orientation-aligned Subset](http://modelnet.cs.princeton.edu/) directly and You can create 2D dataset from 3D objects (.obj, .stl, and .off), using [BlenderPhong](https://github.com/WeiTang114/BlenderPhong)
- https://drive.google.com/file/d/0B4v2jR3WsindMUE3N2xiLVpyLW8/view from https://github.com/RBirkeland/MVCNN-PyTorch/blob/master/README.md

- make .png images in order below
  - data_utils/make_views_dir.py
  - data_utils/off2obj.py (after 'sudo apt install openctm-tools')
  - data_utils/obj2png.py

## Quick Start
- make group-view image tfrecord file
  - dataset_tools/create_modelnet_tf_record.py
- execute train.py

## Retrieval
- For training efficiency, it was implemented at the [other repository.](https://github.com/ace19-dev/mvcnn-tf) 

## Notice
- It had better use lighter model or decrease image size because it needs a big resources.
- Only 1 batch size is available now.  

## References from
- http://openaccess.thecvf.com/content_cvpr_2018/papers/Feng_GVCNN_Group-View_Convolutional_CVPR_2018_paper.pdf
- https://github.com/WeiTang114/MVCNN-TensorFlow
- https://github.com/pclausen/obj2png

