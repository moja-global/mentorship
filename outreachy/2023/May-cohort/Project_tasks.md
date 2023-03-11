# Outreachy May 2023 Contribution Phase

Welcome to the Outreachy May 2023 contribution phase at [Moja Global](https://moja.global/). We are very excited to have you participate in our community during this second phase of the selection process of the Outreachy program. Collaboration, transparency and peer encouragement is highly required in the Moja global slack community. We have compiled a list of beginner friendly tasks to help you in this phase of your application. Endeavor to follow the instructions as stated and don't forget to record your contribution after the completion of each task. Happy Contributing:)

# Task 0- Git & Github
Git and Github play a central role in maintaining open-source projects. This encourages transparency, collabortion and accessibility.
* Create a[ github account](https://docs.github.com/en/get-started/onboarding/getting-started-with-your-github-account) if you don't have one yet.
* Add a new repository called Outreachy_username_2022. Where username = your slack handle on [moja global slack community](https://join.slack.com/t/mojaglobal/shared_invite/zt-o6ta1ug0-rVLjAo460~d7JbZ~HpFFtw)
* Clone this repository to your local computer using [git](https://git-scm.com/downloads). To facilitate your work, you can use a code editor such as [VS Code](https://code.visualstudio.com/).  

# Task 1- Land sector management
The [Land sector dataset repository](https://github.com/moja-global/Land_Sector_Datasets) is bringing together datasets that can be useful for land sector management. The metafiles are located in the repository whereas the the data library is located on [moja global hosted google drive](https://datasets.mojaglobal.workers.dev/0:/). You can draw inspiration from this [issue](https://github.com/moja-global/Handbook/issues/8) in the Handbook.

* Select a given country/region/province/state/city (preferably your local environment).
* Navigate the data library to find all types of data corresponding to your selected area.
* Create a jupyter notebook in your repository and carryout data analysis on the corrsponding data you found in the data library.(Use graphs, plots, dataframes etc to provide visualization and interpretation of the data).
* Sign off commits, push your work, record your contribution and share the results of your analysis(notebook) in the #outreachy channel of the slack community.

# Task 2- DVC init
Data driven projects are usually made up of humongous chunks of data. This makes it difficult to keep track of modifications in the data as projects evolve. Fortunately just as we have git for source version control, we also have a tool for data version control referred to as [DVC](https://dvc.org/). 

* Fork and clone the [Land sector repository](https://github.com/moja-global/Land_Sector_Datasets) to your computer.
* Navigate the data library and select a dataset of your choice. Associate the dataset with it's metafile in the cloned repo.
* Initialise the dvc environment and track the datafile. Make sure to identify the metafiles(YAML files)  newly created by this step.
* Setup a [Google Drive DVC Remote](https://dvc.org/doc/user-guide/how-to/setup-google-drive-remote) to provide accessibility to the tracked file.
* Sign off commits and push your work, raise a pull request, record your contribution and share the link in the #outreachy channel of the slack community. Note: exclude the data file from the commit i.e your remote repo should not contain the data file obtained from the data library. Only metafiles should be contained in the updated commit . You can use .dvcignore to exclude the data file.

# Task 3- DVC Repro
A typical data science project is made up of workflows which constitute the pipeline of the project. A pipeline is made up of stages where stages represents individual data processes including the input and resulting output. Adopting DVC in the land sector dataset can be seen as an Extract-Transform-Load process. Extract here refers to obtaining data from the original source(links found in metafiles of datasets). Transform refers to preprocessing of the dataset to make it flint ready(preprocessing commands are found in metafiles of datasets). Load refers to outputting to one or more destinations.
* Create a [reproducible pipeline](https://dvc.org/doc/start/data-management/data-pipelines) for the [Global Soil Maps](https://github.com/moja-global/Land_Sector_Datasets/blob/master/Data/Soil/GlobalSoilOrganicCarbonDensitykgCm2to1mdepth.ipynb).
* Sign off commits and push your work, raise a pull request, record your contribution and share the link in the #outreachy channel of the slack community. Note: exclude the data file from the commit.

# Task 4- Data Hunter
An important charactersitic of being a data engineer is being able to identify and capture data for an ongoing project. 

* Read through this paper on [Global forest management data for 2015 at a 100 m resolution](https://www.nature.com/articles/s41597-022-01332-3#Sec10) and identify the dataset used.
* Create a DVC pipeline for the dataset. Note: a corresponding descriptive metafile should be created as well. Use [this guide]([https:/](https://drive.google.com/file/d/1y9CsPE2gyYub72SB-hdWAJVyWAyEV5ZR/view?usp=sharing)/) for reference on adding a dataset to the land sector repo.
* Sign off commits and push your work, raise a pull request, record your contribution and share the link in the #outreachy channel of the slack community. Note: exclude the data file from the commit.

# Task 5- Automate curation of land sector datasets
* Create a [reproducible pipeline](https://dvc.org/doc/start/data-management/data-pipelines) for a dataset of your own choosing from the data library located on [moja global hosted google drive](https://datasets.mojaglobal.workers.dev/0:/).
* Using GHA and cron jobs, create a suitable workflow to manage, process and update the dataset you selected.

### Conclusion
The criteria for selection for the final phase are irrepective of the completion of the stated tasks, but rather based on qualities clearly defined on the Outreachy website. If you have completed the tasks and want to add your contributions, please feel free to repeat Tasks 2 & 3 for different datasets in the data library.