# MLops for reproducible science

## Mentors

Andrew O'Reilly-Nugent (2022)

## Project Details

| **Intensity**                          | **Priority**              | **Involves**  | **Mentors**              |
| -------------                          | ------------              | ------------- | -----------              |
|  Hard  |  High  | Docker, Python, DVC, CML  | [@aornugent](https://github.com/aornugent); [andrew@moja.global](andrew@moja.global)}} |

moja global's community run earth system simulations to track the flow of carbon in the forestry and land sectors. Models are calibrated to account climate, forest types, disturbances like fires or hurricanes and land-use transitions.

We aim to make these simulations trivially reproducible by streamlining the workflow of data scientists that use our software. We provide pre-built containers with versioned code but do not yet apply this process to our data. Members of the FLINTcloud project aim to add Data version control (DVC) and Continuous machine learning (CML) to our deployment scenario templates.

The goal of DVC is to bring agility, reproducibility, and collaboration into existing data science workflows.

Data engineers, machine learning, and data science practitioners work with a wide range of data. They need to have a workflow and tools to support it to keep track of their artifacts and their versions, resolve issues, and collaborate across teams and systems.

DVC indexes the input and outputs of model code and automatically updates the model to the latest version when data inputs change. CML is an open-source library that complements this process by integrating DVC into continuous integration pipelines such as Github Actions.

This project demonstrate the functionality of reproducible analysis using Github Actions. Success will be evaluated on the number of new data, models and simulations shared within the community.

## Information for Students

moja global's software is strongly targeted at a specific scientific domain - greenhouse gas inventory in the Agriculture, Forestry and Other Land Use (AFOLU) sectors.

In 2021 we began several projects to increase the accessibility of the Full Lands Integration Tool (FLINT) by providing Docker containers running example models using a simple Python interface and the moja global CLI. These pre-built environments provide templates for running common analyses.

moja global also make available open-source land sector datasets for use as inputs into FLINT models. The bottleneck now becomes the calibration of FLINT models to specific data requirements. Using DVC and CML provide a light-weight means to track the specific configuration and calibration of FLINT simulations.

Interested applicants should be familiar with Docker and Github Actions and their place in the data science workflow. An understanding of computational ecology or earth system modelling is useful to verify what model results make for useful summaries, but your mentors can provide appropriate guidance in this area.

We aim to be an inclusive community and hold regular meet-ups for moja global's Working Groups. Enthusiasm, generousity and creativity are celebrated and encourage people to join our community to collaborate for change.

#### First steps

Download the FLINTcloud GCBM container and re-create the GCBM Demo Run. Share your findings on Slack under `#cloud`.
