# Overview
This section should describe what this script/repository does, what is its purpose, and what the user should expect. 
It should be around three to five sentences in length. For repositories that are a collection of scripts with no 
unified purpose, describe what each script does briefly.

***Example:***
This is the general workflow to make archival information packages (AIPs) that are ready for ingest into the UGA 
Libraries' digital preservation system (ARCHive). The workflow organizes the files, extracts and formats metadata, and 
packages the files. It may be used for one or multiple files of any file format. More specialized workflows have been 
developed for audiovisual materials and web archives.

(source: https://github.com/uga-libraries/general-aip)

# Getting Started
## Dependencies
Provide a list of packages or external libraries required for this code to run or direct a user to the requirements.txt
file. Give an example of how to install the dependencies.

***Example:*** 
- bagit.py (https://github.com/LibraryOfCongress/bagit-python). Follow install instructions in the README.
- FITS (https://projects.iq.harvard.edu/fits/downloads). Configure as indicated below
- [PySimpleGUI](https://github.com/PySimpleGUI/PySimpleGUI) - The GUI used
- [ArchivesSnake](https://github.com/archivesspace-labs/ArchivesSnake) - Library used for interacting with the 
ArchivesSpace API


(source: https://github.com/uga-libraries/general-aip, 
https://github.com/uga-libraries/ASpace_Batch_Export-Cleanup-Upload)

## Installation
This section should explain how a user can download the code, install any dependencies (like packages, code bases (
Python, Ruby, etc.) or external libraries, can also reference the requirements.txt file if available), set up any 
configurations (like API keys or logins), and run the code.

***Example:***
- Install the dependencies (listed above). For Windows, add 7-Zip to your Windows System PATH. In settings, go to 
Environment Variables > Path > Edit > New and add the 7-zip folder.
- Download this repository and save to your computer.
- Use the configuration_template.py to make a file named configuration.py with file path variables for your local machine.
- Change permission on the scripts so they are executable.

(source: https://github.com/uga-libraries/general-aip)

## Workflow
Generally describe how the program works from start to finish. Generally include expected inputs, how the code processes
data or goes through the workflow, and expected outputs.

***Example:***
1. Extracts the department, collection id, folder name, AIP id, title, and version from metadata.csv.
2. Deletes temporary files from anywhere within the AIP folder because they cause errors with validating bags.
3. Creates the AIP directory structure. The AIP folder is named with the AIP ID and contains metadata and objects 
folders.

(source: https://github.com/uga-libraries/general-aip)

## Testing
Detail how a user or developer can test the code to make sure it is running as intended. This can include a link to 
external testing documentation or a list of step-by-step instructions.

***Example:***
- In the barcode box, enter "320121158842"
- Select your repository and click save
- Select the file in Select DLG>ASpace Template button
- Click "START"
- The program may be unresponsive, but it should generate a new file and open the location of the file once done

# Author
State your name, institution, and job title. This is so that anyone looking to ask questions outside opening up an Issue
has a person to reference for questions.

# Acknowledgements
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