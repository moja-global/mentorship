# Google Season of Documentation Case Study

**Project**: Develop a content strategy to consolidate and promote documentation for the FLINT.

**Organization** or Project: moja global (https://moja.global)

**Organization Description**: moja global’s mission is to support ambitious climate action by developing pioneering, open-source software – including the groundbreaking FLINT software – to help users accurately and affordably estimate greenhouse gas emissions and removals from forestry, agriculture and other land uses (AFOLU).

**Authors**: Andrew O’Reilly-Nugent

## Problem Statement
Our community members, especially new ones, experienced difficulty understanding how moja global projects can be used or are interrelated. Many of our documentation and training resources are disconnected and unable to be updated in a cohesive manner. Because our documentation is split across multiple websites and repositories it is difficult develop a cohesive understanding of our core projects.

## Proposal Abstract

The primary goals of this project were to:
* Standardize documentation across all of our repositories and improve navigation between moja global projects
* Promote user documentation on how to conduct and configure FLINT using the JSON configuration application.
* Migrate our control flow and architecture diagrams to our contributor’s site making it accessible to a wide audience
* Create a list of available FLINT modules for users to customise their land use change models.
* Publish a tutorial on how to post-process the FLINT results using the moja global Visualisation and Reporting tools.

In order to facilitate a higher volume of documentation and communications, we also developed a system for publishing case studies in addition to our technical documentation using markdown documents to our contributors website for thematic discussions that appeal to a wide range of audiences. The full proposal is available at: https://github.com/moja-global/Google.Season.of.Documentation/blob/master/GSoD2021-moja-global-proposal.md

## Project Description

### Creating the proposal

moja global has very active mentorship pathways and there are always new proposals waiting for an opportunity. To develop our GSoD 2021 proposal, we discussed areas of interest with new mentors, some of whom were GSoD mentees in 2020. After the initial development, our proposal was presented to the Technical Steering committee for feedback and approval, before being published to Github.

### Budget

The 2021 GSoD program took a different format to typical mentorship programs and allowed us to submit a budget that fit our project proposal (rather than offering pre-defined amounts). However, we still wanted to support contributions from new mentees and estimated mentorship stipends that were aligned with the more generous programs we participate in. Our project had two clear workstreams, and enough funding to support two mentees over a five month period. The budget example provided in the GSoD template was very useful and indicated that small amounts for secondary contributions and swag would be acceptable - however we are still exploring a cost effective way to deliver these awards to our community. 

### Participants

We hired two excellent technical writers Harsh Bardhan and Sarthak Kundra, both of whom we recruited by sharing our project proposal across social media. Our mentors Sabita Rao, Sagar Utekar, Sneha Mishra and Andrew O’Reilly-Nugent were existing community members who volunteered to take part. Our project was also supported by subject matter experts Mohit Kumar, Shubham Karande and Mohammad Warid who make regular contributions to our community. 

### Timeline

We scoped our project to be completed within a five month period. We began with a review of the existing documentation, spread across different platforms and repositories, and developed a strategy for consolidating this information. 

## Results

### A new Community Website

During Google Season of Docs, we migrated the entire moja global community website from ReactJS, Bootstrap to Docusaurus. During the course of this migration, we have adopted all the core features that were present in the community website previously and deployed it on Vercel, with a gracious sponsorship from the Vercel team. You can see the results at: https://community.moja.global/

Because Docusaurus was a significantly simpler platform, that renders Markdown and JSX documents, we were able to increase the number of contributions to the site and now have several project pages, with case studies, and an active blog. Through the community website, we led our first i18n internationalization initiative, by releasing some of our documentation in Spanish with the help of community contributors.

In addition to the lifetime pro access to Vercel under it’s open source software sponsorship grant, the community website was listed on algolia doc search which allows crawlers to easily land on the website and our website is currently in queue to be listed on Docusaurus’ project showcase page.

### Extended our Technical Documentation

Moja global also hosts more technical documentation on ReadTheDocs at https://docs.moja.global. As part of Google Season of Code, we have consolidated documentation from a number of Github repositories, wikis and other Google Docs into a single documentation repository. 

We further established .rst documentation for several projects, which are now hosted as project specific documentation on ReadTheDocs.

Project | Documentation Website
---|---
FLINT UI | https://docs.moja.global/projects/flint-ui/en/latest/ 
GCBM Chile Data Preprocessing | https://docs.moja.global/projects/GCBM-Chile-Data-Preprocessing-Tools/en/latest/ 
FLINT Reporting | https://docs.moja.global/projects/flint-reporting/en/latest/

Lastly, we added a documentation style guide to facilitate and will be publishing a content strategy document to help steer the newly founded moja global Documentation Working Group.

One of the first actions of the Documentation Working Group was to define a standardised README. To further boost the contributions and give a high-level overview of the community and the project involved, we also established an organization README that is directly visible on the GitHub organization: https://github.com/moja-global.

### Metrics

We set an ambitious goal of increasing community engagement with our documentation. Our website had 326 active visitors in the month of October and we had 195 documentation related pull requests during Google Season of Documentation, smashing our goals of 100 new visitors and 70 new pull requests. 

We ranked the community website SEO benchmarks on seoptimer, a popular SEO optimization tool and received an A+ for performance and an A for Usability. Our weakest score was Social with a C, which we aim to improve in the future.

In the past six months our community size has increased 400% due to the active engagement of our Documentation Working Group which provides a fantastic entry point for new contributors. In fact, our Slack channel became so popular that we have exceeded the tiered limit and no longer have access to the full history of our #documentation channel, meaning that we cannot assess the increase in activity. However we gained at least 50 new contributors to our projects which is a sign of phenomenal growth.

### Analysis
Our team worked well together. Having clear milestones and regular meetings made sure everyone was on the same page. Harsh and Sarthak worked independently, but having a large group of mentors meant that they were able to have any questions answered quickly.

One especially positive outcome was the increased engagement of our community. Many people want to contribute to our projects and find documentation an accessible entry point to make valuable new additions. We set up a Documentation Working Group to harness this energy and now lead fortnightly meetings for people to develop new connections and get to know our community.

## Summary
Google Season of Documentation 2021 was a resounding success. I’d like to thank Harsh and Sarthak for their amazing contributions and excellent attitudes throughout the project. It has been a pleasure working with such professional documentation experts.

We want to also thank Google for supporting our project and look forward to participating in Google Season of Documentation in 2022. The new format of the program, submitting a proposal with monetary allocation to be distributed as we saw fit, provided additional flexibility and allowed us to structure the program in a way that maximised the value of this generous funding opportunity.

Through good documentation, we have seen a new energy in our community. We hope to build this momentum and continue producing a great open source experience for anyone that wants to participate. Only with your help can we solve this climate challenge.
