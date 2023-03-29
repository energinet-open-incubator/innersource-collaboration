# Integration Open Source and Agile Work Processes

## Table of Contents
1. [Introduction](#introduction)
2. [Integrating the Planned with the Event-Driven](#integrating-the-planned-with-the-event-driven)
    - [Handling Interrupts](handling-interrupts)
    - [Common Expectations in Open Source](common-expectations-in-open-source)


## Introduction

How does Agile relate Open Source and what could be done to make them work together? This document will treat this question by providing some context, incongruities and finally some practical approaches to take.  

Agile (software development) processes and Open Source (Software development) have in common that they are both strongly focused on being iterative and evolving - as opposed to linear planning from start to finish.

Often, Open Source focuses on "FOSS projects" which involve _products_ often with small(er) or larger communities attached to them. This means that they inherently are _set out to exist for perpetuity_ and evolution instead of the static start-date, end-date and goal in traditional project life-cycles. (Of course FOSS projects can die as well, but the intent is to be highlighted here.)

While **Agile** often appears to be **more plannable** and "clean", **Open Source** historically breathes ultrapragmatism and does not claim planning or having "clean" processes for itself but is **more event driven**.

Both have proven to work over decades, with Open Source and its ways of working representing the bedrock of any digital effort these days.

Open Source historically evolved in an environment with spatially distributed developers, often over multiple time zones. The evolution happened during a time where Zoom and Microsoft Teams were not readily available. Instead, mostly emails, text chats and some simple web applications dominated communication. See also the [Guide on Asynchronous Environments].

High churn of participants was (and is today) dominant as everyone stays only as long as there is something in it for them – often just a bug they need fixed and thus create a fix for themselves, or maybe for a feature. Very few will stay for the community or even become a [Trusted Committer]. Sometimes people come, go and reappear years later, sometimes even the trusted committers in low activity efforts.

Thus, **Open Source is strongly based on text-based, asynchronous interactions**.

Most **Agile** environments **highlight colocation** and usually lots of **verbal interaction**.

## Integrating the Planned with the Event-Driven 

Here are a few practical suggestions, not necessarily complete but a good starter on how to integrate the planned (sprint structured) environment of Agile with the event driven environment of Open Source.

### Handling Interrupts 
You can not predict what people outside of your scope of influence do, but in an Open Source environment you nevertheless rely on them.
Hence, if applying agile structures within your influence, prepare yourself to be able to handle these interrupts/events:

- Leave unplanned room to handle interactions. You could allocate, e.g., 10-20 % of the peoples' time to handle interruptions.
- Acknowledge incoming requests from [Contributor]s in a meaningful way, handle it out of the interruption budget if it can be done fast. 
- Your internal work structures and cadences are usually often not visible to outsiders. Thus, to them it might look like their request is postponed (to eternity). Consider handling the work structures openly too, or at least communicating them, so that outside contributors know. 
- External contributors working with you is not bound to your schedule or sprints. They might have their own, be a hobbyist, etc. Do not expect your usual cadences and turnaround times.
    -If a person becomes a repeated contributor, likely some trust will build up. You may even learn where they work or if they're a hobbyist and maybe even some rapport will build up that may allow some aspects of planability across organizations.
    
- Make sure that you react to events from the Open Source (and InnerSource) domain timely, usually 2-3 days max are good.
    - Nobody likes to wait. Especially if they want to give you a gift, i.e. a contribution.
    - If reacting to a request cannot be done fast, let the person making the request know, hence keeping transparent communication in the Open Source project. You can then plan it into your sprints or other agile structures, as you would plan any other task. Examples on such tasks are:
        - "_We mentor and assist person Y from another scope with building a solution in our scope that will help them and us to achieve feature X_" or
        - "_A solution for this will be beneficial for everyone. Thus, we ask person Y from another scope if they agree, what variations to feature X they'd like to see to accept it in their scope and then start building it there while being mentored by a trusted committer such that the result is acceptable to them_".
        - All variations result in the same value of feature X. Just that there is less waste, potential for value leverage and creation of ultra-valuable domain level connections to likely strenghten resilience and problem solving skills across the entire company. (And: They exist in most companies anyway, but their existence is often denied turning them into an unknown or risk in the worst case. Thus: Accept them and reap the value they contain.)  


### Common Expectations in Open Source

Open Source, and by lineage InnerSource too, environments have certain inbuilt expectations from people. If you know and respect those expectations your likelihood of success is higher:

- Don't feel entitled to contributions or planability even if there have been repeated contributions from the same person. All contributions are gifts. Some gifts just keep on giving.
- As an agile product manager, you likely cannot keep track of what happens in Open Source projects you use or contribute to.
- If it's your own Open Source project, you should know what happens, even on the Open Source front. 
    - Encourage your developers to foster relations with the Open Source projects you depend on so they, and thus you, have a chance to know what's happening in them. 
        - This way they may be able advocate for some of your needs and see opportunities to contribute or shape things where it might be beneficial for you. 
        - They will need time for it; provide that time. It usually has a good Return on Investment (ROI) on short and longer term.
    - You can choose to have [Trusted Committer]s, which are likely lead developers or people that might one day evolve into an engineering manager. 
        - It is the Trusted Committers' job to mentor their community members, advocate for the communities needs, and evolve the product and its roadmap too. Listen to them and see them as your equal.
        - Again: This will cost a relevant amount of time. Provide them with that. It is crucial for success and ROI of your Open Source project.


<!-- Anchorlink style -->
[Guide on Asynchronous Environments]: https://github.com/project-origin/origin-collaboration/blob/main/docs/introductory/acting_in_asynchronous_environments.md
[Trusted Committer]: https://github.com/project-origin/origin-collaboration/blob/main/docs/introductory/innersource-short-role-descriptions.md#the-trusted-committer
[Contributor]: https://github.com/project-origin/origin-collaboration/blob/main/docs/introductory/innersource-short-role-descriptions.md#the-contributor
