# AI-Project-Framework
AI project framework, informed by Gitlab Maturity

## Workflow
Workflow is a combination of github issues, tags, project, and built-in automation. This workflow is setup for Github, but the framework could be replicated in other systems. I like github because it keeps the data scientists working and planning in the same environment. 


### Issue Templates
There are two issues types available. Tasks are actions that add function to the AI project. Bugs are problems found with the AI project.
- Task: Task relating to an AI project
- Bug: Bug with the AI project

Each issue is made up of 5 components:
- Title: Unique and descriptive title
- Content: Details of the task or bug
- Tags: Add the stage(s) associated with the issue
- Project: AI project kanban board of the AI team
- Milestone: Bucket of work based to enable the prioritization

#### Tags:
<img width="666" alt="Screen Shot 2023-12-13 at 12 34 59 PM" src="https://github.com/jfirminger/AI-Project-Framework/assets/9371702/4b425c19-c632-49e2-9f50-91833848f40e">

### Setting up Workflow
TODO

#### 1. Use this repo as template
Navigate to top left of [repo](https://github.com/jfirminger/AI-Project-Framework) and select 'use this template'. 

<img width="236" alt="Screen Shot 2023-12-13 at 12 45 41 PM" src="https://github.com/jfirminger/AI-Project-Framework/assets/9371702/5dd73331-fde4-4029-a550-31237a11e5c0">

This will provide you with a clean repo with the issue templates and tags built in. 

#### 2. Create Github project

Create a project in Github for your team. Make sure everyone can access the project.

#### 3. Setup Automations
- Navigate to project workflow page. use `...` button on top right of project page. 
- Ensure *Item added to project* is turned on
- Ensure *Auto-add to project*. use this query `is:issue,pr is:open label:"ai:task","ai:bug"`

Your project workflow page should look something like this:

<img width="1309" alt="Screen Shot 2023-12-13 at 12 51 10 PM" src="https://github.com/jfirminger/AI-Project-Framework/assets/9371702/967e8351-f993-4236-9c5f-5e315519befb">


