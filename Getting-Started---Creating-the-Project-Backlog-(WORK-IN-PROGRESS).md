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

## Breaking Down Tasks

Once you have an idea of what very high level components make up your project you will need to start defining the tasks that must be completed to build them. In traditional Software Development Lifecycle (SDLC) project management methodologies the result was called the *_work breakdown structure (WBS)_* which was typically just a list of the tasks, their relationship to one another, and estimate of time for completion, and who they were assigned to. In SDLC all tasks were defined at the start of the project allowing the project manager to provide an accurate estimate of cost and target date for the project. However, over time it has been proven that for many types of projects this highly structured and rigid approach simply doesn't work.

Agile project management (of which Scrum is one methodology) is based on the fact that "you don't know what you don't know" at the start of the project and as you progress more details will surface that you'll need to react and adapt to. Agile 

The first thing I’d suggest  is to start breaking down your project into discrete tasks. These should be small and achievable in a single sprint. Next, organize them based on their dependencies so they are performed in the right order. For example, you’ll probably want to complete your ‘Create Thing’ page before starting in on a ‘Search for Thing(s)’ page.
 
I like to define tasks as a story of the form “As a <persona> I want <requirement> So I can <value-statement>“. These describe what needs to be done in a fashion that directly relates the task to the individual that will gain the value from it. For example, 

As an Idea Creator 
I want to provide the URL’s to any supporting diagrams. URL’s should have a plain text description in addition to the URL itself.
So I can quickly and easily provide reviewers with more detail about my idea (