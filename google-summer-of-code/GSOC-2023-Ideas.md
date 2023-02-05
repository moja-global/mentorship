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

## Idea: Packaging FLINT for cross-platform usage 

### Abstract

FLINT is an open-source, modular tool that estimates greenhouse gas (GHG) emissions from land by modeling the flux of GHG on millions (or even billions) of land parcels. Moja global community currently relies on FLINT as an integrating platform for estimating land-based greenhouse gas emissions and removals. FLINT is also used as the base framework for various projects under the Moja global umbrella, including FLINT.Cloud, GCBM, and other projects. The primary role of the FLINT is to coordinate the interaction of data (e.g., spatial data, non-spatial data, carbon pools, variables, fluxes) and modules. As a full-mass balance framework, FLINT meets all IPCC requirements and allows the progressive development of MRV-related systems, data, and capacities.

Currently, building FLINT locally is a challenging and time-consuming process. The development build of FLINT has been made possible only on Windows and Ubuntu, while Docker images are available for other Linux-based distributions and macOS. The project idea is to package FLINT and make the packages available across major operating systems and architectures. These packages would be made available on the FLINT repository (as part of the release) and/or on the moja global community website for users to install and get started with. It would allow the moja global community to demonstrate the cross-platform usage of FLINT and help simplify the workflow for contributors and general users.

The project would also entail developing a standard release process for the FLINT. It would involve communicating with stakeholders across the moja global community, technical skills to triage FLINT and other moja global projects, and working with the maintainers to align with the DevOps working group best practices. The release process would facilitate the timely release of various projects and allow the community to use the packages.

| Category              | Rating                                         |
| --------------------- | ---------------------------------------------- |
| Difficulty            | Medium                                         |
| Priority              | High                                           |
| Skills                | C++, BASH, Batch, GitHub Actions, CMake        |
| Project Size          | Large (350 hours)                              |
| Preferred Contributor | Student/Professional                           |
| Mentors               | [@HarshCasper](https://github.com/harshcasper) |

### Project goals

This project entails the following:

- Understanding FLINT, moja libraries, and the build process involved and sketching a release process for the Technical Steering Committee (TSC).
- Implementing build scripts for various operating systems and architectures to build distributable packages for FLINT.
- Integrating GitHub Actions to package the FLINT and creating a test strategy to facilitate before general usage. 
- Development of a release process to facilitate the release of the packages across the moja global community.

### Technical skills

During this project, the developer will work with the DevOps working group under the Technical Steering Committee (TSC) on packaging FLINT and get hands-on experience working with C++, CMake build systems, writing CI/CD pipelines, and initiating a release process for moja global. Experience with C++, CMake, and GitHub Actions is preferred. Understanding FLINT and packaging mechanisms would be preferred but optional.

### Resources

- CMake: https://cmake.org/
- Understanding FLINT: https://docs.moja.global/en/latest/Understanding-FLINT
- Compiler Cache: https://ccache.dev/
- Packaging with GitHub Actions: https://docs.github.com/en/actions/publishing-packages/

Moja global teams also have development-specific draft guides for understanding the technical intricacies of building FLINT along with the base packages. The guides are available here:

- [Moja base libraries](https://docs.google.com/document/d/1i6S0X0nTyxfJwn6KhGo9AahXOH1gBnTdwYdAxGchHsI/edit?usp=sharing)
- [Moja FLINT library](https://docs.google.com/document/d/1jceIX1E7HOmzmLW6C-E6GDbMz9sxM-nIy90CbY463Lw/edit?usp=sharing)
- [Moja FLINT implementation](https://docs.google.com/document/d/139-1Nc5AR0yhN--Jb0W_jIfzUasoItkt4dyYM3m19N4/edit?usp=sharing)

### First steps

Study the FLINT and follow our [FLINT Developer tutorial](https://www.youtube.com/playlist?list=PL_WECUlMWiUkyx5ohT2jglPSa58XmOhgY) and [FLINT Development setup docs](https://docs.moja.global/en/latest/DevelopmentSetup/index.html) to get started. Formulate a release process plan and share your findings with the DevOps and working group on the `#devops` channel.

## Idea: Develop pipeline for high-throughput visualisation on Google Earth Engine 

### Abstract

The outputs of FLINT are spatially explicit and often used to model carbon flux over vast areas (millions of hectares). With free, global coverage availability, remote sensing data (e.g., Landsat) models are often conducted at 30 m resolution, resulting in billions of spatial units. Natural Resources Canada (NRCan) has developed a visualization workflow for extensive model outputs. We wish to increase the performance and utility of this pipeline to handle truly massive simulation results. 

The Generic Carbon Budget Model is a set of comprehensive science modules that run on FLINT and report carbon stocks and fluxes for several carbon pools relevant to the AFOLU sector. These include forest, debris, soil, peat, moss, and atmospheric pools. While running simulations for tens or hundreds of years, at high resolution, over large areas (e.g., regional or national scales) results in the simulation output databases on hundreds of gigabytes.

Typical post-processing analyses include summarising and aggregating these databases by administrative land unit (e.g., property, county, or state boundaries). Such operations are slow. This project involves developing a new approach to post-processing that improves the performance and throughput of IPCC-compliant reporting guidelines. Candidates will be expected to communicate with stakeholders from moja global and NRCan and demonstrate creativity in proposing new solutions. A background in computer science will be necessary to evaluate the algorithmic complexity of different approaches and algorithms. 

| Category              | Rating                                         |
| --------------------- | ---------------------------------------------- |
| Difficulty            | Hard                                           |
| Priority              | High                                           |
| Skills                | SQL, Geopatial analytics, Google Earth Engine  |
| Project Size          | Large (350 hours)                              |
| Preferred Contributor | Student/Professional                           |
| Mentors               | [@aornugent](https://github.com/aornugent)     |

### Project goals

This project entails the following:

- Researching performant algorithms for database aggregation and geospatial operations.
- Extending existing Google Earth Engine scripts to prototype different solutions.
- Calculate and evaluate the expected performance of the proposed solution.
- Demonstrate the solution's scaling from an example subset to a large (85 GB) benchmark dataset.

### Technical skills

During this project, the developer will work with the Implementation working group under the Technical Steering Committee (TSC) on improving the performance of post-processing and visualization pipelines. Experience with PostgreSQL (or alternative databases), Google Earth Engine, PostGIS, or geopandas is preferred. Understanding carbon modeling and the GCBM is preferred but optional.

### Resources

- GCBM: https://www.nrcan.gc.ca/climate-change/climate-change-impacts-forests/carbon-accounting/forest-carbon-accounting-tools/generic-carbon-budget-model/24366
- Understanding FLINT: https://docs.moja.global/en/latest/Understanding-FLINT
- https://earthengine.google.com/

### First steps

Study the GCBM tutorials on our Youtube channel (https://www.youtube.com/watch?v=WQd8VDrgFRk) to get started. Propose an example algorithm that summarises a geospatial time series and describes its time and memory complexity on the `#04-modules-and-gcbm` channel.

## Idea: Improving FLINT.Reporting for general-purpose usage

### Abstract

Moja global community uses FLINT.Reporting to provide Business Intelligence for analyzing and transforming FLINT output databases into useful information and outputs. FLINT.Reporting Tool takes flux facts and assigns/aggregates them to a land-use category, a reporting table and a UNFCCC reporting variable. The Reporting Tool was brought together to support the generation of tables, graphs, and other reporting artifacts, from the FLINT output databases, to meet policy and other reporting requirements.

The big picture is that the Reporting Tool takes flux facts and assigns/aggregates them to a land-use category, a reporting table and a UNFCCC reporting variable. We did not envision the support for these reporting requirements to happen all at once; but rather in a piece-by-piece manner, with the first version of the Reporting Tool (the current version) supporting the generation of UNFCCC CRF tables. 

The project will involve improving the FLINT.Reporting and ready for our users to extract actionable business intelligence from the FLINT. This project should demonstrate the functionality of FLINT.Reporting to a broader audience by implementing new features, generalizing the reporting process, and improving the analysis for a wider audience. The project would benefit non-technical users like researchers, policymakers, and analysts to understand FLINT and the overall reporting process better.

| Category              | Rating                                         |
| --------------------- | ---------------------------------------------- |
| Difficulty            | Hard                                           |
| Priority              | High                                           |
| Skills                | Spring Boot, Angular, PostgreSQL, Docker, BASH |
| Project Size          | Large (350 hours)                              |
| Preferred Contributor | Student/Professional                           |
| Mentors               | [@tonnix](https://github.com/Tonnix)           |

### Project goals

FLINT.Reporting was built to facilitate processing the Flux database UNFCCC National Inventory as part of National Communications and Biennial Update Reporting. The reporting structure was designed & implemented under the 2006 IPCC Guidelines as a requirement of the enhanced transparency framework. In 2021, the FLINT.Reporting tool was re-designed and implemented with the support for generating UNFCCC CRF tables. Future versions are envisioned to support REDD+ reporting and other reporting requirements.

This project entails the following:

- Developing the administrative unit of the FLINT.Reporting to be as generic as possible. Currently, it is based on the Kenyan Administrative Unit Structure since the reference was Kenyan-based.
- Improve FLINT.Reporting to share the same PostgreSQL database with the FLINT to avoid re-importation issues or re-design it to have its own PostgreSQL database to allow successful importation of dumped data.
- Build an interface for onboarding data to make it easier for non-technical users to operate the system. The FLINT output data is currently loaded into the Reporting Tool's PostgreSQL database via a script which kick-starts the aggregation exercise.
- Expose the FLINT.Reporting configuration allows future users to tweak them to their country's requirements. The Reporting Tool Report Parameters were fixed based on Kenyan policies.

### Technical skills

During this project, the developer will work with the Technical Steering Committee (TSC) on contributing to FLINT.Reporting while getting hands-on experience with Spring Boot, Angular, PostgreSQL, and Docker while understanding FLINT.Reporting in depth. Experience with Spring Boot and PostgreSQL is preferred. Experience with Angular and Docker would be helpful. Understanding FLINT would be preferred but optional.

### Resources

- FLINT.Reporting: ​​https://docs.moja.global/projects/flint-reporting/en/latest/index.html

### First steps

Get FLINT.Reporting up and running on your local machine by following the docs and understanding the various microservices and software components. After setup and initial discovery, share your findings on the `#reporting-tool` channel.

## Idea: UI pipeline for a deforestation predictor

### Abstract

Deforestation is one of the primary sources of greenhouse gas emissions from the land sector. Efforts to reduce deforestation are currently hampered because of a lack of accurate predictions. This project is focused on developing a UI pipeline around our ML model. The model predicts the likelihood of a particular area in the landscape being deforested over the projection period. The predicted deforestation for each area can be aggregated to obtain expected deforestation for a project area, administrative region, or whole country, which will be more informative for the policy-building agencies.

The model pipeline involves predicting deforestation using Landsat 7 satellite images from the Google Earth Engine (GEE) and deforestation labels extracted from relevant datasets (such as the [matt hansen dataset](<https://earthenginepartners.appspot.com/science-2013-global-forest/download_v1.7.html>)).

This project aims to *make the model available to a broader audience.* One of our goals since the project's inception has been to facilitate decision-makers to make informed decisions using our model. Open-sourcing the code and creating convenient interfaces to interact with the model are steps toward this goal.

| Category              | Rating                                   |
| --------------------- | ---------------------------------------- |
| Intensity             | Medium                                 |
| Priority              | Medium                                   |
| Skills                | Python, JavaScript, UI/UX, Design Systems|
| Project Size          | Large(350 hours)                         |
| Preferred Contributor | Student                                  |
| Mentors               | @harshcasper                             |

### Project goals

This project entails the following:

- Creating a web-based application to interact with the model. This would involve taking geospatial coordinates from the user as input and connecting with the remote model server to process the query. 
- Returning the user to a neat and intuitive interface consisting of relevant model outputs, the deforestation labels for the queried region, deforestation plots, and explainability information.
- Managing the deployment of the model and the server-side development at scale to handle large-scale deployments and accommodate faster inferences.
- Development of a scalable user interface that introduces new input and output parameters with minimal effort/change in the client-side code-base for ease of maintenance.

### Technical skills

Experience designing and implementing Web Applications while managing end-to-end client and server-side development is a must! Understanding of a popular Python web framework (FastAPI, Flask, Django) is needed. The choice of the UI library/tools is flexible and will be based on the consensus of the mentor and the mentee. Understanding how a complete UI stack is set up would help the project be finished smoothly. Knowledge of the formats in which large geographical images are stored/rendered is preferred but optional.

### First steps

Please get started by reading and understanding the problem statement and our approach in this [publically available case study](https://community.moja.global/case-studies/powering-deforestation-prediction-using-artificial-intelligence). Try to understand the case study, the use-cases and how you can build an application around it. Share your thoughts on the `#machine-learning` channel and start working on the project's rough architecture and system design.

## Idea: Object-oriented refactor of FLINT.Cloud

### Abstract

Moja global's community runs earth system simulations to track the flow of carbon in the forestry and land sectors. Models are calibrated to account for climate, forest types, disturbances (like fires, hurricanes, and so on), and land-use transitions. FLINT.Cloud is a cloud deployment framework for rapid deployment of FLINT implementations and offering FLINT as a demonstration service. It currently provides various models & simulations that allow an easy entry point for new users to evaluate the FLINT platform and provide a blueprint for new users to roll their own.

Currently, the FLINT.Cloud offers two microservices: FLINT.Example REST API and GCBM REST API. The current implementation follows a functional programming paradigm that is difficult to scale. We have often faced problems implementing new API endpoints and following a consistent schema that would enable us to version our APIs and work on new features. We also wish to switch to an asynchronous, event-driven mode of executing the simulations to ensure a more efficient API layout and an increased processing velocity.

The goal of this project is to implement an object-oriented refactor for FLINT.Cloud, including the addition of `Flask-RESTful` to extend the project modularity. The project should also involve the investigation and implementation of asynchronous task processing to make the carbon simulations more efficient. The current scope of work also entails implementing the unit, integration, and E2E tests to cover the new functional implementation and scale aspects.

| Category              | Rating                                                                   |
| --------------------- | ------------------------------------------------------------------------ |
| Intensity             | Medium                                                                   |
| Priority              | High                                                                     |
| Skills                | Python, Flask, Docker, Object-Oriented programming, RESTful API design   |
| Project Size          | Large(350 hours)                                                         |
| Preferred Contributor | Student                                                                  |
| Mentors               | [Gopinath Balakrishnan](https://www.linkedin.com/in/bgopi), @harshcasper |

### Project goals

In 2021 & 2022, we implemented FlINT.Cloud to showcase a cloud pipeline for FLINT deployments. During this timeline, we also significantly refactored the GCBM REST API to make it more scalable and easier to maintain. As the project progresses, we have identified the need for refactoring the FLINT.Cloud microservices, with a focus on developer experience, scalability, and maintainability. It would ensure the robustness of the blueprint we provide to our users and make it easy to run earth system simulations to track carbon flow in the AFOLU sector at scale.

This project entails the following:

- Refactor the FLINT.Cloud microservices to follow an object-oriented programming paradigm which would involve the implementation of a new schema structure.
- Improve the project's modularity by implementing `Flask-RESTful` extension to FLINT.Cloud microservices, and draw out a consistent testing strategy for the new implementation.
- Investigate and implement asynchronous task processing to make the carbon simulations more efficient for our users and benchmark the performance of the new implementation.
- Present a proof-of-concept for event-driven processing of the carbon simulations, to make the microservices protocol-agnostic and document the new implementation.

### Technical skills

Experience with Python, Flask, and Object-oriented programming is preferable. Understanding Docker and various engineering aspects, such as design, development, testing, and packaging, is useful. Experience with asynchronous task processing and event-driven programming is a plus. Knowledge of the FLINT ecosystem, including various moja global projects, carbon models, and GCBM, is preferred but optional.

### First steps

Introduce yourself on Slack in the `#cloud` channel. Download the FLINT.Cloud GCBM container and re-create the GCBM Demo Run. Share your findings on Slack under `#cloud`. Next, create a system design for the new implementation focusing on improving the API performance, and share it on Slack.
