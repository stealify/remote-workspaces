# remote-workspaces
A Multi User Multi Group Developer Workflow

## Goals
Use a Single IDE to Connect to a Remote Host and Configure Workspaces Containers and SSH Access handle the url routing for the dev environments
and finaly allow the developer to focus on his main coding task. 


## Scenario 1 (Wordpress Development) Multiple Developers own Forks sharing and not sharing db instances
Lets Assume your running a Big Wordpress Project with many new Extension Upgrades lets say Daily or even Hourly.
Lets Assume your working with multiple agencys each has 5 developers working on diffrent plugins/templates/chor and parts of that.

Each Developer needs to access a Common Pool of Projects (git) fork it and setup the correct dev environment for that using the Company Resources supplyed to the developer. So that no code gets transfered by that workflow without knowing about that to the external company that does the dev task.

Also it should not be needed to brief the External Dev Team about the environment they should get Everything out of the Box while they should be able to use the Favorit IDE That they are currently using

what is needed? 

- Ability to configure Domain Resolution and or at last URL Resolution for the remote host. (Already do able via remote-ssh)
- Ability to configure Remote Users and Permissions (Already do able via remote-ssh)
- Connect IDE Logic to the remote-host logic fs views search (execute commands and show the response in the IDE)
- a collection of code that executes commands on the remote host and gives feedback back to the ide
- protocols and definitions how to talk to that remote-host with other methods then ssh. (WebRTC DataChannels)
