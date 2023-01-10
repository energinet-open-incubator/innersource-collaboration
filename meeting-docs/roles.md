This document describes the various roles involved with running the meetings involved in the creation of Project-Origin.
All of these roles should be filled and completed for each meeting to be as successful as possible.
The roles are:

* [Scheduler](#scheduler)
* [Facilitator](#facilitator)
* [Scribe](#scribe)

<a name="scheduler"></a>
## Scheduler

The _Scheduler_ sends the calendar invite for the meeting. 
The following guidelines apply to the scheduler:

**Within 24 Hours of Previous Meeting**
* [ ] Prepare the new invite based on the old one. Add any new attendees email-address and add a short summary of the agenda. You can take the short agenda part the [Scribe] prepared.  
* [ ] Visit the [working session meeting notes folder].
* [ ] Open the  meeting template and select "raw" from the right hand menu. Copy the entire content to the clipboard.
* [ ] Go to the [working session meeting notes folder] and select "Add file" -> "Create new file", and paste the content of the clipboard to this file.
* [ ] Name the file `project-origin-working-session-MM-DD-YYYY.md` (and of course replace `MM`, `DD` and `YYYY` with the date of the upcoming meeting.
* [ ] **Complete the steps in the following, to set up this document**
<a name="preparedoc"></a>
* [ ] Prepare and add the new agenda to the document:
  * [ ] Create the new agenda. [The meeting template](workinggroup-minutes-template.md) already contains some fixed agenda points to go through at every meeting. If relevant, add any additional points to go through at the next meeting. 
  * [ ] When the new agenda is created, fill out the small form at the end (the commit-message) with, e.g., "Create new agenda for MM-DD-YYYY" in the textbox where it by default says "Create new file". 
  * [ ] When you want to directly add the file to the repository without the review process of a pull request, keep the "Commit directly to main branch" setting. 
  * [ ] To upload the document, press the big green "Commit new file" button. You'll arrive at the new file you just created in the folder. Now, copy the URL for the file you created (to add to the calendar invite).

* [ ] Update the calendar invite for the next meeting:

  * Paste the link to the agenda document in the invite. (The scribe will need this link to add notes to it during the working session.)
  * Copy/paste the role assignments and agenda to the e-mail (the two first sections in the document you created).

### Tips

* You can reuse the old invite.

<a name="facilitator"></a>

## Facilitator

The _Facilitator_ conducts the meeting so that all of the agenda items are finished within the allotted time.

**Day Before Meeting**

* [ ] Review the agenda and ensure that you are reasonably familiar with each item on it.

**During Meeting**

* [ ] Facilitate the meeting according to the **Tips** below.


* Have the agenda open and share your screen with the people on the call.
* Guide the group through reviewing each agenda item from top to bottom.
* Before discussing each item, briefly remind people of what it is so that they're up to speed and can contribute to the conversation).
* The purpose of reviewing each agenda item is to generate actionable, assigned next steps.
### Tips
  * Guide the conversation towards understanding what is blocking the item's progression and what can be done to advance it.
  * Strive for each task to be assigned to a volunteer on the call.
  * When all such tasks have been assigned, move on to the next agenda item.
  
* When reviewing the project board:

  * Treat each issue in the **In Review** and **In Progress** columns as if it were its own item on the agenda.
  * The **Done** column does not need review.
  * Call out if anyone would like to review any issue in the **To Do** column.
  If so, then treat that issue like a regular agenda item.

* Remember that it's OK to finish early.
Once the agenda is complete the meeting is over.
* At the close of the call thank everyone for participating.

<a name="scribe"></a>

## Scribe

The _Scribe_ ensures that meeting notes are taken and sends them out.

Use the meeting template created by the Scheduler for this. Open the linked file and click the pencil button in the menu to the right.

**During Meeting**

* [ ] Note the first names of each meeting attendee.
* [ ] Record a short summary of each discussion in the **Key Points** section.
* [ ] Record all assignments in the **Assignments** section.

**After Meeting**

* [ ] Email the notes to everyone on the meeting invite. 
  This email should include (in order):
  * Link to the agenda document where the notes are located.
  * Any access disclaimer where needed.
  * Copy/pasted notes from the agenda document. (If it's a formatted email you can just take the pretty rendered content from GitHub.)

See this [sample email].
* [ ] Upload this document into the [working session folder].
  * [ ] See [PrepareDoc] for how to check in the changes. It could be useful to add a comment along the lines of "Minutes for working session MM-DD-YYYY added".  


### Tips

* Ensure that a regular attendee who is not at the meeting could understand what happened by the notes only.
* Make sure the notes are clear and to the point.
Part of your service as _Scribe_ is to summarize the key points of what was said so that recipients don't need to wade through all of the conversation in order to understand its essentials.
<!-- * Here is a [sample notes announcement].
* Here is a [sample email]. -->
* An easy way to send the notes to everyone on the meeting invite is to "Reply all" to the invite.

[template]: https://github.com/project-origin/origin-collaboration/pull/87
[learning path folder]: https://github.com/project-origin/origin-collaboration/tree/main/meeting-docs
[Scheduler]: #scheduler
[Facilitator]: #facilitator
[Scribe]: #scribe
[PrepareDoc]: #preparedoc
[sample email]: ./examples/notes-email.md