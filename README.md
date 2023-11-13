# VoxelMorph-MRI-Registration-Study
VoxelMorph model for performing medical image registration

# Medical image registration for MRI
This code was tested with 3D MRI brain volumes.

## Training

```
python3 make_list_us.py
python3 ./scripts/tf/train.py --img-list ./train_list_us_mov.txt --img-fix-list ./train_list_us_fix.txt --model-dir ./model/outputs
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
