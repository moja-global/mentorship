# Google Season of Docs 2022

## About moja global

Help fight climate change from your keyboard! [moja global](https://moja.global/) provides tools for estimating emissions and removals of greenhouse gasses (GHG) from the land sector. The [Full Lands INtegration Tool](https://github.com/moja-global/flint) also known as FLINT, available under MPL-2.0 License, is a platform developed by the moja global team for data collection, analysis, and continuous improvement of greenhouse gas inventories related to land use and land-use change at local, national, and global scales.

The FLINT is based on over 20 years of experience building and operating measurement, reporting, and verification (MRV) tools in Australia and Canada. The FLINT provides the capability to quickly establish an operational MRV system that can respond to policymaking and planning needs. The FLINT has been designed to help guide users to the system complexity they need with incremental, step-by-step improvements.

New FLINT users are expected to follow the IPCC guidelines to develop increasingly accurate and robust systems for greenhouse gas accounting. Users are supported by moja global, a vibrant developer community, and philanthropic partners like the UNFCCC and IUCN. We hope to grow the number of institutional users to 14 countries by 2023 and require excellent communication, education, and documentation across a wide range of topics including science, policy, and software development.

moja global has hosted mentees from [Google Summer of Code](https://summerofcode.withgoogle.com/), [Google Season of Docs](https://developers.google.com/season-of-docs), [The Linux Foundation](https://mentorship.lfx.linuxfoundation.org/), and [Outreachy internships](https://outreachy.org/). The Mentorship Working Group can put interested applicants in contact with previous mentees and mentors as needed. We aim to be an inclusive community and hold regular meet-ups for moja global's Working Groups. Enthusiasm, generosity, and creativity are celebrated and we encourage anyone to join our community to collaborate for change.

## Problem Statement

moja global has participated in Google Season of Docs 2020 & 2021. Over the past two years, we have developed a documentation website for technical documentation and a community website to host, case studies, initiatives, blogs, and project quickstarts. Last year’s Google Season of Docs saw the development of a Documentation Working Group, led by our Google Season of Docs interns, which has helped over 50+ new contributors to contribute to moja global and get started with our projects. Our [case study](https://community.moja.global/blog/google-season-of-docs-2021) details an 400% increase in the community size due to the active engagement of our Documentation Working Group providing an easy entry point for new contributions.

Though we saw an increase in technical documentation, reference guides, and case studies, there is still much to do. We are looking for technical documentation regarding the capabilities of our central framework in order to provide clear examples of common FLINT use cases. While the FLINT framework can describe any generic stock and flow model (including finances, water or biodiversity) the most popular use case is landscape and carbon process modeling. In addition to technical documentation of our software, we are looking for new analysis case studies as part of the FLINT Analysis Handbook, which will serve as a gentle introduction for new users progressing through the FLINT training examples. Both of these projects will explain the core ecosystem and analysis concepts taking place when running a FLINT model and how it exactly works!

The primary goals of this project are:

-   Adopt a source documentation generator for the FLINT and GCBM and publish them on our ReadTheDocs website.  
-   Publish tutorials around various moja global projects, like FLINT-UI, FLINT.Cloud, FLINT Reporting Tool, to make them accessible to a wide audience.  
-   Develop a FLINT Analysis Handbook to help users understand various FLINT training examples and explain the core concepts of the FLINT framework.  
-   Create user and technical documentation on various upcoming moja global projects like GCBM.Colombia, GCBM.Belize and more.   
-   Research and implement FLINT use-cases for our general purpose audience and improve the understanding of our users and contributors.  
-   Implement a feedback funnel on our Community Website and ReadTheDocs to build a friction log and mitigate outdated documentation.

Our technical documentation is built on Sphinx, further deployed through the ReadTheDocs platform. Our community documentation for our contributors and users is created on Docusaurus, a static site generator based on React and MDX. We expect new contributors to experiment with source documentation generators like Doxygen, which can be further published over our Sphinx website by automatically cross-linking them using Breathe.

All our documentation work is tracked and maintained over GitHub Issue tracker for moja global docs and Community Website. We expect the technical writers to make contributions via pull requests and undergo a series of reviews by the Subject Matter Expert (SME) and a Docs reviewer before it is merged. We are looking to welcome new ideas around making our documentation more accessible, user-friendly, inclusive, and technically accurate.

## Projects

### Technical Writer #1 - Building technical documentation, case studies and testing existing documentation

We are accepting applications for Technical Writer #1. Interested applicants can reach out to us on mentorship@moja.global or join our #documentation channel on Slack and propose their interest to participate. The Technical Writer #1 will work with Dr. Andrew O’Reilly-Nugent (TSC Director) and Harsh Mishra (TSC Community Manager and GSoD ‘21 intern) in developing technical documentation for our users, building credible case studies to promote moja global’s FLINT further, and building a pipeline to test and validate existing documentation. During GSoD, Technical Writer #1 will work with the documentation working group under the Technical Steering Committee and make credible progress in furthering the usability and accessibility of moja global documentation.

The Technical Writer #1 will be expected to:

-   Publish FLINT and GCBM source documentation over Sphinx:  
	- Strategize on the adoption of Doxygen and create a workflow to auto-publish the documentation incrementally.  
	- Work with the TSC and core developers to make various contributions to the FLINT and GCBM for compatibility with Doxygen.  
	- Setup the workflow and automate the process of publishing documentation over Sphinx and ReadTheDocs.  

-   Develop case-studies and technical documentation for moja global projects:
    - Collaborate with the TSC members to write and publish documentation for new moja global projects (GCBM.Colombia and GCBM.Belize).  
     - Develop tutorials on working with the FLINT.Cloud, FLINT-UI and FLINT reporting tool projects in collaboration with the user-interface working group.  
     - Write a case study on FLINT modules and popular use-cases to help our users better understand the capabilities of FLINT.  

-   Integrate a test pipeline for moja global documentation:  
      
    - Adopt the documentation style guide at moja global to be used in CI pipelines with Vale.  
     - Implement a feedback funnel for our ReadTheDocs and Community Website to gather real-time feedback from our users.  
      - Collaborate with the documentation working group to build a friction log and improve the state of the documentation at moja global.

We will have multiple milestones to ensure that the technical writer has been following up with our requirements throughout the project duration.

|Milestones  |Achievement                                                     |Tentative Date   |
|------------|----------------------------------------------------------------|-----------------|
|Milestone #1|Publish FLINT and GCBM docs on Doxygen and Sphinx               |May 20, 2022     |
|Milestone #2|Publish documentation websites for two new moja global projects |July 8, 2022     |
|Milestone #3|Deliver tutorials for various moja global projects.             |August 19, 2022  |
|Milestone #4|Furnish case studies on FLINT use-cases and modules.            |October 7, 2022  |
|Milestone #5|Implement the feedback funnel and CI pipelines for docs testing.|November 11, 2022|

### Technical Writer #2 - Building FLINT handbook and preparing credible docs on climate science

We are accepting applications for Technical Writer #2. Interested applicants can reach out to us on mentorship@moja.global or join our #documentation channel on Slack and propose their interest to participate. Technical Writer #2 will work with Dr. Andrew O’Reilly-Nugent (TSC Director) and Harsh Mishra (TSC Community Manager and GSoD ‘21 intern) to write more approachable FLINT development and calibration documentation. It will help our users and contributors better understand climate science, carbon models, and how FLINT fits amongst them. During GSoD, Technical Writer #2 will work with the documentation and the science working group under the Technical Steering Committee and develop a handbook for our new FLINT users to get started with FLINT and develop their implementations.

The Technical Writer #2 will be expected to:

-   Update the existing FLINT technical documentation:  
      - Collaborate with the TSC and FLINT Modules Working Group and understand the scope of FLINT and GCBM.  
      - Develop credible docs for `Understanding FLINT` section over ReadTheDocs aimed at new users.  
      - Create an index/glossary of essential FLINT concepts and terminology and publish them on the Community Website.  

-   Prepare documentation on carbon models and climate science:  
      - Collaborate with the TSC and science working group and connect with subject matter experts to better understand carbon models.  
      - Provide a beginner-friendly case study on understanding more about climate change mitigation, carbon models, and how FLINT helps.  
      - Collaborate with volunteers to develop more extensive documentation on calibrating and developing FLINT.  

-   Develop the FLINT Analysis handbook for new users and contributors:  
      - Strategize with the Documentation Working Group to build the FLINT Analysis handbook and publish it.  
      - Collaborate with the TSC and Modules Working Group to document FLINT training examples and modules.  
      - Provide handy tutorials for the handbook to help users run their FLINT analysis and build their implementation.

We will have multiple milestones to ensure that the technical writer has been following up with our requirements throughout the project duration.

|Milestones  |Achievement                                                     |Tentative Date   |
|------------|----------------------------------------------------------------|-----------------|
|Milestone #1|Publish the documentation for Understanding FLINT over ReadTheDocs.|May 16, 2022     |
|Milestone #2|Publish a case study on carbon models and climate change mitigation.|July 15, 2022    |
|Milestone #3|Document FLINT training examples and modules over Community Website.|August 19, 2022  |
|Milestone #4|Publish technical documentation of FLINT internals and functioning.|October 7, 2022  |
|Milestone #5|Finalize the FLINT Analysis handbook for analysis and calibration.|November 15, 2022|

## Performance Metrics

We will assess our GSoD 2022 impact against the following metrics:

- Conduct the first survey for moja global’s technical documentation and set up a target of 50 feedback submissions to the fhandriction log.
- Publish five new case studies or tutorials detailing FLINT, carbon models, and various moja global projects.
- The Documentation Working Group releases the first edition of the FLINT Analysis Handbook by the end of 2022.
- Increase the number of core moja global projects represented at our ReadTheDocs website from 4 to 10.
- Expand the documentation working group by 50% and take new initiatives to set up a test and integration funnel.
- Increase the visibility and adoption of the Community Website and Technical documentation from 800 to over 1500 monthly unique views.
- Documentation coverage above 70% for two of the core moja global projects: FLINT and GCBM, estimated using a tool like coverxygen.

## Recommended Skills

- Great intuition for what makes excellent documentation. 
- Familiarity with Git/Github and Markdown-documentation.
- Familiarity with C++ Python programming languages.
- Previous experience with Sphinx and Docusaurus.
- Experience with carbon models, climate science, and science communication.
- Experience with land-use change monitoring and emissions accounting or desire to learn!
- Prior experience participating in an open-source community is a plus (but we welcome new contributors, too!).

## Project Budget

|Budget Item |Amount                                                          |Running Total    |Notes/Justification                                                            |
|------------|----------------------------------------------------------------|-----------------|-------------------------------------------------------------------------------|
|Technical Writers|$12,000                                                         |$12,000          |2 Technical Writers x $6000 each                                               |
|Project T-Shirts|$150                                                            |$12,150          |Amount includes T-Shirt and shipping costs                                     |
|In kind contribution from moja global mentors|$0                                                              |$12,150          |Involvement of 3 - 10 moja global representatives, developers and contributors.|
