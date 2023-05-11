# Pull Requests
GitHub pull requests allow you to propose and collaborate on changes to a repository. Everyone in the community can [create a pull request](#create-a-pull-request), or add reviews, comments, and suggestions to existing pull requests. The contribution process for pull requests is described in detail in the [Contribution Guidelines]. In the following, a practical guide for getting started with pull requests is provided. 

### Create a Pull Request
To begin, create a pull request to propose changes. If you want to create a new file, or make changes to an existing file, you must create a pull request by either:

1. [Navigating](https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/github_guides/navigation.md) to a relevant location for your new file, clicking on "Add file" and then "Create new file" in the drop-down menu. 
    - Give the file a title (remember to add ".md" if you want to create a Markdown file), and fill in the file with the content you want to propose. 
    - Scroll down to the "Commit changes" section. You can add a summary of the proposed changes, give the pull request a title, and optionally change the branch name.
2. Navigating to the location of a file you want to modify, clicking on the file, and then clicking on the "✏️" in the upper right corner of the file, to add your proposed changes. 
    - Scroll down to the "Commit changes" section. You can add a summary of the proposed changes, give the pull request a title, and optionally change the branch name.
4. Navigating to the [Pull Request Templates] to find a relevant template for your pull request (if you want to create 1. a Request for Comments (RFC), or 2. a [Meeting Minutes]), and then:
   - Click on the pull request template you want to use
   - Click on the "Copy raw contents" symbol (The two overlapping squares)
   - Navigate to a relevant location for your file, click on "Add file" and then "Create new file" in the drop-down menu. 
   - Left-click in the new file and choose "Paste" in the drop-down menu, or press ctrl+V to paste the template. 
   - Fill in the template with your content 
   - Scroll down to the "Commit changes" section. You can add a summary of the proposed changes, give the pull request a title, and optionally change the branch name.

An example of filling in the "Commit changes" section is shown below:

<img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/pull_request_commit_changes.png" width="100%"/>
 
**Note** that in this repository, changes must always be proposed in a separate branch, to ensure that the default branch only contains finished and approved work. 

### Merging a Pull Request
After initializing a pull request, you'll see a review page that shows a high-level overview of the changes between _your branch_ (the compare branch) and the repository's _main_ branch (the base branch). 

While your pull request is _open_ (and visible in the [Pull Request]s tab, you can add follow-up commits to the pull request, add labels, projects, reviewers and assignees, and @mention individual contributors or teams. You can also link a pull request to an [issue](https://github.com/energinet-open-incubator/origin-collaboration/issues) to show that a fix is in progress for the topic discussed in the issue. Additionally, when your pull request is created, other contributors can review your proposed changes, add comments, add additional commits, and contribute to the pull request discussion. 

There are two types of pull requests: _ready for review_ and _draft_. Draft pull requests cannot be merged, but you can convert a pull request to a draft at any time, to signal to the community that you still want to do more work before expecting any in-depth reviews. 

Once you're happy with the changes, and you received one or several approving reviews you can merge the pull request. Remember to delete your branch when the content of your pull request has been merged. 

  
### Reviewing Others' Pull Requests
If you want to review someone else's pull request, you can review changes and leave individual comments or make change suggestions in the file(s) contained in the pull request, by:

- Navigating to the pull request you want to review, from the list of open [Pull Request]s
- In the pull request, click on the tab "Files changed"

  <img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/pull_request_files_changed.png" width="70%"/>
 
- Hover over the line of code where you'd like to add a comment, or suggest a change and click the blue comment icon that appears. 
  
  <img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/pull_request_add_comment.png" width="70%"/>
 
- To add a comment or suggestion for multiple lines, click and drag to select several lines simultaneously, and then click the blue comment icon.
  - If you want to make a change suggestion to the selected lines, click the square with a "+-" sign inside, in the top right corner of the comment box that appears. 
  
    <img src="https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/figures/pull_request_add_suggestion.png" width="70%"/>
    
  - When you added your comment or suggestion, choose "Add Single Comment", if you only have the one thing to add, or choose "Start a Review" if you want to add several comments and/or suggestions for a more in-depth review.


<!-- Anchorlink style -->
[Contribution Guidelines]: https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/guidelines/contribution_guidelines.md#pull-requests
[Pull Request]: https://github.com/energinet-open-incubator/origin-collaboration/pulls 
[Discussions]: https://github.com/energinet-open-incubator/origin-collaboration/discussions
[Issues]: https://github.com/energinet-open-incubator/origin-collaboration/issues
[Issue Templates]: https://github.com/energinet-open-incubator/origin-collaboration/issues/new/choose
[Projects]: https://github.com/energinet-open-incubator/origin-collaboration/projects?query=is%3Aopen
[Trusted Committer]: https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/introductory/innersource-short-role-descriptions.md#the-trusted-committer
[Pull Request Templates]: https://github.com/energinet-open-incubator/origin-collaboration/tree/main/pull_request_templates
[RFC]: https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/additional_reading/rfc.md
[Meeting Minutes]: https://github.com/energinet-open-incubator/origin-collaboration/tree/main/meeting_minutes
[Trusted Committer of this repository]: https://github.com/energinet-open-incubator/origin-collaboration
[Projects Guide]: https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/github_guides/projects.md
[Decision-Making Policy]: https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/guidelines/decision_making_policy.md
[Project-Origin Backlog]: https://github.com/orgs/energinet-open-incubator/projects/6
[Collaboration Platform Backlog]: https://github.com/orgs/energinet-open-incubator/projects/2/views/1
[First Workshop in Aarhus 8.11.2022]: https://github.com/orgs/energinet-open-incubator/projects/5/views/1 
[Weekly Synchronous Sesssions]: https://github.com/energinet-open-incubator/origin-collaboration#weekly-synchronous-sessions
