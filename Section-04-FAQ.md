
You may be thinking "Ok, I'm the PM, what the ?!?$ do I do now??? What should I expect?"

Here are a few reflections from past Chingu Project Managers (who once felt the same as you): 

- [Ben's video: on his PM experience](https://www.youtube.com/watch?v=6TsFBW-c6to&feature=youtu.be)
- [Olly's article: Taking the reins: A Junior Developer’s voyage as a PM](https://medium.com/chingu/taking-the-reins-a-junior-developers-voyage-as-a-pm-c2883ae04467)


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

-----


### Agile vs. SDLC Project Management - What's the difference?

Once you have an idea of what very high level components make up your project you will need to start defining the tasks that must be completed to build them. In traditional Software Development Lifecycle (SDLC) project management methodologies the result was called the *_work breakdown structure (WBS)_* which was typically just a list of the tasks, their relationship to one another, and estimate of time for completion, and who they were assigned to. In SDLC all tasks were defined at the start of the project allowing the project manager to provide an accurate estimate of cost and target date for the project. However, over time it has been proven that for many types of projects this highly structured and rigid approach simply doesn't work.

Agile project management (of which Scrum is one methodology) is based on the fact that "you don't know what you don't know" at the start of the project and as you progress more details will surface that you'll need to react and adapt to. Agile methodologies are based on the following principles which contrast them to traditional SDLC approaches:

- Individuals and interactions over processes and tools
- Working software over comprehensive documentation
- Customer collaboration over contract negotiation
- Responding to change over following a plan
