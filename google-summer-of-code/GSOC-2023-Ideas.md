# Google Summer of Code 2023 Ideas

## About moja global

Help fight climate change from your keyboard! [Moja global](https://moja.global) provides tools for estimating emissions and removals of greenhouse gasses (GHG) from the land sector. The [Full Lands INtegration Tool](https://github.com/moja-global/flint), also known as FLINT, available under MPL-2.0 License, is a platform developed by the moja global team for data collection, analysis, and continuous improvement of greenhouse gas inventories related to land use and land-use change at local, national and global scales.

The FLINT is based on over 20 years of experience building and operating measurement, reporting, and verification (MRV) tools in Australia and Canada. The FLINT provides the capability to quickly establish an operational MRV system responding to policymaking and planning needs. The FLINT has been designed to achieve the required accuracy through step-by-step improvements.

New FLINT users are expected to follow the IPCC guidelines to develop increasingly accurate and robust systems for greenhouse gas accounting. Users are supported by moja global, a vibrant developer community, and philanthropic partners like the UNFCCC and IUCN. We aim to grow our institutional users and require excellent communication, education, and documentation across various topics, including science, policy, and software development.

Moja global has hosted mentees from [Google Summer of Code](https://summerofcode.withgoogle.com/), [Google Season of Docs](https://developers.google.com/season-of-docs), [The Linux Foundation](https://mentorship.lfx.linuxfoundation.org/) and [Outreachy internships](https://outreachy.org/). The Mentorship Working Group can put interested applicants in contact with previous mentees and mentors as needed. We aim to be an inclusive community and hold regular meet-ups for moja global's Working Groups. Enthusiasm, generosity, and creativity are celebrated and encourage people to join our community to collaborate for change.

Prospective developers should have a look at the [Google Summer of Code website](https://summerofcode.withgoogle.com) and the [Google Summer of Code Student Guide](https://google.github.io/gsocguides/) to learn more about the program. To draft a proposal, use the [Google Summer of Code proposal template](GSOC-STUDENT-TEMPLATE.md) proposed by our community.

## Idea: Developing a FLINT Forest Monitoring tool using Land Sector datasets

### Abstract

Interested in how forests help us store carbon? We are embarking on a pilot project to monitor the effect of forest management practices worldwide. We hope this work can support forest owners, stakeholders, and policymakers. Using various forest management indicators and a representative sample of the ecosystem and climatic conditions, we aim to develop an open-source workflow for assessing ecological conditions in forests worldwide.

Our project involves finding 100+ small squares of forest worldwide and cross-referencing these locations with freely available land sector datasets to develop a realistic growth simulation. Mentees will work with the moja global DevOps Working Group to develop and document a proof-of-concept for a semi-automated, FLINT-based workflow. 

Although this project aims to run a unique FLINT simulation of forest dynamics for each location, the parameterization and analysis of these simulations will be developed by a cohort of community members of which you will be a part. You'll be responsible for helping set up a scalable and repeatable system for running these simulations, storing and sharing each result in a NoSQL Database (MongoDB). The DevOps Working Group has templates for local and cloud-based deployment of FLINT, and it's associated models that you can use.

| Category              | Rating                                                                                     |
| --------------------- | ------------------------------------------------------------------------------------------ |
| Difficulty            | Medium                                                                                     |
| Priority              | High                                                                                       |
| Skills                | Python, MongoDB, CI/CD, Data Science                                                       |
| Project Size          | Medium (175 hours)                                                                         |
| Preferred Contributor | Student/Professional                                                                       |
| Mentors               | [@aornugent](https://github.com/aornugent), [@HarshCasper](https://github.com/harshcasper) |

### Project Goals

FLINT.cloud provides several templates for container-based deployment of FLINT with a Flask-based API. We have successfully implemented the Generic Carbon Budget Model that describes forest dynamics of large landscapes. We want to demonstrate this capability by running many smaller examples across various ecosystems and climate conditions. 

Generating the model configuration remains a manual (and often tedious job). GSoC mentees will be required to develop semi-automated configuration generation and input data QA as part of this project. Once a simple workflow has been established, the success of our project will be determined by our ability to easily create, track and compare the results of many small simulations at once. A stretch goal is to document a meta-learning protocol for optimizing each simulation's configuration to improve the consistency and accuracy of the simulation ensemble.

![FLINT Monitoring Tool architecture](images/flint-monitoring-tool-architecture.png)

This project entails the following:

- Study the Land Sector datasets and sketch out a data workflow to intelligently identify small squares of forest worldwide.
- Development of a Python-based tool to produce GCBM configurations for the identified squares and dispatch simulations using the FLINT.Cloud templates
- Integrate a CI/CD-based workflow to push generated results to a remote MongoDB Atlas instance while applying rules-based projections.
- Document the results on public moja global documentation and offer a template to users looking to try the above.

### Technical Skills

During this project, you will work with the moja global DevOps Working Group on developing and deploying a new pre-processing tool. This will require hands-on experience with Python, MongoDB, and CI/CD while implementing data science and analysis methodologies. Experience with Python and MongoDB is preferred. Experience with Docker and CI/CD would be helpful. Understanding FLINT, carbon modeling, and the moja global ecosystem will be helpful but optional.

### Resources

- Land Sector Datasets: https://github.com/moja-global/Land_Sector_Datasets
- FLINT.Cloud: https://github.com/moja-global/FLINT.Cloud
- MongoDB Python connection: https://www.mongodb.com/languages/python

### First steps

The best way to get started is to join our Slack community: https://join.slack.com/t/mojaglobal/shared_invite/zt-o6ta1ug0-rVLjAo460~d7JbZ~HpFFtw

Please introduce yourself in `#cloud` - we'd love to know where you come from and what you're interested in. Then proceed to `#documentation` and the [FLINT Handbook](https://moja-global.github.io/Handbook/). If you'd like to install FLINT please review the instructions at [docs.moja.global](https://docs.moja.global) and as for help in `#installation` support. We have some demonstration guides in the FLINTcloud and GCBM.Belize that you can follow to better understand the types of models we plan on using. 

Once comfortable, please study the existing FLINTcloud templates and the Land Sector Datasets repository. Find an appropriate forest dataset and propose a location of interest (pick a forest you like!). Find another datasets of interest and document a workflow to extract and summarise forest squares in your location. Then share your findings on the `#cloud` channel.
