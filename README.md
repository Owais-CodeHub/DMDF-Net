# DMDF-Net
### Dual Multiscale Dilated Fusion Network for Accurate Segmentation of Lesions Related to COVID-19 in Lung Radiographic Scans

<p align="center">
  <img src="workflow diagram.png" width="100%">
</p>

## Overview

DMDF-Net is a deep learning framework developed for automatic lung and infection segmentation from chest CT scans. The framework utilizes a dual multiscale dilated fusion architecture to accurately localize infection regions and quantify the severity of lung involvement.

### Key Features

- Automatic lung segmentation
- COVID-19 infection segmentation
- Infection area quantification
- Dual multiscale dilated feature fusion
- Cross-dataset evaluation capability
- Lightweight and efficient CAD framework

---

## Repository Structure

```text
DMDF-Net/
│
├── DMDF_Net1_Lung_Seg.mat          # Trained lung segmentation model
├── DMDF_Net2_Inf_Seg.mat           # Trained infection segmentation model
├── MainCode.m                      # Main execution file
├── function_RH_Transformation.m    # Reinhard transformation
├── RGB2Lab.m                       # RGB to Lab color conversion
├── Lab2RGB.m                       # Lab to RGB color conversion
├── workflow diagram.png            # Framework overview
├── Sample Data/                    # Example CT images
└── README.md
```

---

## Methodology

The proposed framework consists of four major stages:

1. **Pre-processing**
   - Reinhard transformation for domain normalization.

2. **Lung Segmentation (DMDF-Net-1)**
   - Extraction of lung regions from chest CT scans.

3. **Infection Segmentation (DMDF-Net-2)**
   - Identification of COVID-19 infection regions.

4. **Post-processing & Quantification**
   - Refinement of segmented regions.
   - Infection proportion estimation.

---

## Usage

Run the following MATLAB script:

```matlab
MainCode
```

The script will:

- Load the trained models.
- Perform lung segmentation.
- Segment infection regions.
- Quantify infection burden.
- Display and save the final results.

---

## Sample Data

Example CT scans are provided in the `Sample Data` folder for quick testing and demonstration.

---

## Requirements

- MATLAB R2020a or later
- Deep Learning Toolbox
- Image Processing Toolbox

---

## Citation

If you find this work useful in your research, please cite:

```bibtex
@article{owais2022dmdf,
  title={DMDF-Net: Dual multiscale dilated fusion network for accurate segmentation of lesions related to COVID-19 in lung radiographic scans},
  author={Owais, Muhammad and Baek, Na Rae and Park, Kang Ryoung},
  journal={Expert Systems with Applications},
  volume={202},
  pages={117360},
  year={2022},
  publisher={Elsevier}
}
```

---

## Paper

**Muhammad Owais, Na Rae Baek, Kang Ryoung Park**

*DMDF-Net: Dual Multiscale Dilated Fusion Network for Accurate Segmentation of Lesions Related to COVID-19 in Lung Radiographic Scans*

**Expert Systems with Applications**, Volume 202, 2022, Article 117360.

---

## Contact

**Muhammad Owais**  
Khalifa University, UAE

For questions, suggestions, or collaborations, please open an issue in this repository.
