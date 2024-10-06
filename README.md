# Medical and Biological Imaging / Knowledge Representation (IMA204) - 2023/2024

## Course Overview

This repository contains materials and resources for the course **IMA204: Medical and Biological Imaging / Knowledge Representation**, part of the **Image-Data-Signal** curriculum. The course introduces students to the field of medical imaging, covering topics such as image registration, statistical shape analysis, and graph-based methods for image segmentation and matching.

### Key Topics:

- Image Registration: Techniques using pixel intensity and landmarks for image alignment.
- Statistical Shape Analysis: Understanding and applying statistical models to image shapes.
- Graph-Based Methods: Graph matching and structural registration.
- Medical Imaging Techniques: X-ray, MRI, and dermoscopic imaging, along with segmentation methods for various types of medical images.

## Prerequisites

Students are expected to have knowledge of:
- Basic image processing (IMA201 or equivalent)
- Fundamentals of programming

## Course Structure

- Total Hours: 24 hours of lectures and practical sessions, plus 24 hours of personal work.
- Credits: 2.5 ECTS
- Evaluation: Analysis and discussion of scientific articles, practical reports.

## Instructor

- Professor Pietro Gori

## Installation and Setup

Some exercises and projects require Python and relevant image processing libraries. You can follow the instructions below to set up your environment using `conda`:

1. Anaconda/Miniconda: Download and install Python with Anaconda or Miniconda from [Conda Official Site](https://docs.conda.io/en/latest/).
2. Image Processing Libraries: Create a new conda environment with the necessary packages:
   ```bash
   conda create -n ima python matplotlib numpy scipy scikit-image ipykernel pandas scikit-learn jupyter tqdm bokeh opencv munkres
   ```
3. Activate the environment:
   ```bash
   conda activate ima
   ```

4. Launch Jupyter Notebook (if required for exercises):
   ```bash
   jupyter notebook
   ```

This will set up the necessary environment for running image processing tasks and exercises for the course.

## How to Contribute

Feel free to contribute to the repository by:
- Submitting pull requests for corrections or improvements.
- Providing additional examples or extending the projects.
