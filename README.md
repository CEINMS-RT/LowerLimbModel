<img src="https://github.com/CEINMS-RT/ceinmsrt-core-cpp/blob/main/logo-ceinms-rt-white-v.png" width="50%" alt="CEINMS-RT logo">

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)]()

# LowerLimbModel
Lower-limb model for CEINMS-RT

<img src="https://github.com/CEINMS-RT/LowerLimbModel/blob/main/model/lowerLegModel.JPG" width=300>

## Getting Started
This repo contains the lower limb model, testing data, as well as configure files for CEINMS-RT.

Osim model and testing data are from the subject 06 in a locomotion experiment: https://doi.org/10.5281/zenodo.6457662

Muscle moment arm splines are generated and stored at the folder of **SplineCoeff**.

## How to use:
* Clone/download this repo and put it inside the CEINMS-RT **cfg** folder.
* Copy the the folder of **SplineCoeff** into the cfg folder


* Run the CEINMS-RT command with the provided configure files.

```
.\bin\Win\Debug\CEINMS.exe -e .\cfg\LowerLimbModel\executionRT.xml -s .\cfg\LowerLimbModel\subjectMTU.xml -g
```

## What's inside:
This lowerlimb CENIMS execution example contains 9 muscles at the right side of the leg, that span over the ankle, knee, and hip joints.

These nine muscles are:
_tib_ant_r; soleus_r; med_gas_r; lat_gas_r; rect_fem_r; vas_med_r; vas_int_r; vas_lat_r; bifemlh_r; semimem_r; bifemsh_r_

In the example data folder, gait data of two walking speed (_3.6 & 4.5 km/h_) and one running speed (_8.1 km/h_) are provided.

Calibrated subject-specific muscle parameters on these gait data trials are provided as well: **SubjectCalibrated.xml** in data folder.
As well as uncalibrated model: **gait2392_simbody_marker_ankle_knee_hip_r.xml** in data folder.

## Citation

```BibTeX
@article{durandau2017robust,
  title={Robust real-time musculoskeletal modeling driven by electromyograms},
  author={Durandau, Guillaume and Farina, Dario and Sartori, Massimo},
  journal={IEEE transactions on biomedical engineering},
  volume={65},
  number={3},
  pages={556--564},
  year={2017},
  publisher={IEEE}
}
```
