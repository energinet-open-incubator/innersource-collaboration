This document describes the various roles involved with running weekly meetings in Project-Origin.
All of these roles should be filled and completed for each meeting to be as successful as possible.
The roles are:

* [Scheduler]
* [Facilitator]
* [Scribe]

## Scheduler

The _Scheduler_ sends the calendar invite for the meeting. 
**Preferably prepare the agenda and send it out before 48 hours prior to the meeting**. 
A complete to-do list for preparing and sending out the agenda is provided in the following: 


1. To most easily set up the agenda, find the [meeting template] and select _"Copy raw contents"_ from the upper right hand menu (the two overlapping squares).
2. Go to the [working session meeting notes folder] and select _"Add file"_ ➡️ _"Create new file"_, and paste the content of the clipboard to this file.
3. Name the file `project-origin-working-session-dd-mm-yyyy.md` (and of course replace `dd`, `mm` and `yyyy` with the date of the upcoming meeting).
4. Prepare the new agenda (The [meeting template] that you pasted already contains some fixed agenda points): 
    - Update the _"Roles"_ section with the role assignments agreed at the previous working session (which you can find in the [working session meeting notes folder])
    - Edit the numbers for each board's status columns to reflect their current state. 
    - Add any additional points to go through at the next meeting, if requested by any participants.
    - Below the _"assignments"_ item, first add the assignments from the previous agenda that haven't been striked out. Then add any new assignments agreed from the previous meeting's [Scribe] notes (You can find both in the [working session meeting notes folder]).
5. When the new document is done, scroll down to the small commit-form at the end. 
    - Leave the default title as-is (which is probably _"Create project-origin-working-session-dd-mm-yyyy.md"_). 
    - In the text box where you can add an extended description, you can write down relevant information about the meeting. A suggestion for such description is (just copy/paste the below if it is useful):
       > This adds the notes template with new agenda, carry-over etc. for the DD-MM-YYYY weekly sync session.
       >
       > Please review, add your material, your comments on your assignments etc. before the meeting.
       > * Added names agreed for each of the three roles
       > * Updated status overview of boards
       > * Added assignments from last weeks session
       > * Made document ready for scribe notes
6. Create the document as a [pull request], by using the _Create a new branch for this commit and start a pull request_ setting. Call the branch `working-session-notes-dd-mm-yyyy`. 
    - Then, related discussions can happen here, agenda points can potentially be added, and the scribe can add their notes directly to the pull request.
7. To upload the document, press the _"Commit new file"_ button. Copy the URL link for the file you just created (to add to the calendar invite).
8. Update the calendar invite for the next meeting:
    - Open the next calendar instance in Outlook
    - Add a small message to everyone, such as (just copy/paste this, if it is useful):
      > Project Origin Weekly DD, MM, YYYY
      > 
      > Hello everyone, 
      > 
      > Here is the agenda for our first weekly sync session. 😊 NOTE: To be updated/cleaned up further up until 24 hours before the meeting. If you have anything to add, feel free to add it to the pull request: _link-to-pull-request-here_.
      >
      > Roles
      > [...]
      > 
      > Agenda
      > [...]
      > 
    - Add the correct meeting date to the first line and paste the link to your [pull request] at _link-to-pull-request-here_. (The scribe will need this link to add notes to it during the working session.)
    - Copy/paste the _"Roles"_ and the _"Agenda"_ content you just created into the calendar invite. This is easiest to do by going to the _"Files changed"_ tab in your [pull request] and then choosing _"Display the rich diff"_ setting (which is a rectangle icon in the upper right corner)


## Facilitator

The _Facilitator_ conducts the meeting so that all of the agenda items are finished within the allotted time. Below is a suggested list of to-do's to ensure that the meeting runs smoothly: 

### Before the meeting
* Review the agenda and ensure that you are reasonably familiar with each item on it. 
* If convenient to you, it can be useful to:
  * Open the [pull request] created by the [Scheduler] and select the _"Files changed"_ tab. Choose the _"Display the rich diff"_ setting (which is a rectangle icon in the upper right corner) and scroll to the agenda. 
  * Open the three [Project board]s in each their tab, by right-clicking the links provided in the agenda and choosing _"Open in new tab*_. 
 
### During the meeting
* Have the agenda open and share your screen with the people on the call.
  * Present the agenda and then guide the group through reviewing each agenda item from top to bottom.
  * Before discussing each item, briefly remind people of what it is so that they're up to speed and can contribute to the conversation.
  * Keep in mind that the main purpose of reviewing each agenda item is to generate actionable, assigned next steps to create continuous project progress.
    * If you are stuck, guide the conversation towards understanding what is blocking progression and what can be done to advance it.
    * Strive for each task to be assigned to a volunteer on the call.
* When reviewing a [Project board]:
  * Treat each issue in the **In Progress** and **Waiting/Blocked** columns as its own item on the agenda.
  * Ask if anyone would like to review any issue in the **To Do** column. If not, this column can be skipped.
  * The **Done** column does not need review. When you want to empty the column click the three dots in the upper right corner of the column and choose _"Archive all"_.
* Remember that it's OK to finish early. Once the agenda is complete the meeting is over.
* At the close of the call thank everyone for participating.


## Scribe

The _Scribe_ ensures that meeting notes are taken and sends them out.

Use the meeting template created by the Scheduler for this, which can be found as a [pull request](https://github.com/project-origin/origin-collaboration/pulls) marked with the meeting date. Open the linked file (there is a "files changed" tab in the pull request) and click the three dots in the upper right corner and click "Edit".

**During Meeting**

* [ ] Note the first names of each meeting attendee in the **Attendees** section.
* [ ] Record a short summary of each discussion in the **Key Points** section.
* [ ] Record all assignments in the **Assignments** section.

**After Meeting**

* [ ] Upload your notes to Github by committing them to the pull request. It could be useful to add a comment along the lines of "Minutes for working session DD-MM-YYYY added".
* [ ] Email the notes to everyone on the meeting invite. 
  This email should include (in order):
  * Link to the agenda document where the notes are located.
  * Any access disclaimer where needed.
  * Copy/pasted notes from the agenda document. (If it's a formatted email you can just take the pretty rendered content from GitHub.)

  * [ ] Allow some time for a bit of post-processing of the meeting notes. If anyone has something to add, they can commit it to the pull request, and related discussions can happen in the pull request. Within a reasonable time, finish processing/adding to the notes and merge the pull request, to upload it to the [meeting minutes folder](https://github.com/project-origin/origin-collaboration/tree/main/meeting-minutes).


### Tips

* Ensure that a regular attendee who is not at the meeting could understand what happened by the notes only.
* Make sure the notes are clear and to the point.
Part of your service as _Scribe_ is to summarize the key points of what was said so that recipients don't need to wade through all of the conversation in order to understand its essentials.
<!-- * Here is a [sample notes announcement].
* Here is a [sample email]. -->
* An easy way to send the notes to everyone on the meeting invite is to "Reply all" to the invite.

[meeting template]: https://github.com/project-origin/origin-collaboration/blob/main/pull_request_templates/meeting-minutes-template.md
[working session meeting notes folder]: https://github.com/project-origin/origin-collaboration/tree/main/meeting_minutes
[Scheduler]: #scheduler
[Facilitator]: #facilitator
[Scribe]: #scribe
[pull request]: https://github.com/project-origin/origin-collaboration/pulls
[Project board]: https://github.com/project-origin/origin-collaboration/projects?query=is%3Aopen
