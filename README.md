# Startup-Test
This checklist of important things that tech organisations should be doing in the fields of communication, project management, and programming.

It is inspired by the [Joel Test](http://www.joelonsoftware.com/articles/fog0000000043.html). It's just a way bigger list that is intended to become a definitive, open and collaborative list of good practices, widely accepted by tech companies. This collection of questions are inspired mostly by Agile development and the actual, practical experience that comes with it. There are other ways of successfully developping software, but this way is used widely enough to be considered and industry standard.

This document being open source, it is intended to be refined as much as possible by people's ideas, and new practices that may be discovered, in order to serve as a reliable resource for any tech organisation.

You can see it as a test, checklist or general wishlist.

It is a **work in progress**, many things are yet to be written, but this first draft is accessible for feedback and improvement. Feel free to fork, add things and make a Pull Request if you want to help. You can also open issues here on Github for discussion, questions, or suggestions.

##Project Management

* Do you break down feature requests in [small chunks of isolated tasks](#breaking-down-tasks) that each require a small amount of time?
* Do you let members of the team participate in [estimating the tasks](#estimating-tasks) duration?
* Do you set your planning for short sessions (few days/weeks) and then refine it at the end of each session?

##Communication and general team coordination

* Do you have a centralized [communication platform](#communication-platform)?
* Do you [avoid meetings](#avoiding-meetings) when possible?
* Do you [keep trace](#storing-information) of things said during meetings?
* Do you have clear [channels of information](#information-channels) that let people know about the various decisions made?
* Do you regularly [discuss as a team](#discussing-success-and-failures) the success and failures of your recent work?
* Do you encourage individuals to suggest new ideas and [give feedback](#team-feedback)?


##Programming

* Do you use [version control](#vource-control)?
* Does _all_ of your team actually know how to [properly use source control](#properly-using-version-control?)
* Do you have a [branching strategy](#branching-strategy) for your team?
* Do you perform mandatory [code reviews](#code-reviews) before merging any change in production at some point?
* Do you let enough time to your developers to properly perform code reviews?
* Do you have a bug database?
* Can you make a build in one step?
* Do you have some form of continuous integration running?
* Do you have automated tests running after each build?
* Do you write new automated tests before writing new code or fixing a bug?
* Do you fix all known bugs before working on new features?
* Do you take the time to update old code to current standards when you need to modify it?
* Do you have a coding convention?
* Do you check that the coding convention is respected?
* Do you have a documentation that summarises the project's architecture?
* Do you work with modular code, split in small, independant files?

#Detailed list

(wip)


## Estimating Tasks

It is very important that when working with a team, the persons estimating the duration for a task are actually the ones that will work on it. Even if the manager knows the work of the people, they might not necessarily know all the details and other things the tasks depends on. So it's way safer to have the people actually working on the project deciding how much time they need. Multiple advices are always good.

So the idea is to take everyone concerned by a task on the team and let them discuss the task, and decide the time they need. A manager (or anyone not directly working on the task) should not have the power to reduce the estimated time.

It's also important to note that on the engineering side, people tend to underestimate the duration of a task, and it is a good idea to multiply the estimated time for some error margin. Better overestimate a task and be faster than expected, than delivering late.

## Breaking Down Tasks

The "standard" allowable times for tasks are: 1, 2, 4 and 8 hour. If you estimate a task, it must be one of these times. If you estimate, say, 3 hours, then pick 4, don't try to fit it in two hours.

These fixed time chunks are there to avoid people trying to fit things in lower, needlessly precise intervals of time, which is often a sign of underestimation. So don't just try to say this task will be 5 and a half hour. Just allow the day to it and do it properly.

If any task is more than 8 hours, then it's too big a task and should be broken down in smaller chunks. A big task during more than one day creates problems. It's not easy to track progress on long tasks, and our brains are not really made for that. We're made for working with small problems. The smaller the better.

Less is more. With restrictive but simple rules on the way you plan, you can make sure that the rules are actually followed properly.

##Communication Platform

> TODO (Centralized communication platform that avoid spreading on multiple tools. ie. Slack)

##Avoiding Meetings

> TODO (Avoiding useless meetings all the time, always stopping the productivity of people. Learning to have meetings only when necessary)

##Storing Information

> TODO (Keeping trace of important things/data. Taking note of things said during meetings, and having most discussions directly on the public communication platform so they don't need to be transcribed later, allowing new team members do read through the collective knowledge of the team)

##Information Channels

> TODO (Making information available to everyone who may be concerned, letting people know where they can find information. Allowing/encouraging people to communicate, ask questions if needed etc. Clarity above all)

##Discussing success and failures

> TODO (Regularly look back on the recent work and discuss as a team what worked and what didn't. Adapt your different processes according to that)

##Team Feedback

> TODO (Let the team frequently give general feedback on any matter, either related to product, or general office life. This should be done regularly, as a standard practice. It might be good to allow anonymized feedback for people that might have sensitive issues).

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

##Code Reviews

Contrary to popular belief, code review need not be hard. And they are [incredibly useful](https://www.atlassian.com/agile/code-reviews). Just by having someone give a look at a commit before puttin it in production, you can avoid horrible bugs later.

There again, there are multiple strategies. But the simplest, which is the model followed by open source development on websites like Github, is code review on Pull Request.

Basically the idea is, when someone wants to merge their changes from a development branch to the production/staging/whatever branch, they open a Pull Request. You then have at least one developer, ideally multiple, read through the code to see if everything is OK before validating the change.

The benefits are multiple: Social pressure makes people write better code, risky code that create bugs can be detected sooner, and people in the project understand more about the code that other persons wrote, which is better for maintenance.

#Tools

> TODO: This section is a list of tools related to this guide. Feel free to add some to the list.


## Communication

### Slack

[Slack](http://slack.com/) is an awesome communication platform. It centralizes everything and can connect to pretty much any API. A ton of companies have started using it and have been able to stop working with crowded mail inboxes, useless meetings and other problems.

## Project Management

### Jira

[Jira](https://www.atlassian.com/software/jira/)

### Trello

[Trello] (https://trello.com/)

## Source Control

### Github

[Github](http://github.com)

### Bitbucket

[Bitbucket](http://bitbucket.com)

### GitLab

[GitLab] (https://about.gitlab.com/)

## Others



#Resources

> TODO: This is a list of links to resources related to this guide (not tools, see previous chapter). Feel free to link any relevant article, tutorial, presentation, documentation...
