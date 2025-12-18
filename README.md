
# KmerVision (Annotated)

## Overview

This dataset contains **annotated road images collected in the city of Douala, Cameroon**, created to support computer vision research and applications such as **object detection, traffic analysis, and intelligent transportation systems**.

The dataset was developed as part of a **Master’s thesis project** and focuses on real-world urban road scenes representative of Central African traffic environments.

The deployed model can be tested here: https://universe.roboflow.com/iu-internationale-hochschule/master-s-thesis-part-one/model/1

---

## Dataset Description

* **Location:** Douala, Cameroon
* **Domain:** Urban road scenes
* **Task:** Object detection
* **Annotation type:** Bounding boxes
* **Image source:** Real-world street-level images
* **Environment:** Diverse lighting, traffic density, and road conditions

The dataset captures the complexity of road infrastructure and traffic patterns commonly found in Douala, including mixed traffic and variable road layouts.

---

## Annotation Format

The dataset is annotated and exported in **YOLOv8 format**, making it directly compatible with Ultralytics YOLOv8 training pipelines.

Each image has:

* A corresponding `.txt` annotation file
* Normalized bounding box coordinates
* One annotation file per image

---

## Directory Structure

```text
dataset/
├── train/
│   ├── images/
│   └── labels/
├── valid/
│   ├── images/
│   └── labels/
├── test/
│   ├── images/
│   └── labels/
└── data.yaml
```

---

## Usage

This dataset can be used for:

* Object detection model training and evaluation
* Traffic monitoring research
* Road safety and urban mobility studies
* Benchmarking computer vision models in African urban contexts

### Example (YOLOv8)

```bash
yolo detect train data=data.yaml model=yolov8n.pt
```

---

## Dataset Versioning

This repository corresponds to **Version 1** of the dataset as hosted on Roboflow. Future versions may include:

* Additional images
* Improved annotations
* Expanded object classes

---

## Limitations

* The dataset is geographically limited to Douala and may not generalize to all regions.
* Traffic patterns and infrastructure are specific to the local context.

---

## License

Please refer to the **Roboflow project page** for licensing and usage terms.
If you use this dataset in academic work, **citation is required**.

---

## Citation

If you use this dataset in your research, please cite it as:

```
Flore N'kam Suguem (2023). KmerVision, Master’s Thesis Project,
IU Internationale Hochschule, 2023.
```

---

## Contact

For questions, corrections, or collaboration inquiries, please contact flore.nkam-suguem@iu-study.org.
