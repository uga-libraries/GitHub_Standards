# Collaborative Development Workflow

## Overview 

This workflow supports collaborative development of scripts by Libraries’ employees who are not full-time developers. 
It adapts concepts from agile methodology to the situation where everyone is working on the project intermittently, 
to keep momentum and support communication. 

In the context of the Digital Stewardship unit, born-digital archiving workflows can be enhanced through scripting, 
and efficient development of the more involved scripts require consistent blocks of time. 
In those cases, the Digital Archivist acts as the product owner and Head of Digital Stewardship as the primary developer. 
When time allows, the Digital Archivist also assists with development. 
After the development cycle, the two have shared responsibility for ongoing maintenance. 

## Terminology 

Development Cycle: period for working on the script, kickoff through retrospective 

Developer: writer of code 

Issue: space in GitHub to describe things to fix and ideas for changes 

Milestone: key goal for the development, like completing a feature 

Product Owner: user of the code, person with subject/workflow knowledge 

Production: used for real to do work 

Proof of Concept: a kind of milestone; a rough test to show what something might be like 

MVP: a kind of milestone; the minimum features needed to use in production 

Sprint: a development period, with a set of issues to accomplish 

Retrospective: reflecting on the process 

## Workflow

1. Kickoff meeting 
2. Create or edit GitHub repository (developer) 
3. Series of sprints (1-2 months each)  
    a. Development   
    b. Review (product owner)  
    c. Sprint meeting
4. Finalize GitHub repository (developer) 
5. Retrospective meeting 

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
And the development cycle ends with a retrospective meeting to reflect on the process.

#### Typical Kickoff Meeting Agenda

1. What does the script need to do  
   - Might be a new script or adding functionality to an existing one
   - For automating a workflow, consider a workflow diagram or outline
   - To define functionality, consider user stories: as a _ROLE_, I _WANT/NEED/CAN GOAL_ so that _REASON_
2. How does this fit into the workflow overall
3. How long will we spend on development 
4. What have any of us done that is similar (as code reference) 
5. Identify test data needed for development 
6. Outline milestones  
   - Proof of concept 
   - Sometimes one or more related to key functionality 
   - MVP: everything required to use it in production 
   - Sometimes one or more related to bonus functionality
7. Schedule sprint meetings
8. Make a new GitHub repo or decide which to add it to
9. Decide what to work on for the first sprint

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
4. Problem Areas (identify solutions for one problem for next time) 
5. Review and update issues – any to add or remove? 
6. For new scripts, establish a maintenance cycle 
7. Make GitHub Repo public, if it isn’t already 

Retrospective resources:
- [Agile: Virtual Retrospectives - 8 Retro Templates](https://www.linkedin.com/pulse/agile-virtual-retrospectives-8-retro-templates-you-elaine)
- [Atlassian Team Playbook: Retrospective](https://www.atlassian.com/team-playbook/plays/retrospective)
- [Guide to agile retrospectives](https://www.aha.io/roadmapping/guide/agile/what-is-an-agile-retrospective)   
- [Sprint Retrospective Meeting](https://blog.trello.com/sprint-retrospective-meeting)