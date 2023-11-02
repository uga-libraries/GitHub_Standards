# Title of Project
Provide the title of the code project for this repository as the header. No description is needed.

## Overview
This section should describe what this script/repository does, what is its purpose, and what the user should expect. 
It should be around three to five sentences in length if it has an overall purpose. For repositories that are a 
collection of scripts with loosely connected or no unified purpose, describe what each script does briefly.

***Example:***
This is the general workflow to make archival information packages (AIPs) that are ready for ingest into the UGA 
Libraries' digital preservation system (ARCHive). The workflow organizes the files, extracts and formats metadata, and 
packages the files. It may be used for one or multiple files of any file format. More specialized workflows have been 
developed for audiovisual materials and web archives.

(source: https://github.com/uga-libraries/general-aip)

## Getting Started

### Dependencies
Provide a list of packages or external libraries required for this code to run. We default to 
[PyCharm's default requirements settings](https://www.jetbrains.com/help/pycharm/managing-dependencies.html).

***Example:*** 
- bagit.py (https://github.com/LibraryOfCongress/bagit-python). Follow install instructions in the README.
- FITS (https://projects.iq.harvard.edu/fits/downloads). Configure as indicated below
- [PySimpleGUI](https://github.com/PySimpleGUI/PySimpleGUI) - The GUI used
- [ArchivesSnake](https://github.com/archivesspace-labs/ArchivesSnake) - Library used for interacting with the 
ArchivesSpace API


(source: https://github.com/uga-libraries/general-aip, 
https://github.com/uga-libraries/ASpace_Batch_Export-Cleanup-Upload)

### Installation
This section should explain how a user can download the code, install any dependencies (like packages, code bases (
Python, Ruby, etc.) or external libraries, can also reference the requirements.txt file if available), set up any 
configurations (like API keys or logins), and run the code. Additionally, make sure to include any account setup info, 
such as links to external services, such as Archive-It or ArchivesSpace. We generally expect users to know how to use
GitHub and download Python, so anything beyond that should be included here.

***Example:***
- Install the dependencies (listed above). For Windows, add 7-Zip to your Windows System PATH. In settings, go to 
Environment Variables > Path > Edit > New and add the 7-zip folder.
- Download this repository and save to your computer.
- Use the configuration_template.py to make a file named configuration.py with file path variables for your local 
machine.
- Change permission on the scripts so they are executable.

(source: https://github.com/uga-libraries/general-aip)

### Script Usage/Arguments
List any script arguments for the code here. If you have a collection of scripts with different arguments, break this 
section for each script and list out the requirements.

***Example:***

Script usage: python warc_download.py date_start date_end

    dates: the store date range for WARCs to be downloaded.
    date_start is inclusive: the download will include WARCs stored on date_start.
    date_end is exclusive: the download will not include WARCs stored on date_end.

(source: https://github.com/uga-libraries/web-aip/tree/github-requirements)

### Testing (Optional)
Outline any testing procedures or unittests that are integrated within the repo. If testing is a procedure, link to 
the procedure in this section. If you use unit testing, make sure to refer to those unit tests and include any special 
information for developers.

## Workflow
Generally describe how the program works from start to finish. Generally include expected inputs, how the code processes
data or goes through the workflow, and expected outputs. If the workflow is already written or in more detail elsewhere,
link to that documentation here - rather than duplicating the info or summarizing.

***Example:***
1. Extracts the department, collection id, folder name, AIP id, title, and version from metadata.csv.
2. Deletes temporary files from anywhere within the AIP folder because they cause errors with validating bags.
3. Creates the AIP directory structure. The AIP folder is named with the AIP ID and contains metadata and objects 
folders.

(source: https://github.com/uga-libraries/general-aip)

## Author
State your name, institution, and job title. This is so that anyone looking to ask questions outside opening up an Issue
has a person to reference for questions.

## Acknowledgements
A bullet-point list of any person, community, or resource who assisted in the making of this repository. This can also 
be the place to describe previous repositories or workflows that influenced the making of this repository.

***Example:***

These scripts were adapted from a set of two bash scripts that were used for making AIPs from 2017-October 2019 at UGA 
Libraries. (https://github.com/uga-libraries/aip-mac-bash-fits)

- Adriane Hanson - Head of Digital Stewardship at the University of Georgia Libraries
- ArchivesSpace community
- Kevin Cottrell - GALILEO/Library Infrastructure Systems Architect at the University of Georgia Libraries
- PySimpleGUI

(source: https://github.com/uga-libraries/general-aip, 
https://github.com/uga-libraries/ASpace_Batch_Export-Cleanup-Upload)

## History (Optional)
Include this section if it would be beneficial to include information about the project's context in your institution. 
This could mean talking about previous workflows or code that served the same or similar purpose and why this project 
and repo was made.

***Example:***

First developed in 2023 by the Digital Stewardship Unit (Adriane Hanson, Corey Schmidt, Emmeline Kaser) to consolidate 
our GitHub practices after a few years of maintaining code and documentation in GitHub.

(source: https://github.com/uga-libraries/GitHub_Standards#history)