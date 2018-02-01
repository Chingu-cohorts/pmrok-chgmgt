## What is a PM?

An Agile PM is responsible for managing the resouces, time, and scope that
make up a project to ensure that a quality product is delivered within the
desired schedule and budget. A Chingu PM doesn't just coordinate the project. 
She also acts as a member of the development team writing code, testing the
app, and creating documentation.

An important difference between a PM in a corporate setting and yourselves is
that since we are operating in a volunteer environment just like every Open
Source project you are also a coach, a motivator, and a role model. We can't
order our team mates we must establish and environment that motivates them to
be both innovative and productive.

In your role as a Chingu Project Manager’ your most important two tasks are to
understand your teams needs and to remove any obstacles blocking their progress.
This requires a large amount of communication and a deep understanding of what
resources, including people, are available in the Chingu organization.

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

-----

### Agile vs. SDLC Project Management - What's the difference?

Once you have an idea of what very high level components make up your project you will need to start defining the tasks that must be completed to build them. In traditional Software Development Lifecycle (SDLC) project management methodologies the result was called the *_work breakdown structure (WBS)_* which was typically just a list of the tasks, their relationship to one another, and estimate of time for completion, and who they were assigned to. In SDLC all tasks were defined at the start of the project allowing the project manager to provide an accurate estimate of cost and target date for the project. However, over time it has been proven that for many types of projects this highly structured and rigid approach simply doesn't work.

Agile project management (of which Scrum is one methodology) is based on the fact that "you don't know what you don't know" at the start of the project and as you progress more details will surface that you'll need to react and adapt to. Agile methodologies are based on the following principles which contrast them to traditional SDLC approaches:

- Individuals and interactions over processes and tools
- Working software over comprehensive documentation
- Customer collaboration over contract negotiation
- Responding to change over following a plan

----

# Getting Started: Issue Reporting and Tracking

# Introduction
The PMRoK Project uses GitHub not only for source code management, but also for issue reporting. The purpose of the following guidelines is to provide guidance on how to report an issue. You might be asking yourself "How hard can this be?". You might be surprised to find out how often bad issue reports are actually created. Here are some examples:

- "The profile screen doesn't work right. Please correct this asap."
- "When I hit the Option-B key combination nothing happens."
- "Damnit how many times must I ask for this frigging software to work right. On the account entry screen the phone number textbox doesn't accept a country code"

The problem with the first two examples are they don't describe what the error actually is or where it's occurring within the application. The second example is marginally better since it defines how to recreated the problem, but that information is useless since there's still no indication of which screen the user was on when Option-B was attempted.

The last issue report is the best of the three since it defines which screen the user experienced the issue on, what she was trying to do, and what the expected outcome was. Unfortunately the first sentence is totally useless information that's inappropriate for an issue report and sends a signal to whoever works on this issue that the user is going to be difficult to work with. The lesson here is that issue reports should be factual and not emotional. 

# Issue Reporting Template
The result of having the complete, accurate, and appropriate information is that the Developer will be able to resolve the issue faster and more correctly. The key information that should be entered into the issue are:

- Description of what occurred and what the desired outcome should have been.
- Summary of the symptoms including screenshots and logs, if available.
- List of steps the Developer can follow to recreate the problem. This should include not only navigation steps, but also data values that are to be entered. 

The information above should be entered by the individual that report's the issue. When the issue is resolved the Developer is responsible for describing how the issue was resolved along with any supplemental information that may be useful to other Developers if the issue should reoccur in the future.

To help ensure that this information is properly captured we ask our users and developers to use the following template when creating issues for PMRoK. Simply copy and paste this into new issues and then enter information about your issue in the appropriate section.
```
**_Issue Description & Expected Outcome:_** 

**_Symptoms:_**

**_Steps to Recreate:_** 

**_Resolution:_** 
```
# The Importance of Labels
Having the complete and accurate information that describes an issue is important, but so is classification of the issue. Classifying or grouping issues into categories helps the Development team to triage issues so they are worked on in the proper order. 

This project uses GitHub Issue Labels for classification. These labels and their definitions are shown below.
```
Label                 Description 
--------------------  ---------------------------------------------------------
                      Issue type
type:bug              ..A defect resulting in a deviation from expected results
type:documentation    ..A defect in documentation or need for additional clarity
type:enhancement      ..Request for an minor enhancement
type:feature request  ..Request for a major new feature
type:question         ..A question to the Development Team
type:refactor         ..Request by Developer to modify how the code currently
                        accomplishes a given function.
                      Priority
priority:must have    ..Significant impact to user requiring ASAP resolution.
                        Users are encouraged to describe the impact in the
                        issue description.
priority:should have  ..Issue has an impact to the app that detracts from it's usefulness, but a work around exists.
priority:nice to have ..Issue has no longterm impact to the effectiveness or value of the app, but would improve it.
                      Status
status:on hold        ..Deferred, unable to resolve at this time.
status:duplicate      ..Duplicate issue. Development team will add this tag along with the issue number of the original problem report, then close the duplicate issue.
                      Scope of Development Effort
scope:story           ..Small or trivial unit of work
scope:epic            ..Moderate amount of work that consists of multiple user stories and may span more than one sprint.
scope:saga            ..Considerable effort required that consists of more than one epic and spans multiple sprints.
```
Issue Type and Priority labels are to be assigned by whoever creates the issue. Status and Scope labels are maintained by the Development Team.

# Examples
The best source of examples for how issues are to be defined and labeled is the [PMRoK Issue Log](https://github.com/Chingu-cohorts/pmrok/issues).

------

# Up & Running: Team Documentation

One of the foundations of the [Agile Manifesto](http://agilemanifesto.org/) is that Working software is valued over comprehensive documentation. This has led to the misconception that Agile methodologies, like Scrum, produce only code and not documentation. In fact, Agile methodologies promote the production of documentation at the right point in time and at the right level of detail. 

Generally speaking the "right point in time" is when the necessary details are stable enough to produce documentation that will not require later revision. You may need to keep notes as your sprints progress so you'll have the information you need to create usable documentation, but you won't create that documentation until the details have been defined and are stable.

The "right level of detail" means that you don't want to create documentation just for the sake of producing documentation. Your goal should be to produce just the documentation users need and no more. It also means that what you produce must be concise and to the point. Diagrams and pictures are generally used to convey information the user needs to know with words used sparingly.

As an example consider the following diagram produced by @zashishz for the Voyage3 Toucans-26 team to document their Git workflow. 

![Team Git Workflow](https://github.com/Chingu-cohorts/pmrok/blob/development/diagrams/Git%20Workflow%20Diagram%20Example.png)

This diagram shows the reader everything he or she needs to know regarding how they are expected to conduct their day-to-day development tasks with respect to Git and GitHub.
