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