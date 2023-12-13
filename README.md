# AI-Project-Framework
AI project framework, informed by Gitlab Maturity

## Workflow
Workflow is a combination of github issues, tags, project, and built-in automation. This workflow is setup for Github, but the framework could be replicated in other systems. I like github because it keeps the data scientists working and planning in the same environment. 

- [Best Practices](#best-practices)
- [Issue Templates](#issue-templates)  
- [Setting up the Workflow](#setting-up-the-workflow)
- [Tool Recommendations](#tool-recommendations)

### Best Practices
Having a mature AI organiation involves building AI with a streamlined, task-focused approach. Instead of concentrating on features and sprints, the emphasis is on tasks and their priority, which makes Kanban an ideal method.

The advantage of integrating the AI workflow into a Source Code Management (SCM) tool, like this (or GitLab), is that it aligns closely with the developer's existing workflow. This is especially beneficial for data scientists who are encouraged to enhance their coding practices.

While many templates exist for managing code and tasks at this level, the key is to establish standard practices across issues, Kanban boards, and workflow tracking. This ensures not only consistency but also adds significant value to the project management process.

Milestones can then be used to bucket work tasks into levels of priority and set a timeline for which to team to work towards. 

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

### Setting up the Workflow 

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

#### 4. Create First Milestone

Create a milesone in github repo. This will be your buckets of work that you can priorite tasks and bugs into. Pick a reasonable date for current workstream. This date might be a release date of a company feature, update milestone for leadership, or something else. Its really just a line in the sand the team agrees to work within. 

#### 5. Create First Task
- Create new issue
- Select Task issue type
- Add title and detail content
- Add tag(s) of associated AI stage
- Add milestone based on priority, none if task is in parking lot

#### 6. Rinse and Repeat

Use this for all tasks or bugs (or add your own types that make sense) for the AI project. 

### Tool Recommendations

#### Experiment Tracking
If you don't know what experiment tracking is checkout Neptune.ai's blog post [here]([url](https://neptune.ai/blog/ml-experiment-tracking)https://neptune.ai/blog/ml-experiment-tracking). Ultimately, if you already have something for experiement tracking keep using it, can expand the data you collect. Note, the tool you pick here does not suddenly give your team a massive competative advantage, pick something that works for your system today and don't over index on the decision. 

- My choice: [MLflow](https://mlflow.org/).
It's probably the easiest to use and most flexible. If you are interested in a manged offering you can leverage with Databricks. 

Other options (not exhaustive):
- [DVC](https://dvc.org/)
- [Comet ML](https://www.comet.com/site/)
- ...

#### Data Mangement
- My choice: [DVC](https://dvc.org/)
Again, lots of options, but this is easy to setup, use and gets you moving quickly. 

Other Options (not exhaustive):
- [Dolt](https://github.com/dolthub/dolt)
- [Feast](https://feast.dev/)
- ...
