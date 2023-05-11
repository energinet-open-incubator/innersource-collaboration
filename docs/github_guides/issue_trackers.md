# Issue trackers in Github
This guide provides an overview on the Issues tool on Github, describing their purpose and layout on Github. Additionally, some information about how to use them here in Project-Origin is provided.  

## Overview
An issue in Github can be created to track progress on a specific task or topic. 
In this context, the term _“issue”_ should not be interpreted as “problem”, but rather as a _“subject that needs attention and action”_. 
All repositories have a tab, containing all issues created in the given repository:

![Issues tab](https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/issues.png)

In this tab, all issues created will be available in a list:

![issues list](https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/issues-list.png)

The issue list allows for precise filtering and mass-processing, e.g. if you want to mass update labels or clean up during a housekeeping session.

## Useful attributes
Issues can consist of several different attributes, including at least a title, issue number, creation date, and author.

<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/issue-example.png" width="90%"/>

Attributes that are useful when working with issues are 'assignees', who are the ones responsible for ensuring progress on the issue, and 'labels', which can help indicate the type of issue.

<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/attributes.png" width="30%"/>

If you wish to change, add or delete a label, click on the gear icon next to it (In the [_quick issue view_](#handling-issues-directly-in-the-projects-view) click on the label). 

As work on the issue progresses, Actions related to the issue will be visible in the issue item:

<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/issues-biggerindividualview.png" width="75%"/>

If there are pull requests in the Github Organization related to the issue, these can be linked to the issue, to track progress on these as well:

<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/link-to-pr.png" width="30%"/>

To make sure to follow progress on issues relevant to you, you can subscribe to an issue, to get notifications whenever an update happens. 

<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/subscribe.png" width="30%"/>!

If you are mentioned in an issue or have created it, you will be automatically notified.

## Mentioning, notifying people and tasks, and cross-referencing
You can cross-reference all content everywhere by just putting # and the issue number or pull request number in your text. 
If you do, the referenced element will get a link to the referencing element. 
As an example: If you write _"#90"_ you reference the pull request that initially created this document. 

<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/tagging-pr.png" width="70%"/>
 
The same works for people. 
You can reference them using @ and their username. For example _@lenucksi_ or _@lauranolling_.

<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/tagging-person.png" width="70%"/>

## Issues in Projects views
As an alternative to the full list of issues in the Issues tab, issues can be put into customized Project views, a list of which is found under the Projects tab:

![issues in projects](https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/projects.png)

In Projects, the advantage is that you can make your own custom views, and sort the issues by issues by topic, priority, status, and others. 
Projects can be viewed either as a KANBAN (see also: Trello) style board or as a list. 

Note that you can add _items_ in the Projects views. 
These will be created as _draft issues_. 
However, these are local to the project board and have very little features. 
There's a button in the _draft issue_ to convert them to a "real" issue.

The Projects views also offer you a _quick issue view_ if you click on an issue's title:

![issue view](https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/projects-list-inline-issueview.png)

To learn more about the Github Projects feature, you can take a look at the [Projects Guide](https://github.com/energinet-open-incubator/origin-collaboration/tree/main/guides/projects.md).

## Task Lists using Issues
Creating task lists to keep track of progress on a specific block of work can be very useful. You can use issues to divide a larger task into smaller to-do's and track progress on these to-do's using Github's Task List feature:

<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/issues_task_list.png" width="70%"/>

When adding tasks you can either tag existing issues, or — when you have written down your to-do's — convert these to issues:

<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/issues_task_issue_tag_issue.png" width="70%"/>
<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/issues_task_issue_create.png" width="70%"/>

When you navigate to one of the issues linked in the task list, Github will show the issue number of the task list:

<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/issues_task_tracked_by.png" width="50%"/>

Github will automatically keep track of the tasks, so when issues are closed, they will automatically be marked as "complete" in the task list. Alternatively, you can mark tasks as complete, by clicking the checkbox. The number of task completed is shown in the issue containing the task list:

<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/issues_task_tracking.png" width="70%"/>

You can create a task list, by using the [issue template](https://github.com/energinet-open-incubator/origin-collaboration/issues/new/choose) made for this purpose. 

For more information about Github Task Lists, you can take a look at [Github's official Documentation on task lists](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/about-task-lists).

## Issue Templates

To use issues in Project Origin, we have set up some issue templates, to make sure that all the relevant information will be included, and that it is easier to find the issues to people for whom it is relevant. Take a look at the [Issue templates here](https://github.com/energinet-open-incubator/origin-collaboration/issues/new/choose).
