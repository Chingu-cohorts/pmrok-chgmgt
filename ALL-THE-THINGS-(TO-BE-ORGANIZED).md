# Editing Section 01 Getting Started: Issue Reporting and Tracking

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

# Section 04 Up & Running: Team Documentation

One of the foundations of the [Agile Manifesto](http://agilemanifesto.org/) is that Working software is valued over comprehensive documentation. This has led to the misconception that Agile methodologies, like Scrum, produce only code and not documentation. In fact, Agile methodologies promote the production of documentation at the right point in time and at the right level of detail. 

Generally speaking the "right point in time" is when the necessary details are stable enough to produce documentation that will not require later revision. You may need to keep notes as your sprints progress so you'll have the information you need to create usable documentation, but you won't create that documentation until the details have been defined and are stable.

The "right level of detail" means that you don't want to create documentation just for the sake of producing documentation. Your goal should be to produce just the documentation users need and no more. It also means that what you produce must be concise and to the point. Diagrams and pictures are generally used to convey information the user needs to know with words used sparingly.

As an example consider the following diagram produced by @zashishz for the Voyage3 Toucans-26 team to document their Git workflow. 

![Team Git Workflow](https://github.com/Chingu-cohorts/pmrok/blob/development/diagrams/Git%20Workflow%20Diagram%20Example.png)

This diagram shows the reader everything he or she needs to know regarding how they are expected to conduct their day-to-day development tasks with respect to Git and GitHub.
