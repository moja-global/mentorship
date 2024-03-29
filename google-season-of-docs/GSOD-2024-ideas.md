# Google Season of Docs 2024

## About moja global

Help fight climate change from the comfort of your home! Moja global provides tools for estimating emissions and removals of greenhouse gases (GHG) from the land sector. The Full Lands INtegration Tool, also known as FLINT, available under MPL-2.0 License, is an open-source platform developed by the moja global team for data collection, analysis, and continuous improvement of greenhouse gas inventories related to land use and land0use change at local and national, and global scales.

The FLINT is based on over 20 years of experience building and operating measurement, reporting, and verification (MRV) tools in Australia and Canada. The FLINT provides the ability to quickly establish an operational MRV system that responds to policymaking and planning needs. The FLINT has been designed to help guide users to the system complexity they need with incremental, step-by-step improvements.

The FLINT platform has multiple models operating on it, one of which is a set of science modules the Canadian Forest Service (CFS) developed known as the generic carbon budget model, or GCBM. The GCBM is a tool developed to assess and report the cumulative effects of [anthropogenic and natural disturbances](https://moja-global.github.io/Handbook/Chapter3/section_one.html) on our forests.

New FLINT users are expected to follow the IPCC guidelines to develop increasingly accurate and robust systems for greenhouse gas accounting. Users are supported by moja global, a vibrant developer community, and philanthropic partners like the UNFCCC and IUCN. We aim to increase institutional users to 14 countries by 2024. We require excellent communication, education, and documentation across various topics, including science, policy, and software development.

Moja global has hosted mentees from Google Summer of Code, Google Season of Docs, The Linux Foundation, and Outreachy internships. The Mentorship Working Group can put interested applicants in contact with previous mentees and mentors as needed. We aim to be an inclusive community and hold regular meetups for moja global’s Working Groups. We celebrate enthusiasm, generosity, and creativity and encourage anyone to join our community to collaborate for change.

## Problem Statement

moja global has participated in [Google Season of Docs [2020]](https://developers.google.com/season-of-docs/docs/2020/participants), [[2021]](https://developers.google.com/season-of-docs/docs/2021/participants), and [[2022]](https://developers.google.com/season-of-docs/docs/2022/participants). Over the past three years, we have developed a [documentation website](https://docs.moja.global/) for technical documentation, a [community website](https://community.moja.global) to host case studies, initiatives, blogs, and project quickstarts, and a [FLINT handbook](https://moja-global.github.io/Handbook/index.html) to break down FLINT concepts in a beginner-friendly manner.

Last year’s Google Season of Docs brought about automation and ensured synchronisation between the code and the documentation. Google Season of Docs 2022 gave us the first edition of the [FLINT Handbook](https://moja-global.github.io/Handbook/) that seeks to guide new users through the “whys” and “hows” of our software.

Though we saw an increase in technical documentation, reference guides, and case studies, there is still much to do. We are looking for technical documentation regarding the customisation of the GCBM and using DVC for reproducibility. In addition to creating new technical documentation, we are looking to increase the visibility of the work done at moja global by creating SEO-enhanced case studies, technical articles, tutorials, etc. These technical contents will teach users how to use the FLINT software to solve real-life problems without supervision.

The primary goals of this project are:  

-   Publish SEO-enhanced tutorials and How-To guides around various moja global projects like FLINT-UI, FLINT.Cloud, and FLINT Reporting Tool, to make them accessible to a broader audience
-   Boost textual explanations with non-textual visuals or graphics, alongside a revamped contributor guide to onboard newcomers further by supporting them with a wide range of information.
-   Extend the [FLINT Handbook](https://moja-global.github.io/Handbook/) to contain information on the customisation of the GCBM and reproducibility using [data version control (DVC)](https://dvc.org/).
-   Publish the first edition of FLINT model gallery through a generalized template to document FLINT’s sample simulation runs.
-   Coordinate the development of capabilities to find and fix outdated documentation among moja global projects and establish a continuity of the processes.
    
The moja global technical documentation is built on [Sphinx](https://www.sphinx-doc.org/en/master/) and further deployed through the ReadTheDocs platform. Our community documentation is created on [Docusaurus](https://docusaurus.io/), a static site generator based on React and [MDX](https://mdxjs.com/). We expect new contributors to experiment with source documentation generators like Doxygen, which can be further published over our Sphinx website by automatically cross-linking them using [Breathe](https://breathe.readthedocs.io/).

All our documentation work is tracked and maintained over the GitHub Issue tracker for moja global docs and Community Website. We expect the technical writers to contribute via pull requests and undergo a series of reviews by the Subject Matter Expert (SME) and a Docs reviewer before it is merged. We are looking to welcome new ideas around making our documentation more accessible, user-friendly, inclusive, and technically accurate.

## Projects

These are the projects the technical writers are expected to work on.

### Creating high-level SEO-enhanced tutorials, How To guides, and Case studies

We are accepting applications for `Technical Writer #1`. Interested applicants can contact us at [mentorship@moja.global](mailto:mentorship@moja.global) or join our `#documentation` channel on Slack and propose their participation. The `Technical Writer #1` will work with [Dr. Andrew O’Reilly-Nugent](https://github.com/aornugent) (TSC Director), [Amarachi Iheanacho](https://github.com/Iheanacho-ai)(Community Documentation Lead), and [Harsh Mishra](https://github.com/harshcaspe) (TSC Community Manager) in creating credible tutorials, how-to guides and case studies to further develop the usability and accessibility of moja global documentation.

The `Technical Writer #1` will be expected to:  

-   Create high-level tutorials, How To guides with solutions to frequently asked questions.
	-   Create tutorials, working demos and theoretically explanatory articles for people without prior knowledge of working with moja global projects.   
	-   Work with the community to create non-textual graphics and designs for breaking down FLINT & GCBM concepts.  
	-   Work with the community to improve the SEO of existing technical content published on the community website.  

-   Develop case studies and technical documentation for moja global projects:
    -   Collaborate with the Technical Steering Committee to build and publish the development documentation for FLINT on Sphinx.
    -   Develop project-specific case studies on FLINT.Cloud, FLINT-UI, DVC & CML integrations, and cloud-native adoption within moja global.
	-   Utilize the friction log to find outdated information, and collaborate with Documentation Working Group to fix common issues across the technical documentation.

-   Create a comprehensive contributor onboarding guide for moja global:
	-   Engage with the Technical Steering Committee members and project maintainers to build new contributor guides for the project.
	-   Collaborate with volunteers to develop technical content (developer guides, videos, blogs, and more!) to help first-time contributors onboard to the project.
	-   Work with the Mentorship working group to publish these new contributor guides on the community website after a validation run with the rest of the community.

We have multiple milestones to ensure that the technical writer has followed up with our requirements throughout the project duration.

| Milestones  | Achievement                                                                | Tentative Date     |
|-------------|----------------------------------------------------------------------------|--------------------|
| Milestone 1 | Deliver the new contributor onboarding guide                               | June 10, 2024      |
| Milestone 2 | Publish the new project-specific case studies on community website         | July 21, 2024      |
| Milestone 3 | Publish the development documentation for FLINT on Sphinx                  | August 11, 2024    |
| Milestone 4 | Furnish non-textual graphics and designs for FLINT & GCBM concepts         | September 15, 2024 |
| Milestone 5 | Finalize the first series of high-level tutorials for moja global projects | October 20, 2024   |

### Extending the FLINT Handbook and preparing documentation for GCBM Toolkit

We are accepting applications for `Technical Writer #2`. Interested applicants can contact us at [mentorship@moja.global](mailto:mentorship@moja.global) or join our `#documentation` channel on Slack and propose their participation. The `Technical Writer #2` will work with [Dr. Andrew O’Reilly-Nugent](https://github.com/aornugent) (TSC Director), [Amarachi Iheanacho](https://github.com/Iheanacho-ai)(Community Documentation Lead), and [Harsh Mishra](https://github.com/harshcaspe) (TSC Community Manager) in extending our FLINT Handbook, a collaboration effort started during GSoD ‘21, documenting our Data Version Control (DVC) & Continuous Machine Learning workflow (CML), and prepare new documentation on our GCBM Toolkit and peripheral projects, like GCBM.Carpathians.

The `Technical Writer #2` will be expected to:

-   Coordinate further development of FLINT Analysis Handbook to publish new documentation:
	-   Strategize with the Documentation Working Group on upcoming chapters and coordinate further development with volunteers.
	-   Work with the Technical Steering Committee to build a friction log for the existing Handbook and calibrate its enhancement.
	-   Document the in-development FLINT modules and provide reproducible code samples to simulate and analyze them locally with FLINT.Cloud.  

-   Prepare new documentation for GCBM Toolkit and GCBM.Carpathians:
	-   Coordinate with the Outreachy interns to understand the scope of GCBM Toolkit and its technical aspects
	-   Develop credible documentation for the project and publish it over our ReadTheDocs platform for new users.
	-   Provide a beginner-friendly developer and user guide for GCBM.Carpathians with a focus on DOM modelling.  

-   Develop documentation around Data Version Control (DVC) & Continuous Machine Learning workflow (CML):
	-   Study the case study published by `Technical Writer #1` and sketch out a general template to simulate DVC & CML workflows. 
	-   Document the template and write how-to-guides to run simulations on external datasets while building content for a model gallery.
	-   Implement a static site generator to pull this content from markdown files and render the simulation graphs.

We have multiple milestones to ensure that the technical writer has followed up with our requirements throughout the project duration.

| Milestones  | Achievement                                                                                | Tentative Date     |
|-------------|--------------------------------------------------------------------------------------------|--------------------|
| Milestone 1 | Plan and deliver the new plan for FLINT Analysis Handbook                                  | June 9, 2024       |
| Milestone 2 | Publish the user guide for GCBM Toolkit on ReadTheDocs                                     | July 19, 2024       |
| Milestone 3 | Publish the DVC & CML template and publish the how-to-guide on community website           | August 18, 2024    |
| Milestone 4 | Furnish the developer and user guide for GCBM.Carpathians on ReadTheDocs                   | September 15, 2024 |
| Milestone 5 | Finish the static site generator to implement the model gallery for FLINT model simulation | October 20, 2024   |

### Volunteers

-   `Volunteer #1`, to help `Technical Writer #1` in developing the graphic assets and designs for moja global documentation.
-   `Volunteer #2` to help coordinate `Technical Writer #2` for building and publishing the FLINT model gallery.
-   `Volunteer #3` to build a friction log and organizing initiatives to find outdated documentation and fixing them.

### Performance Metrics

We will assess our GSoD 2024 impact against the following metrics:

-   Extend the FLINT Analysis Handbook from six to ten chapters, thus accommodating four new chapters.
-   Publish three new case studies around moja global project development and open-source initiatives on the community website.
-   Enhance the visibility of the community blog by publishing five new blogs, including a contributor onboarding guide.
-   Increase the visibility and adoption of community website & technical documentation from 2000 to over 5000 monthly views.
-   Develop a committee of 5 members responsible for building the friction log and tackling outdated documentation in the community.
-   Update moja global’s technical documentation with at least 15 figures and graphics to improve the explainability.
-   Increase the number of active contributors by 10% with the newly updated contributor guide to kick-start new contributions.

## Recommended Skills

-   Great intuition for what makes excellent documentation.
-   Familiarity with Git/Github and Markdown-documentation.
-   Familiarity with C++ Python programming languages.
-   Previous experience with Sphinx and Docusaurus.
-   Experience with carbon models, climate science, and science communication.
-   Experience with land-use change monitoring and emissions accounting or desire to learn!
-   Prior experience participating in an open-source community is a plus (but we welcome new contributors, too!).

## Project Budget

| Budget Item                                   | Amount  | Running Total | Notes/Justification                                                             |
| --------------------------------------------- | ------- | ------------- | ------------------------------------------------------------------------------- |
| Technical Writers                             | $12,000 | $12,000       | 2 Technical Writers x $6000 each                                                |
| Volunteers                                    | $1500   | $13,500       | 3 Volunteers x $500 each                                                        |
| Project T-Shirts                              | $150    | $13,650       | Amount includes T-Shirt and shipping costs                                      |
| In kind contribution from moja global mentors | $0      | $13,650       | Involvement of 3 - 10 moja global representatives, developers and contributors. |
