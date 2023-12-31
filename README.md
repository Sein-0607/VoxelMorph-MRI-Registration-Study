# VoxelMorph-MRI-Registration-Study
VoxelMorph model for performing 3D medical image registration

# Medical image registration for MRI
This code was tested with 3D MRI brain volumes.

## Training
1) setup.py
2) make_list_us.py (train_list_3d.txt 생성)
3) train.py
```
python3 setup.py 
python3 make_list_us.py 
python3 ./scripts/tf/train.py --img-list ./train_list_3d.txt --model-dir ./model/outputs

[gpu--version]
python3 ./scripts/tf/train.py --img-list ./train_list_3d.txt --model-dir ./model/outputs --gpu 1
```

## Inference

```
python3 inference.py
```

# Dataset
[Neurite OASIS Sample Data for Training](https://github.com/adalca/medical-datasets/blob/master/neurite-oasis.md)<br/>
[MRI Sample Data for Inference](https://surfer.nmr.mgh.harvard.edu/pub/data/voxelmorph/tutorial_data.tar.gz)

# References
https://github.com/voxelmorph/voxelmorph

[![Paper](https://img.shields.io/badge/Paper-IEEE%20Transactions%20on%20Medical%20Imaging-lightgrey)](https://doi.org/10.1109/tmi.2019.2897538)

```bibtex
@article{Balakrishnan_2019,
  author = {Guha Balakrishnan and Amy Zhao and Mert R. Sabuncu and John Guttag and Adrian V. Dalca},
  title = {{VoxelMorph}: A Learning Framework for Deformable Medical Image Registration},
  journal = {{IEEE} Transactions on Medical Imaging},
  year = 2019,
  volume = 38,
  number = 8,
  pages = {1788--180},
  publisher = {Institute of Electrical and Electronics Engineers ({IEEE})},
  doi = {10.1109/tmi.2019.2897538},
  url = {https://doi.org/10.1109/tmi.2019.2897538},
}
```
