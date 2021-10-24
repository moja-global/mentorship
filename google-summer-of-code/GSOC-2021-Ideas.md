# Google Summer of Code 2021 Ideas

**NOTE**: moja global is not participating in the Google Summer of Code 2021.

A list of projects available for interested moja global mentees. All projects will be supported by a mentor and a mentorship grant. Project details and terms of reference will be developed collaboratively with interested candidates.

## Background

FLINT is an open source, modular tool that estimates greenhouse gas (GHG) emissions from land by modelling the flux of GHG on millions (or even billions) of land parcels.

Measuring emissions and sinks from land use is notoriously difficult and developing tools to estimate these sinks and emissions is expensive and requires specialised expertise.

Through global collaboration between scientists and coders, moja global reduces the cost and increase the quality of the software that can estimate emissions and sinks from land use.

This year (2021) we are focusing on the usability of the FLINT platform. All projects should seek to improve the user experience and help drive the adoption of monitoring, reporting and verification (MRV) of global carbon emissions.

## Pre-requisite skills:

We need a wide range of skills, from coders with JS, Python and C++ experience, to DevOps specialists, cloud architects and UX designers. Understanding spatial and temporal data processing and carbon emissions reporting would be useful but not essential, we will gladly teach you.

## Proposed themes

These are assigned an estimated difficulty (**D0** - easy, **D1** - medium, **D2** - hard) and priority (**P0** - urgent, **P1** - important, **P2** - valuable). If you would like to explore a topic further, please open an issue or contact us on [Slack](https://mojaglobal.slack.com).

### Installation

1. Interface to configure and interact with FLINT Docker containers [**D1**, **P1**] - see: [#4](https://github.com/moja-global/Google_Summer_of_Code/issues/4)
2. Pre-compiled executable with point and click GUI (simplified point models at first) [**D2**, **P2**]

### Documentation

1. Develop a user experience (UX) plan, user interface (UI) style guide [**D1**, **P0**] - see: [#5](https://github.com/moja-global/Google_Summer_of_Code/issues/5)
2. Sequence diagrams for the FLINT architecture and control flow [**D0**, **P1**] - see: [#6](https://github.com/moja-global/Google_Summer_of_Code/issues/6)
3. One or more case studies in module development, ideally the creation of a ‘module repository’ [**D0**, **P0**] - see: [#7](https://github.com/moja-global/Google_Summer_of_Code/issues/7)

### Notebooks

1. Develop notebook workflow for module validation and reporting (possibly pre- and post-processing) [**D1**, **P2**]
2. Could end up as Python or R interfaces that wrap the core FLINT libraries [**D2**, **P2**]

### Benchmarking

1. Design simple reference implementation (e.g. FLINT.example) for profiling and testing [**D1**, **P0**]
2. Implement tooling for profiling performance of core library [**D2**, **P0**]
3. Design adaptive sampling regime to prioritise pixel selection as resolution increases from coarse to fine [**D2**, **P2**]
4. Develop an asynchronous job-queue for work scheduling and distributed computation [**D2**, **P1**]

### Testing

1. Configure tests of reference implementation to run in continuous integration pipeline [**D1**, **P1**]
2. Design a continuous deployment framework for cloud-based demonstration purposes, linking multiple containers (e.g. engine, reporting, visualisation) [**D2**, **P1**]

### Optimisation

1. Evaluate alternative in/output data structures, possibly switching to e.g. compressible GeoTIFFs [**D2**, **P1**]
2. Investigate inconsistencies with exception handling, particularly during spin-up [**D2**, **P0**]
3. Investigate reported issue in forest turn-over rates during non-stand-clearing disturbance events (e.g. parasitism) [**D1**, **P1**]
