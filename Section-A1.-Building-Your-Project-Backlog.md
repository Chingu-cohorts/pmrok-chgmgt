## User Stories

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