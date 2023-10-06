# Title
When it's relevant, this first section can include contextual or background info for the workflows being described. May include a brief summary of the workflow's history and the roles responsible for it.

Example:
> The following processes were instituted in August 2022. Digital archives processing is the responsibility of the digital archivist in the Digital Stewardship unit.
> 
> This is a unified workflow that receives born-digital archival material from both the Russell and Hargrett libraries. The digital archivist works in collaboration with each library's collecting archivists to properly address sensitive information and provide an appropriate level of description for each collection.

## Overview
A brief description of the workflow documented in the repository, including any other repositories that the documentation references. 

Example:
> Processing actions are defined here as processes that prepare born-digital archives for ingest into permanent digital preservation storage and subsequent researcher access. Processing begins after all digital components in a collection are accessioned and appraised.
> 
> This documentation references Python scripts in the accessioning-scripts repository in the UGA Libraries GitHub.

## Purpose
A numbered list of goals that the workflow accomplishes. This is not a step-by-step procedure, but a condensed list of the most high-level outcomes. 

Example:
> 1. Create a processing plan. 
> 2. Arrange material into AIPs. 
> 3. Address any imminently at-risk formats, if necessary. 
> 4. Address any sensitive information. 
> 5. Create, document, and properly store any altered access copies (DIPs). 
> 6. Document all decisions and actions performed on a collection. 
> 7. Generate file inventories for each DIP. 
> 8. Turn arranged materials into AIPs and ingest into the digital preservation system. 
> 9. Perform subject analysis for description purposes, if necessary. 
> 10. Update and publish the finding aid.

## Procedure Overview
A step-by-step, numbered workflow that accomplishes the goals laid out in the "Purpose" section. This section should include links to any relevant scripts. It can also link to more in-depth markdown files for complex sub-processes within the workflow as needed. (For example, the step "Generate an initial file manifest using technical-appraisal-logs.py" may link to another markdown file that includes granular steps for running the script and cleaning up or adding to the resulting logs.) Separate documents should also be created when contextual or background info is needed for a certain process. These files should be saved to the same documentation repo.

## Documentation Overview (Optional)
A bulleted list of the documentation produced by the workflow. This section may or not be relevant depending on the process. 

## Policy Revision History
This section should provide a brief narrative history of the workflow/processes before they were published and include any authors and their roles. It can be updated with summaries of major updates, but GitHub's version control features are sufficient to document smaller and more routine updates.

Example:
> The first born-digital processing workflow was documented in the Hargrett and Russell libraries' "Electronic Records Processing Manual" created in 2013 by Adriane Hanson (Head of Digital Stewardship). Additional documentation and scripts were created by Brandon Pieczko (Processing and Digital Archivist, Russell Library) in 2019. This documentation supersedes the prior suite of born-digital processing documentation created at that time.
> 
>The initial version of this workflow was completed in August 2023 by Emmeline Kaser (Digital Archivist, Digital Stewardship) and represents the processes in place starting in August 2022. This workflow draws conceptually from older documentation but supersedes those processes due to changes in technological capabilities.