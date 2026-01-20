# Ultrasound Model Evaluations

**Status:** In Progress

## Project Overview
This project is focused on evaluating computer vision (CV) models for ultrasound image analysis. The goal is to implement, benchmark, and compare different CV architectures to determine the most effective approach for medical imaging tasks.

## Project Goals
- Set up a reproducible environment for model evaluation between NanoHD, ResNet, and EdgeViT.
- Collect evaluation metrics to compare model performance benchmarks:
    - Core Performance
        - Accuracy (task-appropriate metric, e.g., classification accuracy)
        - Inference latency (milliseconds per inference)
        - Model size (parameter count and/or serialized size)
        - Memory usage (peak memory during inference)
    - Consistency & Stability
        - Same Data, Different Run (SDDR)
            - Measure output consistency across repeated runs on identical input data.
        - Different Data, Different Run (DDDR)
            - Measure output variability across different input samples.
        - Dataset anomaly detection
            - Identify potential dataset irregularities or unstable model behavior based on DDDR outcomes.
- Visualize findings and present trade-offs for each model across key medical domain constraints:
    - Interpritability
    - Reproducability
    - Security
    - Accuracy

## Plan
- **Sprint 1:** Functional requirements and project setup (repository, directories, environment).
- **Sprint 2:** Data preparation and preprocessing.
- **Sprint 3:** Baseline model implementation.
- **Sprint 4:** Model evaluation and metrics collection.
- **Sprint 5:** Results analysis and documentation.

## Directory Structure
ultrasound-cv-model-evaluations/
│
├─ datasets/                  # datasets
├─ notebooks/             # experiments and analysis
├─ src/
│  ├─ main.py             # entry point
│  ├─ pipeline/           # evaluation pipeline
│  ├─ models/             # model implementations
├─ README.md
└─ requirements.txt

## How to Run
Currently, this repository contains only the initial project structure. Implementation steps will be added incrementally over the coming weeks.

## License
MIT License
