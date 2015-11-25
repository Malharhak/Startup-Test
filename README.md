# Startup-Test
The checklist of stuff that a startup should do

##Project Management

* Do you let members of the team participate in planning and estimating the tasks?
* Do you collect enough data and user feedback to know what is really important to work on, instead of relying on opinion?

##Communication and general team coordination

* Do you have a centralized communication platform?
* Do you avoid meetings when possible?
* Do you keep trace of things said during meetings?
* Do you have clear channels of information that let people know about the various decisions made?
* Do you regularly discuss as a team the success and failures of your recent work?
* Do you encourage individuals to suggest new ideas and give feedback?


##Programming

* Do you use [vource control](#vource-control)?
* Does _all_ of your team actually know how to [properly use source control](#properly-using-version-control?
* Do you have a [branching strategy](#branching-strategy) for your team?
* Do you perform mandatory code reviews before merging any change in production at some point?
* Do you let enough time to your developers to properly perform code reviews?
* Do you have a bug database?
* Can you make a build in one step?
* Do you have some form of continuous integration running?
* Do you have automated tests running after each build?
* Do you fix all known bugs before working on new features?
* Do you take the time to update old code to current standards when you need to modify it?
* Do you have a coding convention?
* Do you check that the coding convention is respected?
* Do you have a documentation that summarises the project's architecture?
* Do you work with modular code, split in small, independant files?

#Detailed list

##Version Control

If you're here, you probably know what [source control](http://www.git-tower.com/learn/git/ebook/mac/basics/what-is-version-control#start) is. It is the absolute minimum standard for any project involving code. Even if there is only one programmer working alone, source control is required. This one is non-negotiable. Here's [why](http://www.git-tower.com/learn/git/ebook/mac/basics/why-use-version-control), and here's [how to get started](http://www.git-tower.com/learn/git/ebook)

##Properly using version control

Even though most companies use source control, very few of them use them properly. Thing is, for some reasons developers are rarely properly trained for it, and people assume that it should just work out of the box. Especially with the existing graphical interfaces for Git that hide the command-line part for you.

Long story short: If you only use git to commit/pull/push, you're missing a ton of things. Have you ever had to copy/paste lines to cancel a change someone made, or comment tons of line because you were developping a feature and need to temporarily disable it? If those sort of things remind you something, you're probably not using git to its full capacity. Do you [use branches](http://www.git-tower.com/learn/git/ebook/mac/branching-merging/branching-can-change-your-life#start)?

If you want to really understand git and be the person that saves the team with their understanding of git, you should definitely look at [this website](http://think-like-a-git.net/).

##Branching Strategy

Using branches is a good thing, but you should have a clear process for working with branches. People creating branches when they work on something is fine, but it's way better if you have a standardized way of managing those branches.

There are many ways to do that and in the end it depends on how you work and how your team is structured. But basically, you should be clear with your team about:

* Why branches are made
* How they're named
* When and where they are merged/deleted
* Which branches are sensible, permanent branch (like the branch you will use for beta builds, production builds...)


#Tools

## Slack

[Slack](http://slack.com/) is an awesome communication platform. It centralizes everything and can connect to pretty much any API. A ton of companies have started using it and have been able to stop working with crowded mail inboxes, useless meetings and other problems.


## Jira
## Github
