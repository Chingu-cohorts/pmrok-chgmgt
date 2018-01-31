TBD

#Overview: Chingu-Voyage Build-to-Learn Roadmap
### Act 1 
**Milestones**

#1 — Meet the Team

#2 — Set Goals & Expectations 

#3 — Brainstorm Project Options

#4 —Define your Workflow

#5 — Set up

#6— Define the MVP 

### Act 2
**Milestones**

#1 — Plan the Sprint

#2 — Begin the Sprint

#3 —Team Standup Review

#4 — Sprint Progress Review

#5 — Code Review & Merging

#6 — Completed Sprint Review

### Act 3 
TBD
------
# Defined: Chingu-Voyage Build-to-Learn Roadmap

### Act 1 
**Milestones**

#1 — Meet the Team

What: 

Resources: 

-[Virtual Icebreakers for Remote teams](https://www.collaborationsuperpowers.com/44-icebreakers-for-virtual-teams/)
-[Ice-breaker questions](https://docs.google.com/document/d/1tBCjXMBXpD3M2uC90_Z3B7kfPjaxMoWS8v5uHLu3ASQ/edit?usp=sharing)  

#2 — Set Goals & Expectations 

It's important that the team "has the same picture in their heads" as far as goals & expectations go. Common questions to ask for this are: What does success look like for this project? How much time can you expect me to work on this project each week? What tech-stack am I familiar with? 

#3 — Brainstorm Project Options

Resources: 

- [Chingu Voyage Project Prompts](https://medium.com/chingu/chingu-voyage-3-team-projects-lineup-9c3380709d77)

#4 —Define your Workflow

#5 — Set up

#6— Define the MVP 

### Act 2
**Milestones**

#1 — Plan the Sprint

#2 — Begin the Sprint

#3 —Team Standup Review

#4 — Sprint Progress Review

#5 — Code Review & Merging

#6 — Completed Sprint Review

-----

# How can I define and assign tasks to my team? 

## Introduction

When you start a new project one of the first things you'll need to do is to define the tasks that must be completed to meet the projects goals. As a PM the very first step is to brainstorm with your team to define who your users are, the value the app will bring to each of them, and the high level components of the app responsible for delivering this value.

## Workflow
Once you've done this the next step is to start defining more discrete tasks and adding them to your project backlog. What is a "backlog"? Very simply its just a place where you maintain the tasks your project needs to complete, but which haven't yet been started. Agile projects organize themselves around a project board that's consists of the following vertical lanes:

- Backlog - the stories we know we need to do, but haven’t gotten to yet
- Next - the stories we know need to be performed in the next Sprint. If we complete all the stories in the current sprint we’ll go here to get more work before dipping into the backlog
- In Progress - The stories that have to be completed in the current Sprint. Don’t overload this with stories! at the beginning of the Sprint you’ll need to decide as a team what needs to be done in the upcoming sprint
- Blocked - Stories that have been started, but can’t be completed due to an unfulfilled dependency on another story or due to a decision that needs to be make, or a technical issue. These should be resolved as quickly as feasible so you don’t accumulate technical debt.
- Done - Stories that have been completed. It’s important to move a story card to this lane only with the story is fully completed - Coded, tested, and promoted to your release branch

This is also known as a Kanban board and it imposes a workflow to your project that gives you visibility to the progress of the project based on the state of its tasks. 

## Sprints

With an Agile approach you will divide the time between the start of your project and its delivery date into *_sprints_* of equal duration in which you'll be completing tasks. At the start of each sprint you and your team will review the backlog and choose the tasks that must be completed in the new sprint. If you complete all of these before the end of the sprint then you'll start new tasks, one-at-a-time, from your backlog to fill the remaining time.

Dividing your project in this way and planning and executing in a progression allows the team to adapt to change and to start tasks at the optimal point in time when enough details are known to allow development to be both efficient and result in something that is relevant.

## Building the Backlog

Building the backlog of tasks involves breaking down your project into discrete tasks. A good place to start is to treat every page in the app as a component and organize them in a logical sequence based on their dependency to one another. For example, you’ll probably want to complete your ‘Create Thing’ page before starting in on a ‘Search for Thing(s)’ page.

Once you've done that define a *_user story_* for each unit of work needed to build the components. These should be very discrete and each one should be able to be completed in a single sprint. User stories are not expressed in technical terms. Instead they identify the persona that will use the delivered piece of functionality, what that requirement is, and the value they will realize from it. This may sound very foreign to you in your role as a WebDev, but its critical to ensuring that your product delivers value to the end user. The most technically beautiful implemented app is useless if it doesn't deliver on this value proposition.

User stories help you to define what both "good" and "done" mean with respect to the development of your application.

Stories are simple statements having a form such as:
```
As a <persona> 
I want <requirement> 
So I can <value-statement>
```
For example,
```
As an Idea Creator 
I want to provide the URL’s to any supporting diagrams. URL’s should have a plain text description in addition to the URL itself.
So I can quickly and easily provide reviewers with more detail about my idea
```
Even though the story is expressed in non-technical terms this doesn't mean that you can't annotate it with technical details as they become known. Many of the tools you have at your disposal allow story cards to contain additional information. However, while documentation is important keep in mind that Agile values working code over comprehensive documentation this doesn't mean you don't produce documentation. It means you produce it at the right level of detail and at the right time.

Many teams do find it useful to annotate the user stories with very high level checklists listing the steps to be completed for the story and the order they are to be completed in. It's important to keep in mind that these define what is to be done and not how it is to be done. It's just as important to first concentrate on building the user stories before starting work on defining the steps involved in each story.
```
As an Idea Creator
I want to provide the URL's to any supporting diagrams. URL's should have a plain text description in addition to the URL itself.
So I can quickly and easily provide reviewers with more detail about my idea
[] Define the constraints for the URL and its description
[] Define layout of these fields on the Idea screen
[] Create component to support capture, display, and edit of these fields
[] Add these fields to the database
[] Add support for maintaining this information in the various backend idea routes
```
Remember that the focus of the user story is to classify who your users are, what functionality they require, and the value each function will deliver.

## Backlog Grooming

Once you have defined your initial backlog of tasks you can start your first sprint as previously described. With each team meeting and each sprint you will be updating the backlog with new information that comes to light. This will involve adding, modifying, and even removing stories. You'll find that some stories aren't granular enough and must be broken up into additional stories, you'll find than stories you thought were completed need to be moved out of the Done lane on your project board and back into In Progress. In short, keeping the backlog relevant is a never ending task while the project is underway.

## Wrapping It Up

This has been a very light introduction to Agile project management and has been focused on practical steps to get your project to the point where you can start Sprint 1. Just as there are many paths to failure there are also many paths to success. As Chingu PM's its your responsibility to share what you've learned with your peers. Feel free to add your lesson's learned to this wiki.

Good luck on your projects! 

