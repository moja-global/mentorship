# Outreachy May 2024 Contribution Phase- Week 2
Welcome to the second week of the Outreachy May 2024 contribution phase at Moja Global. We hope you had a productive first week and are ready to continue making valuable contributions to our community. Remember, collaboration, transparency, and peer encouragement are crucial in the Moja Global Slack community. We have prepared a new set of tasks for you to work on during this week. Let's dive in!

## Project 1: Developing a FLINT Forest Monitoring tool using Land Sector datasets
**Task 1: Olympic National Park**
- Generate a report from the Land Sector Datasets about [Olympic National Park](https://en.m.wikipedia.org/wiki/Olympic_National_Park.).
To accomplish this task, you can utilize the Land Sector Datasets to extract relevant information about Olympic National Park. This data can be used to generate a comprehensive report that highlights various aspects of the park, such as its ecological characteristics, biodiversity, climate conditions, and any other relevant information. The report can serve as a valuable resource for showcasing the park's features to the administrators of the latest grant.

**Task 2: GCBM Emerald Edge**
- Add GCBM Emerald Edge to the FLINTcloud test suite.
The second task involves integrating GCBM Emerald Edge into the FLINTcloud test suite. FLINTcloud is a platform that allows for the testing and evaluation of different models and simulations. By adding GCBM Emerald Edge to the test suite, you can assess its performance and functionality within the FLINTcloud environment. This will provide valuable insights and allow for further analysis and comparison with other models or simulations.

Considering the similarity of the ecotypes between Olympic National Park and the Puget lowland forests, it is possible that the parameters used in [Hien's GCBM simulation for Puget](https://github.com/mHienp/GCBM.Puget) can be reused or adapted for the Olympic National Park scenario. This can help in creating a small-scale demonstration that showcases the potential application of [GCBM Emerald Edge](https://github.com/mHienp/GCBM.EmeraldEdge.Data?tab=readme-ov-file) in the park.

**Resources**
- [Land Sector Datasets](https://github.com/moja-global/Land_Sector_Datasets)
- [FLINT.Cloud](https://github.com/moja-global/FLINT.Cloud)

## Project 2: Packaging FLINT for cross-platform usage
**Task 1: Streamline Installation Process**

- Review the FLINT Development setup documentation and user feedback.
- Identify pain points or challenges faced during installation.
- Propose improvements to simplify the installation process for cross-platform usage.
- Implement changes, create installation guides or scripts for different operating systems.
- Document the revised installation process and share findings in the #18-outreachy channel.

**Task 2: Documentation and Tutorials**

- Identify areas of the FLINT Handbook that require improvement or expansion.
- Update existing documentation to reflect recent changes or additions to FLINT.
- Create new tutorials or guides that address common user queries or specific use cases.
- Ensure clarity, accuracy, and accessibility of the documentation.
- Share progress and any new resources created in the #18-outreachy channel.

**Resources**
- [CMake](https://cmake.org/)
- [Understanding FLINT](https://docs.moja.global/en/latest/Understanding-FLINT)
- [Compiler Cache](https://ccache.dev/)
- [Packaging with GitHub Actions](https://docs.github.com/en/actions/publishing-packages/)

## Project 3: Develop pipeline for high-throughput visualization on Google Earth Engine
**Task 1: Algorithm Implementation**

- Implement the proposed algorithm for summarizing geospatial time series data using Google Earth Engine.
- Refer to GCBM tutorials on the Moja Global YouTube channel for guidance on working with Google Earth Engine.
- Write code to extract relevant data, perform necessary calculations, and generate visual outputs.
- Test the algorithm on sample datasets and ensure efficiency and accuracy.
- Document the algorithm's implementation details and share progress in the #18-outreachy channel.

**Task 2: Performance Optimization**

- Analyze the time and memory complexity of the implemented algorithm.
- Identify potential bottlenecks or areas for performance improvement.
- Explore optimization techniques such as parallel processing or data aggregation.
- Implement identified optimizations and measure their impact on performance.
- Document the optimization process and share findings, including performance comparisons, in the #18-outreachy channel.

**Resources**
- [GCBM](https://www.nrcan.gc.ca/climate-change/climate-change-impacts-forests/carbon-accounting/forest-carbon-accounting-tools/generic-carbon-budget-model/24366)
- [Understanding FLINT](https://docs.moja.global/en/master/FLINT/UnderstandingFLINT/index.html)
- [Earth Engine](https://earthengine.google.com/)


### General Note: Recording Contributions on the Outreachy Dashboard

It is essential to remember to record all contributions made during the Outreachy program on the Outreachy dashboard. This includes not only code contributions but also any suggestions, pull requests, documented workflows, and other valuable contributions. Every effort made towards the project should be documented and recorded.

To ensure a comprehensive record of your contributions, it is recommended to create a dedicated GitHub repository, such as "Outreachy_MG_M24," to store your documents and code. You can use various document formats such as Markdown (.md) files or Jupyter Notebooks (.ipynb) to summarize your findings, document workflows, or provide detailed explanations of your work.

For each completed task, consider creating a document that summarizes your findings, improvements, or changes made. Include relevant code snippets, screenshots, or any other supporting materials that showcase your work. Once you have created the document, upload it to your dedicated GitHub repository.

After uploading the document to your repository, copy the link to the document and record it as a contribution on the Outreachy dashboard. This ensures that your contributions are properly documented and recognized by the program.

Remember, every contribution, no matter how big or small, is valuable and should be recorded. Proper documentation and recording of contributions not only help track progress but also demonstrate your active involvement and impact on the project.
