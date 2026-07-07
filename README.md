# OCT_ONH_RNFL_Analysis
Automated OCT image analysis pipeline for optic nerve head localization and retinal quantification.
# OCT ONH RNFL Analysis

**A Python-based pipeline for automated analysis of retinal Optical Coherence Tomography (OCT) images with a focus on optic nerve head (ONH) localization, retinal nerve fiber layer (RNFL) analysis, and quantitative biomarker extraction.**

---

## Overview

Retinal OCT has become an essential imaging modality for studying retinal structure and optic nerve pathology. However, quantitative analysis of OCT images often requires extensive manual processing and lacks reproducible workflows, particularly in preclinical animal models.

This project aims to develop an open, reproducible, and extensible pipeline for automated OCT image analysis, including:

- Optic nerve head (ONH) localization
- OD/OS eye identification
- Four-quadrant retinal segmentation (SN, ST, IN, IT)
- RNFL thickness measurement
- Retinal intensity analysis
- Edema quantification
- Export of quantitative measurements for statistical analysis

The long-term goal is to provide an open-source toolkit for retinal researchers working with experimental OCT datasets.

---

## Features

### Current

- Load OCT images
- Image preprocessing
- Visualization of retinal OCT scans
- Modular Python workflow
- Google Colab compatible

### In Development

- Automatic ONH detection
- Automatic OD/OS identification
- Four-quadrant retinal segmentation
- RNFL thickness analysis
- Intensity profile analysis
- Edema index calculation
- Batch processing of multiple OCT images

### Future Development

- Deep learning-based ONH detection
- Automatic retinal layer segmentation
- 3D OCT volume analysis
- Graphical User Interface (GUI)
- Report generation (PDF/Excel)
- Support for multiple OCT systems

---

## Workflow

```text
Input OCT Image
        │
        ▼
Image Preprocessing
        │
        ▼
Optic Nerve Head Detection
        │
        ▼
Eye Identification (OD / OS)
        │
        ▼
Quadrant Segmentation
(SN • ST • IN • IT)
        │
        ▼
Quantitative Measurements
        │
        ▼
CSV / Excel Output
```

---

## Repository Structure

```
OCT_ONH_RNFL_Analysis/

│── notebooks/
│     OCT_pipeline.ipynb
│
│── src/
│     preprocessing.py
│     detect_onh.py
│     segmentation.py
│     measurements.py
│
│── images/
│     workflow.png
│     example_result.png
│
│── examples/
│     sample_OCT.png
│
│── requirements.txt
│── README.md
```

---

## Software

- Python 3
- Google Colab
- OpenCV
- NumPy
- SciPy
- scikit-image
- Matplotlib
- Pandas

---

## Example Output

The pipeline is designed to generate:

- ONH location
- Retinal quadrant map
- RNFL thickness
- Retinal intensity profile
- Edema measurements
- CSV/Excel output for downstream statistical analysis

---

## Applications

This project is intended for research involving:

- Retinal imaging
- Optic nerve head analysis
- Glaucoma
- Papilledema
- Hydrocephalus
- Neuro-ophthalmology
- Experimental animal models
- Translational ophthalmic research

---

## Citation

If you use this project in your research, please cite the repository and any associated publications (coming soon).

---

## Roadmap

<p align="center">
  <img src="images/week1/project_overview_workflow.png" width="900">
</p>
---

## 🚀 Development Updates

### Week 2 – Automatic ONH Detection

The current development focuses on automatic localization of the **Optic Nerve Head (ONH)** from retinal en-face OCT images.

Reliable ONH localization serves as the anatomical reference for:

- Automatic retinal quadrant generation
- RNFL thickness analysis
- Intensity measurements
- Edema quantification

Current status:

- ✅ Image loading
- ✅ Image preprocessing
- 🚧 ONH detection
- ⏳ Quadrant segmentation

<p align="center">
  <img src="images/week2/ONH_detection_workflow_week2.png" width="900">
</p>


## Week 3 – Standardized Retinal Quadrant Analysis

Following ONH localization, the pipeline automatically establishes anatomically consistent retinal quadrants based on optic nerve head position and eye laterality.

Standardized quadrant generation improves reproducibility and enables direct comparison of regional retinal biomarkers across imaging datasets.

Current Development

✔ Image loading

✔ Preprocessing

✔ ONH detection

🚧 Quadrant generation

⏳ RNFL measurements

<p align="center">
  <img src="images/week3/week3_quadrant_generation.png" width="900">
</p>
---
Week 4 — RNFL Thickness Measurement
### Version 1.0

- [x] Project structure
- [x] Image loading
- [x] Preprocessing
- [ ] ONH detection
- [ ] OD/OS identification

### Version 2.0

- [ ] Quadrant segmentation
- [ ] RNFL measurements
- [ ] Intensity analysis
- [ ] Batch processing

### Version 3.0

- [ ] Deep learning segmentation
- [ ] 3D OCT support
- [ ] GUI
- [ ] Automated report generation

---

## Author

**Hamid Aboutaleb Kadkhodaeian, Ph.D.**

Retinal Imaging Scientist

Research interests include:

- Retinal biology
- Optical coherence tomography (OCT)
- Biomedical image analysis
- Ophthalmology
- Artificial Intelligence for retinal imaging
- Quantitative microscopy

GitHub:
https://github.com/habootaleb92-beep

---

## License

This project is released under the MIT License.
