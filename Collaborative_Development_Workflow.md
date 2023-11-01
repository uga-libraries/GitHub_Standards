# Collaborative Development Workflow

## Overview 

This workflow supports collaborative development of scripts by Libraries’ employees who are not full-time developers. 
It adapts concepts from agile methodology to the situation where everyone is working on the project intermittently, 
to keep momentum and support communication. 

In the context of the Digital Stewardship unit, born-digital archiving workflows can be enhanced through scripting, 
and efficient development of the more involved scripts requires consistent blocks of time. 
In those cases, the Digital Archivist acts as the product owner and Head of Digital Stewardship as the primary developer. 
When time allows, the Digital Archivist also assists with development.

## Terminology 

- **Development Cycle:** timeframe for working on the script, kickoff through retrospective 
- **Developer:** writer of the code 
- **Issue:** space in GitHub to describe things to fix and ideas for changes 
- **Kickoff:** first meeting in the cycle, to establish goals and plan the work
- **Milestone:** key goal for the development, like completing a feature 
- **Product Owner:** user of the code, person with subject/workflow knowledge 
- **Production:** used for real to do work 
- **Proof of Concept:** a kind of milestone; a rough test to show what something might be like 
- **MVP:** a kind of milestone; the minimum features needed to use in production 
- **Sprint:** a development period, with a set of issues to accomplish 
- **Retrospective:** reflecting on the process 

## Workflow

1. Kickoff meeting 
2. Series of sprints (1-2 months each)  
    a. Development   
    b. Review (product owner)  
    c. Sprint meeting
3. Finalize GitHub repository (developer) 
4. Retrospective meeting 

## Communication 

### GitHub Issues 

GitHub is the primary method of communication. 
Issues are used to track all desired features or changes to the script.
The developer and product owner record major decisions and answer questions as comments on the issue, 
and labels are used to track their priority and progress. 

GitHub is preferred over email or in-person chats because it is asynchronous 
(allowing people to give attention at their earliest convenience, balancing interruption and keeping development going) 
and produces a record of the decision for future use. 

### Teams/Document Storage 

Digital Stewardship makes a Teams folder within Programming for the temporary documentation. 
This includes the meeting notes, test files, and any other temporary documentation.
At the end of the development cycle, copy any information (major decisions, ideas for additional functionality) to GitHub 
and delete everything from Teams. 

### Meetings 

There are a few meetings throughout the development cycle to plan the work and review progress.
The development cycle starts with a kickoff meeting to set the goals. 
At the end of each sprint, meet to evaluate the work completed and select work for the next sprint. 
The development cycle ends with a retrospective meeting to reflect on the process.

#### Typical Kickoff Meeting Agenda

1. What the script needs to do and how it fits into the workflow 
   - Might be a new script or adding functionality to an existing one
   - For automating a workflow, consider a workflow diagram or outline
   - To define functionality, consider user stories: as a _ROLE_, I _WANT/NEED/CAN GOAL_ so that _REASON_
2. How much time we have to spend on development 
3. Outline milestones  
   - Proof of concept 
   - Sometimes one or more related to key functionality 
   - MVP: everything required to use it in production 
   - Sometimes one or more related to bonus functionality
4. Schedule sprint meetings for each milestone
5. Make a new GitHub repo, if needed
6. Decide what to work on for the first sprint and set up GitHub issues for them

#### Typical Sprint Meeting Agenda 

1. Review completed issues and close if approved 
2. Merge the sprint branch to the development branch (it may be main) 
3. Review and adjust milestones, if needed (MVP especially may evolve) 
4. Identify issues for the next sprint 
5. Discuss the goals of each issue and add comments to further define the issue

#### Typical Retrospective Meeting Agenda 

1. Future Considerations 
2. Accomplishments 
3. Lessons Learned 
4. Problem Areas (pick one problem and identify solutions for next time) 
5. Review issues: any to add or close? 
6. For new scripts, establish a maintenance cycle 
7. Make GitHub Repo public, if it isn’t already 

Retrospective resources:
- [Agile: Virtual Retrospectives - 8 Retro Templates](https://www.linkedin.com/pulse/agile-virtual-retrospectives-8-retro-templates-you-elaine)
- [Atlassian Team Playbook: Retrospective](https://www.atlassian.com/team-playbook/plays/retrospective)
- [Guide to agile retrospectives](https://www.aha.io/roadmapping/guide/agile/what-is-an-agile-retrospective)   
- [Sprint Retrospective Meeting](https://blog.trello.com/sprint-retrospective-meeting)

## GitHub Usage 

We use GitHub as the primary method for tracking the development work, for communicating about priorities and issues, 
and as the permanent documentation of this process.

During the kickoff meeting, determine if a new GitHub repo is needed or if it will be added to an existing repo. 
For new repos, keep it private until it is ready for production. 
For existing repos, keep it public. 

At the end of the cycle, make sure that the GitHub repo meets [our GitHub Standards](Repository_Standard.md), 
that the README and documentation are complete, and that remaining ideas have been documented as issues. 

### Branches 

If the script is in production, and you don’t want to alter the main branch until after the end of the development cycle, 
make a branch for the development cycle. 
This lets us test that there are no conflicts between different changes prior to moving the new changes into production at the end of the cycle.

At the start of each sprint, make a branch for the sprint from the branch for the development cycle (if any) or main. 
The sprint branch is a space to stage completed development for review by the product owner. 
During review, the developer can begin working on another issue in a branch off the sprint branch without changing what the product owner sees.  

Make a branch from the sprint branch for each issue as you work on it and associate the branch with that issue. 
This clarifies the purpose of each branch and shows that each issue is addressed.  

When work is complete on an issue, merge its branch back into the sprint branch. 
This lets the developer address any conflicts with other completed portions of the development prior to review. 

When the work is reviewed and accepted (usually at the next sprint meeting), 
merge the sprint branch into the development cycle branch or main branch. 

### Issues 

GitHub issues are the central place to document all desired changes. 
Make an issue for every idea, even if you aren’t sure you’ll do it, so everything is in one place and easier to prioritize. 
It also ensures that ideas are not forgotten while allowing the developer to stay focused on the purpose of the sprint. 
The first issues are created during the kickoff meeting, 
and additional ideas are added throughout development by the developer and product owner.  

Use comments to summarize major development decisions and save links to resources used for sections of code (e.g., StackOverflow) as permanent documentation of the development process. 
Also use comments to get additional information from the product owner (@ to send notification), 
which will create a record of the decisions, and to notify them that an issue is ready to be reviewed. 

Use labels to organize issues functionally (e.g., same document, same kind of change), mark priority, and track progress (Review, Approved). 
We use the label "streamline" for ideas to simplify the code but not change the functionality, which can be done during any sprint if there is extra time.
Track which issues are in the current sprint by assigning the issue to the developer.

### README 

This document summarizes the script and how to use it.
Use the [Code README Template](Code_README_Standard.md) to organize the README.  

If the GitHub repo is already public, add a note to the top of the README at the start of the development cycle indicating that it is undergoing development. 
If this is a new repository, add information to the README as you go about script arguments, dependencies, etc. 
to make it easier to finish the README at the end of the development cycle.