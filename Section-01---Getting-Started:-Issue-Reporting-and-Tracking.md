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


----------

# Section 02 Getting Started: How to Define and Assign Tasks to Your Team

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

## An Interlude: Agile vs. SDLC Project Management

Once you have an idea of what very high level components make up your project you will need to start defining the tasks that must be completed to build them. In traditional Software Development Lifecycle (SDLC) project management methodologies the result was called the *_work breakdown structure (WBS)_* which was typically just a list of the tasks, their relationship to one another, and estimate of time for completion, and who they were assigned to. In SDLC all tasks were defined at the start of the project allowing the project manager to provide an accurate estimate of cost and target date for the project. However, over time it has been proven that for many types of projects this highly structured and rigid approach simply doesn't work.

Agile project management (of which Scrum is one methodology) is based on the fact that "you don't know what you don't know" at the start of the project and as you progress more details will surface that you'll need to react and adapt to. Agile methodologies are based on the following principles which contrast them to traditional SDLC approaches:

- Individuals and interactions over processes and tools
- Working software over comprehensive documentation
- Customer collaboration over contract negotiation
- Responding to change over following a plan

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


# Editing Section 03 Up & Running: Managing Application Secrets

## Introduction

Every application has certain secrets, such as build instructions, passwords and SSH keys that could compromise the security and confidentiality of the app if made public. It is the responsibility of the Project Manager to ensure that these are maintained in a secure location and are available to a minimum of two team members. After all, given the fluid nature of team membership you don't want to wake up one day to find that no one on the team has access to the Production server.

Please note that the Guidelines presented below are sufficient to protect most private and commercial secrets, but are NOT sufficient for apps supporting many government departments and agencies such as the U. S. Department of Defense.

## Guidelines

- Assume that your team will forget the app secrets from time-to-time. Keep them in a secure place so you'll be able to produce them on demand.
- Never store confidential information in a public source code repository like GitHub.
- Set up a secure vault for the sharing of app secrets. For example, a tool like 1Password with strong encryption so you can store the password vault in a Cloud storage location without fearing that it can be easily compromised.
- Make sure that all members of the team use `.gitignore` to ensure that service accounts and passwords stored in local `.env` files are never pushed to the remote Git repo.
- Never communicate secrets through email. Use a realtime messaging service like Slack that encrypts the transmission of data. However, if you must use email use separate email messages for the name of the service, the account id, and the password. After sending the messages delete them from your local computer and if supported from any server-based components as well (like Slack channels).
- Never communicate secrets outside of your team. Always double check the recipient list prior to transmission to ensure that it will be sent only to authorized recipients.
- Never write secrets down on paper. Never write secrets down on paper. Never write secrets down on paper. Never write secrets down on paper. Never write secrets down on paper. Never write secrets down on paper. GOT IT?