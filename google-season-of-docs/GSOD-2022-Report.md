# Google Season of Documentation Case Study

**Project**: Building technical documentation, case studies and testing existing documentation.

**Organization**: moja global (https://moja.global)

**Organization Description**: moja global’s mission is to support ambitious climate action by developing pioneering, open-source software – including the groundbreaking FLINT software – to help users accurately and affordably estimate greenhouse gas emissions and removals from forestry, agriculture and other land uses (AFOLU).

**Authors**: Andrew O’Reilly-Nugent

## Problem Statement
The Full Lands Integration Tool (FLINT) is a platform developed by the moja global team for greenhouse gas inventories related to land use and land-use change at local, national, and global scales. While we have an established base of technical documentation, there is a steep learning curve for new users and developers. FLINT is written in C++ for performance and simulates complex ecological systems. hile the FLINT framework can describe any generic stock and flow model (including finances, water or biodiversity) the most popular use case is landscape and carbon process modeling. Our most popular model, the Generic Carbon Budget Model (GCBM) lacks detailed documentation of the source code, making it difficult to understand how the model fumctions and the process that it represents. In addition to technical documentation of our software, developing a series of case studies as part of the FLINT Analysis Handbook, which will serve as a gentle introduction for new users progressing through the FLINT training examples.

## Proposal Abstract

The primary goals of this project are:

* Adopt a source documentation generator for the GCBM and publish them on our ReadTheDocs website.
* Publish tutorials around various moja global projects, like FLINT-UI, FLINT.Cloud, FLINT Reporting Tool, to make them accessible to a wide audience.
* Develop a FLINT Analysis Handbook to help users understand various FLINT training examples and explain the core concepts of the FLINT framework.
* Create user and technical documentation on various upcoming moja global projects like GCBM.Colombia, GCBM.Belize and more.
* Research and implement FLINT use-cases for our general purpose audience and improve the understanding of our users and contributors.
* Implement a feedback funnel on our Community Website and ReadTheDocs to build a friction log and mitigate outdated documentation.

The full proposal is available at: https://github.com/moja-global/mentorship/blob/main/google-season-of-docs/GSOD-2022-Project.md

## Project Description

### Creating the proposal

To develop our GSoD 2022 proposal, we discussed areas of interest with the moja global Technical Steering Committee and surveyed our community members on our forums. We identified that both expert and new users lacked the documentation they need. After the initial development, our proposal published to Github for review and feedbacl.

### Budget

The 2022 GSoD program followed a pattern that worked well in 2021. GSoD allowed us to submit a budget that fit our project proposal (rather than offering pre-defined amounts). Our project had two clear workstreams, and enough funding to support two mentees over a five month period. The budget example provided in the GSoD template was very useful.

### Participants

We hired two excellent technical writers Namya LG and Amarachi Iheanacho, both of whom we recruited by sharing our project proposal across social media. Our mentors Harsh Bardhan (moja global Community Manager), Shloka Gupta, Shubham Karande, and Andrew O’Reilly-Nugent (moja global Director - Technical Steering Committee) were existing community members who volunteered to take part.

### Timeline

We scoped our project to be completed within a six month period. The project was developed as two separate workstreams, one for each writer. Each workstream and 4-5 milestones, constituting approximately 4-6 wks work.

## Results

### A new approach to developer-focused documentation

During Google Season of Docs, Namya annotated the GCBM source code with Doxygen. This allows key clsses and functions to be annotated in code. The source is then parsed for docstrings and compiled into standard documentation framework for C++. Namya was also able to deploy this documentation using Github Actions. This means that the docs are automatically rebuilt each time the source code changes - keeping the docs and code synchronised in lockstep. We used a basic Doxygen them that allows readers to search through the documentation by namespace, classes or files. Class hierarchy diagrams are generated to describe the relationship between key methods in our model. The result of this fantastic work can be viewed at: https://moja-global.github.io/moja.canada/

### Building on the foundations of our user documentation

Our user-focused documentation is organised into technical (primarily relating to installation and testing) and analysis (primarily relating to the application of our software to new problems).

Both Namya and Amarachi contributed to our user documentation. Amarachi created the first edition of the FLINT Analysis Handbook which seeks to guide new users through the "why" and "how" of our software - by describing common analysis tasks, the Handbook takes new users on a journey that increases their skill and capability. We plan to release the FLINT Analysis Handbook in the beginning of December and hope to see it grow into a foundational resource. The Handbook can be accessed at: https://moja-global.github.io/Handbook/

Namya contributed to our user documentation in several ways. A feedback funnel was implemented for readers to indicate where they encountered difficulty or mistakes in our documentatation. A CI action for spell checking was implemented on the moja global Community Website. Documentation websites were deployed for two cornerstone GCBM analyses demonstrating the application of moja global models to national scale carbon stock modelling. Lastly, Namya published a blog on the design and development of the moja global FLINTcloud project.

### Metrics

We set an ambitious goal of receiving 50 feedback submissions using the feedback funnel. At the time of writing, we received only seven submissions for our technical installation. Even so, this demonstrates that the funnel works and will facilitate the long-term maintenance of our documentation. The coverage of our source code documentation for the GCBM has increased to more than 70%.

We exceeded our goal of publising three new case studies by 200%. The moja global Documentation Working Group are on track to release the first edition of the FLINT Analysis Handbook by the end of 2022. The working group remains a cornerstone of our community and participation is growing steadily.

### Analysis
Our 2022 GSoD team worked exceptionally well together. Namya and Amarachi were able to work independently, but having a deep roster of mentors meant that they were able to seek help when necessary.

A delightful outcome of this project has been watching Namya and Amarachi grow into leadership roles in our community. Both contributors are now leading working group and community meetings, as well as contributing to the design and maintenance of our projects.

## Summary
Google Season of Documentation 2022 was a extremely successful. I’d like to thank Namya and Amarachi for their contributions. Both displayed fantastic attitudes to work and community building. I feel honoured that they continue to contribute to our community in such a generous manner.

We want to also thank Google for supporting our project and look forward to participating in Google Season of Documentation in 2023. Google Season of Documentation has been a platform that allowed us to build momentum, as a community, through documentation. Documentation is what encourages contributors to user our software, but is also a means by which people join our community as contributors themselves.

I encourage all interested participants to take part in such a supportive program. For interested organisations, I encourage you to find development pathways for your mentees beyond just the specific project. Collaboration is the only way we can tackle this climate challenge.
