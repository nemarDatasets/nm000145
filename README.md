[![DOI](https://img.shields.io/badge/DOI-10.82901%2Fnemar.nm000145-blue)](https://doi.org/10.82901/nemar.nm000145)

# Munich Motor Imagery dataset

Munich Motor Imagery dataset.

## Dataset Overview

- **Code**: GrosseWentrup2009
- **Paradigm**: imagery
- **DOI**: 10.1109/TBME.2008.2009768
- **Subjects**: 10
- **Sessions per subject**: 1
- **Events**: right_hand=2, left_hand=1
- **Trial interval**: [0, 7] s
- **File format**: set
- **Data preprocessed**: True

## Acquisition

- **Sampling rate**: 500.0 Hz
- **Number of channels**: 128
- **Channel types**: eeg=128
- **Channel names**: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100, 101, 102, 103, 104, 105, 106, 107, 108, 109, 110, 111, 112, 113, 114, 115, 116, 117, 118, 119, 120, 121, 122, 123, 124, 125, 126, 127, 128
- **Montage**: standard_1020
- **Hardware**: BrainAmp
- **Reference**: Cz
- **Line frequency**: 50.0 Hz
- **Online filters**: {'highpass_time_constant_s': 10}
- **Impedance threshold**: 10 kOhm

## Participants

- **Number of subjects**: 10
- **Health status**: healthy
- **Age**: mean=25.6, std=2.5
- **Gender distribution**: male=8, female=2
- **Handedness**: {'right': 8}
- **BCI experience**: mixed
- **Species**: human

## Experimental Protocol

- **Paradigm**: imagery
- **Task type**: motor_imagery
- **Number of classes**: 2
- **Class labels**: right_hand, left_hand
- **Trial duration**: 10 s
- **Tasks**: motor_imagery
- **Study design**: two-class motor imagery with arrow cues
- **Feedback type**: none
- **Stimulus type**: arrow_cue
- **Stimulus modalities**: visual
- **Primary modality**: visual
- **Synchronicity**: synchronous
- **Mode**: offline
- **Instructions**: Subjects were instructed to perform haptic motor imagery of the left or the right hand during display of the arrow, as indicated by the direction of the arrow

## HED Event Annotations

Schema: HED 8.4.0 | Browse: https://www.hedtags.org/hed-schema-browser

```
  right_hand
    ├─ Sensory-event
    │  ├─ Experimental-stimulus
    │  ├─ Visual-presentation
    │  └─ Rightward, Arrow
    └─ Agent-action
       └─ Imagine
          ├─ Move
          └─ Right, Hand

  left_hand
    ├─ Sensory-event
    │  ├─ Experimental-stimulus
    │  ├─ Visual-presentation
    │  └─ Leftward, Arrow
    └─ Agent-action
       └─ Imagine
          ├─ Move
          └─ Left, Hand

```
## Paradigm-Specific Parameters

- **Detected paradigm**: motor_imagery
- **Imagery tasks**: left_hand, right_hand
- **Cue duration**: 7.0 s
- **Imagery duration**: 7.0 s

## Data Structure

- **Trials**: 150
- **Trials context**: per_class

## Preprocessing

- **Data state**: preprocessed
- **Preprocessing applied**: True
- **Artifact methods**: none
- **Re-reference**: car
- **Notes**: No trials were rejected and no artifact correction was performed. Data were re-referenced to common average reference offline.

## Signal Processing

- **Classifiers**: Logistic Regression
- **Feature extraction**: CSP, Beamforming, Laplacian, Bandpower
- **Frequency bands**: analyzed=[7.0, 30.0] Hz
- **Spatial filters**: CSP, Beamforming, Laplacian

## Cross-Validation

- **Method**: bootstrapping
- **Evaluation type**: within_subject

## BCI Application

- **Applications**: motor_control
- **Environment**: shielded_room
- **Online feedback**: False

## Tags

- **Pathology**: Healthy
- **Modality**: Motor
- **Type**: Motor

## Documentation

- **DOI**: 10.1109/TBME.2008.2009768
- **License**: CC-BY-4.0
- **Investigators**: Moritz Grosse-Wentrup, Christian Liefhold, Klaus Gramann, Martin Buss
- **Senior author**: Martin Buss
- **Contact**: moritzgw@ieee.org
- **Institution**: Technische Universität München
- **Department**: Institute of Automatic Control Engineering (LSR)
- **Country**: DE
- **Repository**: Zenodo
- **Publication year**: 2009
- **Keywords**: Beamforming, brain-computer interfaces, common spatial patterns, electroencephalography, motor imagery, spatial filtering

## References

Grosse-Wentrup, Moritz, et al. "Beamforming in noninvasive brain–computer interfaces." IEEE Transactions on Biomedical Engineering 56.4 (2009): 1209-1219.
Appelhoff, S., Sanderson, M., Brooks, T., Vliet, M., Quentin, R., Holdgraf, C., Chaumon, M., Mikulan, E., Tavabi, K., Hochenberger, R., Welke, D., Brunner, C., Rockhill, A., Larson, E., Gramfort, A. and Jas, M. (2019). MNE-BIDS: Organizing electrophysiological data into the BIDS format and facilitating their analysis. Journal of Open Source Software 4: (1896). https://doi.org/10.21105/joss.01896

Pernet, C. R., Appelhoff, S., Gorgolewski, K. J., Flandin, G., Phillips, C., Delorme, A., Oostenveld, R. (2019). EEG-BIDS, an extension to the brain imaging data structure for electroencephalography. Scientific Data, 6, 103. https://doi.org/10.1038/s41597-019-0104-8

---
Generated by MOABB 1.5.0 (Mother of All BCI Benchmarks)
https://github.com/NeuroTechX/moabb
