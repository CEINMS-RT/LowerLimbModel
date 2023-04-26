<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ1vHDQMUcbXRoh_hAcOvHvIXIQVk2dtlak3QBu-KU_PnGjMAwr6yHy9VdkSe04BuIF9_w&usqp=CAU" width=200>

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)]()

# LowerLimbModel
Lower-limb model for CEINMS-RT

<img src="https://github.com/CEINMS-RT/LowerLimbModel/blob/main/model/lowerLegModel.JPG" width=300>

## Getting Started
This repo contains the lower limb model, testing data, as well as configure files for CEINMS-RT.

Osim model and testing data are from the subject 06 in a locomotion experiment: https://doi.org/10.5281/zenodo.6457662

Muscle moment arm splines are generated and stored at the folder of **SplineCoeff**.

Execution configure files are stored in the **execution_cfg** folder. 

## How to use:
* Clone/download this repo and put it inside the CEINMS-RT **cfg** folder.

* Run the CEINMS-RT command with the provided configure files.

## What's inside:
This lowerlimb CENIMS execution example contains 9 muscles at the right side of the leg, that span over the ankle, knee, and hip joints.

These nine muscles are:
_tib_ant_r; soleus_r; med_gas_r; lat_gas_r; rect_fem_r; vas_med_r; vas_int_r; vas_lat_r; bifemlh_r; semimem_r; bifemsh_r_

In the example data folder, gait data of two walking speed (_3.6 & 4.5 km/h_) and one running speed (_8.1 km/h_) are provided.

Calibrated subject-specific muscle parameters on these gait data trials are provided as well: **subjectCalibrated.xml**.  

## Citation

```BibTeX
@article{durandau2023Open,
  title={Open source software: CEINMS},
  author={Durandau, Guillaume, ...},
  journal={--},
  volume={--},
  number={-},
  pages={###--###},
  year={####},
  publisher={IEEE}
}
```
