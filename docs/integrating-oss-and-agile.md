# How does Agile relate Open Source and what could be done to make them work together

Agile (software development) processes and Open Source (Software development) have in common that they are both strongly focused on being iterative and evolving - as opposed to linear planning from start to finish.

Often, Open Source focuses "FOSS projects" which are in reality _products_ often with small(er) or larger communities attached to them. This means that they inherently are _set out to exist for perpetuity_ and evolution instead of the static start, finish and goal to be achieved that traditional project life cycles have.  (Of course they can die, but the initial intent is to be highlighted here.)

While **Agile** often appears to be **more plannable** and "clean", **Open Source** historically breathes ultrapragmatism and does not claim planning or having "clean" processes for itself but is **more event driven**.

Both have proven to work over decades, with Open Source and its ways of working representing the bedrock of any digital effort these days.

Open Source historically evolved in an environment with spatially distributed developers, often over multiple time zones. The evolution happened during a time where Zoom and Team calls were not readily available but mostly emails or text chats and some simple web applications dominated communication. See also the [guide on asynchronous environments](https://github.com/project-origin/origin-collaboration/blob/main/guides/acting_in_asynchronous_environments.md).

High churn of participants was (and is today) dominant as everyone stays only as long as there is something in it for them – often just a bug they need fixed and thus create a fix for themselves, or maybe for a feature. Very few will stay for the community or even become a trusted committer. Sometimes people come, go and reappear years later, sometimes even the trusted committers in low activity efforts.

Thus, **Open Source is strongly based on text-based** interaction as well as on **asynchronous interactions**.

Most **Agile** environments **highlight colocation** and usually lots of **verbal interaction**.

## Integrating the planned, possibly sprint structured environment of Agile with the event driven environment of Open Source

Here are a few practical suggestions, not necessarily complete but a good starter.

### Handling interrupts / the event driven nature of Open Source

Open Source is event driven, or looks like it is. After all you can not predict what people outside of your scope of influence do, but nevertheless rely on them.
Hence, it is best to prepare yourself to be able to handle these interrupts/events. 
One good approach here is to leave unplanned room to handle interactions. You could _allocate 10-20% of the peoples' time to interruptions_.
There are quite a few more unknown sources of interruptions, even without counting in Open Source or InnerSource participation, anyway. Glancing at the reality of average agile they're just as common there as much as agile might create the illusion of a "plan" or "control".

Nobody likes to wait. Especially if they want to give you a gift, i.e. a contribution.
Make sure that you react to events from the Open Source (and InnerSource) domain timely, usually 2, max. 3 days max are good.
Acknowledge their request in a meaningful way, handle it out of the interruption budget if it can be done fast. If not let them know and keep transparent communication in the Open Source project. You can then plan it into your sprints or other agile structures, as you would plan any other task.
  - Nota bene: Your internal work structures and cadences are usually often not visible to outsiders. Thus, to them it might look like their request is postponed to eternity. If you run an open source project anyway, consider handling the work structures openly too. 

Work for InnerSource efforts and Open Source events can be planned and tackled like any other task. It's work that needs to be done, and can be assigned a value contribution and a priority. 
  - Example: You need to work around a change in some dependency. Or want a new feature that could live either in your scope or someone else's scope. 
    - The way of executing this could be "we code 500 lines of code and discuss the domain specifics with business and domain experts for feature X" or "we mentor and assist person Y from another scope with building a solution in our scope that will help them and us to achieve feature X" (assuming the feature is useful for others beyond yourself too)  or "a solution for this will be beneficial for everyone if we build it in another scope. thus we ask a person Y from the other scope if they agree, what variations to feature X they'd like to see to accept it in their scope and then start building it there while being mentored by person Y such that the result is acceptable to them".
    - All variations result in the same value of feature X. Just that there is less waste, potential for value leverage and creation of ultra-valuable domain level connections to likely strenghten resilience and problem solving skills across the entire company. (And: They exist in most companies anyway, but their existence is often denied turning them into an unknown or risk in the worst case. Thus: Accept them and reap the value they contain.)  

Caveat: Open Source events are external dependencies.
The person working with you there is not bound to your schedule or sprints. They might have their own, be a hobbyist, etc. Do not expect your usual cadences and turnaround times.
If a person becomes a repeated contributor, likely some trust will build up. You may even learn where they work or if they're a hobbyist and maybe even some rapport will build up that may allow some aspects of planability across organizations.
If you achieve this: Celebrate each other and value that cooperation.  		

### Common expectations of the environment

Open Source, and by lineage InnerSource too, environments have certain inbuilt expectations of people. If you know and respect them your likelyhood of success is higher. 
Or as they say: When in Rome, do as the Romans do. 

Don't feel entitled to contributions or planability even if there have been repeated contributions from the same person. All contributions are gifts. Some gifts just keep on giving.

As an agile product manager, you likely cannot keep track of what happens in Open Source projects you use or contribute to. Maybe even tracking all the activity in your own one might become difficult.
If it's your own Open Source project, you should know what happens, even on the Open Source front. What can you do nevertheless?
 - Encourage your developers to foster relations with the Open Source projects you depend on so they, and thus by proxy: you,  have a chance to know what's happening in them. This way they may be able advocate for some of your needs and see opportunities to contribute or shape things where it might be beneficial for you. 
   - They will need time for it; provide that time. It usually has a good ROI on short and longer term.
 - For your own Open Source projects: You will have trusted committers, which are likely lead developers or people that might one day evolve into an engineering manager. 
   - It is the trusted committers job to mentor their community members, advocate for the communities needs, and evolve the product and its roadmap too. Listen to them and see them as your equal.
   - Again: This will cost a relevant amount of time. Provide them with that. It is crucial for success and ROI of your Open Source project.

Remember: An Open Source project always needs to be useful to others too – if it only has value for you, nobody else but you will have a reason to care about it.
