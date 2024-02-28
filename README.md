# HORTO-3DLM Dataset
The HORTO-3DLM Dataset contains 3D LiDAR and GNSS/localization data for the purpose of 3D LiDAR-based place recognition, localization and mapping in horticultural environments.

## [Data Download](https://nas-greenbotics.isr.uc.pt/drive/d/s/x4eZ5aPL96blS0i7xNKIl0iJOtkdU7QR/h3YJb7wuqCZpV9NNxgeITnGTRsDJeVNY-a7eAQXUnGQs#file_id=799704328662196403) | 

## Contents
1. [Updates](#1-updates)
2. [Dataset](#2-dataset)

## 1. Updates 
- **1/03/2024** HORTO-3DLM v2.0 added GTJ34 and ON22 sequences
- **1/02/2024** HORTO-3DLM v1.0 Uploaded


## 2. Dataset

### V2.0: 
- GTJ23: recorded in  tomato plantation within a greenhouse, recorded in Coimbra, Portugal.
- ON23: recorded in November 2023, in an orchard in Metz, France.

![Figure](figs/3dmap.jpg) 

Trajectory of each sequence and Recording setups
<p float="left">
  <img src="figs/sequences.jpg" width="330" />
  <img src="figs/robots.jpg" width="290" /> 
</p>

#### Aquistion Setup 
- ***Sequence ON23*** was recorded with an 16-beam Ouster 3D LiDAR and an SBG GNSS/INS system (without RTK) mounted on a Clearpath Husky mobile platform. To address the low LiDAR resolution, the original scans were merged to increase point density, resulting in sub-maps with approximately 100k points per sub-map. This operation reduced the original sequence from 25836 scans to 3086 sub-maps in total.

- ***Sequence GTJ23*** was recorded in June with a 64-beam Ouster 3D LiDAR mounted on a Clearpath Jackal mobile platform. Due to signal interference caused by the greenhouse structure, the GNSS signal was unreliable. Therefore, the ground-truth positions were computed using a SLAM approach.


 
### V1.0: Original HORTO-3DLM recorded in the UK

 ![Figure](figs/horto-3dlm.png)



### Dataset Structure


## Citation:
```
@article{barros2023orchnet,
    title={ORCHNet: A Robust Global Feature Aggregation approach for 3D LiDAR-based Place recognition in Orchards},
    author={Barros, T and Garrote, L and Conde, P and Coombes, MJ and Liu, C and Premebida, C and Nunes, UJ},
    journal={arXiv preprint arXiv:2303.00477},
    year={2023}
}
```


### TO-DO
- Add Sensor TFs