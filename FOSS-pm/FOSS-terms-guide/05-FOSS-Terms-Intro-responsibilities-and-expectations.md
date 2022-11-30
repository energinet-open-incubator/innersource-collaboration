## Responsibilities and Expectations 

As shown above, Open Source is a large domain, however with well defined subdomains that are interlinked at certain points.

There are aspects that are technical, aspects that have a legal focus and aspects that are business strategy.

Energinet needs to start somewhere to make it practical and enable ongoing evolution. 

Currently running aspects are:

- The Energinet incubator: Here, we focus on learning how to work together internally, InnerSource style. There is some collaboration with partners as Mjølner,  Concordium etc.. Energinet should check if it is possible to treat this partnership as InnerSource or if there are any liability/contractual limits. It looks to the author as if this has already been addressed.
- Efforts around Energy Track & Trace / Project Origin with the Registry and the standard. Here, publication is the goal. Legal and Business strategy aspects can be focused here.

The following highlights aspects from the previous aspects for focused discussion. Should any other aspects arise from this in discussion, those should be followed too. 

### Limiting the blast damage: Boundaries

One goal of FOSS publication is to enable and facilitate collaboration with other organizations and people to create a greater common good that benefits everyone. However, the risk of the participating parties needs to be known, isolated and controlled. 

We should not be liable for the actions of others. Thus boundaries need to be set and risks defined. 
A possible course of action is to prioritize handling of the legal aspects of FOSS as described above by the risk the posed due to the enforcement and likelyhood of becoming a problem (legal realism).

#### Publication
##### Liability and Warranty
- Address the warranty and liability sections above and as illustrated in the [legal analysis document]()
##### FOSS compliance
###### Base cases and publication 
All cases assume us publishing code as Open Source package (as e.g. the registry here)

From common experience the relevance/source of problems from these cases are along the following lines:

- Competitors use claims of intellectual property law violation to
  - have cease&desist orders / "Einstweilige Verfügungen" declared by courts against us on the express lane removing the product from the market until a court decision arises long time after.
  - get access to proprietary code. This is used to:  
    - build upon this or 
    - use it as advantage i.e. "industry spionage"
    - use this as grounds for more claims, e.g. patent claims
- People claiming ownership of the intellectual property use this for financial advantage by using "Abmahnungen".   
  - See also: Patent claims as above
  - Companies selling commercial version of the FOSS library use this to sell the commercial version of the FOSS library used.
- Politically motivated actors/activists might use this to damage the publisher or incite general shit storms using combinations of any of the above.
  - Cases have been heard where this was used to force the publisher into creating effective FOSS compliance functions.

These effects are based on German an US reported cases. How does the Danish law and legal practice deal with the above violations and tactical approaches to inflict damage or gain a financial advantage? What opportunities of damage control, healing and limitation exist? Are there any risk evaluations possible?

####### License compatibility

Base question is: What happens upon combination of two licenses that have mutually exclusive conditions in one work. 

Example:

- We publish a FOSS package. It depends on two other FOSS packages. 
- One was assigned the Apache 2 license, the other was assigned the GPL2-only.
- Both have language making them mutually exclusive, see here: [license compatibilty]() 

It could be argued that:

- It is impossible to acquire a license for both of the FOSS packages.
- Both FOSS packages are referenced by the FOSS package published by us and are required for it be useful.
- It is impossible to legally use our FOSS package or publish it with licensed dependencies, thus publication (or even use) would run afoul of intellectual property law making this the equivalent of a stolen copy of Photoshop.

These questions arise:

-  Does this argumentation hold under Danish law? To which degree? Are there any law suits known where this has been argued by someone in court (successfully)?
- How does one heal this: 
  - If nothing happened: Remove one of the conflicting FOSS packages?  

####### Restrictions on outgoing licenses.

Basic question is: Multiple legal texts (licenses) exist trying to govern the same work. Which conditions win?

Example (based on positions often argued by corporations):

- A FOSS package is published. The publisher selects an outgoing license, e.g. MIT (a very permissive license)
- The FOSS package references third party FOSS packages. Some of them licensed with more restrictive licenses, e.g. the GPLv3.

- Maybe the FOSS package is integrated into a commercial solution that is then deployed or distributed only in binary form (for money).

It is then argued (e.g. by counterparties raising claims)

- The resulting FOSS package can not be legally/effectively be published with the outgoing license selected by the publisher. In this example MIT.
- The reason is that the more restrictive license overrules the more permissive license (in our example the GPLv3). The more restrictive license has impact as the combination of the two works (our FOSS package and the referenced GPLv3 FOSS package) created a derivative work upon which the GPLv3 is applicable.
- Thus inclusion of the FOSS package into the commercial solution is not legally possible as there is no offer of the source code. 
- They either make monetary claims for having illegally used their intellectual property until the infringement stops or request that their intellectual property be removed and the infringement be stopped. 
- Variation: They argue the above but request that our FOSS package be licensed under the more restrictive license.

Questions arising:

- Would this hold under Danish law? And to which degree? Are there any court cases with known outcomes? (There are some for the first variation under US/German law) 
- Does the "most restrictive wins" idea hold under Danish law? To which degree?
- The concept of "derivative work" and when something represents a "derivative work" is one more most disputed concepts of the GPL and related licenses. [US]() and [German]() literature has opinions here, are there interpretations for Danish law? 

####### License compliance on full publication
The following position can be repeatedly heard by corporations with "this is acceptable behavior". It should be cleared legally if and to what extent it holds under Danish law. (And practically this should be cleared for other legislations too by the corporations arguing this. However, Energinet is Danish, so that's our focus here.)

- A FOSS package is published by us exclusively in source code.
- The FOSS package references third party FOSS packages. 
  - Those are not copied into the source code distributed by us but referenced by a so called build system. 
    - A build system is another source code file containing references to third party packages. If compiled and deployed this will download the third party packages to the developers machine and combine them with the developers code into a binary.
- The publication contains only our source code, the build system file and the outgoing license we choose.
- The following is then argued:
  - We do not distribute third party FOSS code but only reference it, thus we do not have to give attribution by third party notices. 
  - We already fully publish all source code, hence we should be safe against publication requests  from restrictive licenses such as the GPL.
  - As long as we do not publish binaries (i.e. we compile our FOSS package, leading to combination with the third party FOSS packages and distribute/provide the results for others to download) we are safe.
- These questions come up on this argumentation:
  - Is it valid? Where are limits?
  - What happens if license compatibility issues are hit or the chosen outgoing license can not chosen due to inclusion (dependencies/references to) of other FOSS packages with e.g. restrictive licenses. (See above)
    - Is the resulting FOSS package legally distributable in code?

###### Participation (Incoming and outgoing Contribution)

See above for the definition of the two participation cases.
The following might also be interesting from a perspective of critical infrastructure regulations.

Incoming (Others participate in FOSS packages we published)
- This is the case after successful publication, in the registry example e.g. Elering or Statnet or a Danish or German citizen could participate and offer a contribution
- Liability / Warranty
  - The contributor introduced a defect with their change. We accepted their contribution. A third package uses our FOSS package and incur a damage. 
    - How does our liability to the third party look like? (Likely some limitations, see above sections)
    - How does the liability of the contributor to us (in case we have to settle something with the third party) look like? Does it differ if they are a commercial entity or a private person?

- Intellectual property ownership
  -  Who has which rights to the contributed change?
  - Can the contributor request retraction / removal of their change?
  - What attributions to we have to give them (different from: Do we want to give them)
  - The contributor introduces a change to which he does not have the rights, e.g. corporate secrets, patented inventions, ...
    - How does the liability situation above look here?
    - How do we ensure that they represent to us that that they have the rights to what they contribute? 
      - (A common approach in the industry is the use of the DCO representation by the contributing developer. There are different opinions towards the legal effectiveness of the DCO in its usual way of application.)


Outgoing (We participate in other FOSS packages)

Effectively the flipped version of the above. We should ensure that our liability and intellectual property situation is clearly defined.

Special here: The other FOSS package requests us to sign a CLA/CAA. Sometimes these contain language that would give the counterparty rights to the signing parties patents. It's usually a good idea to set limits on what to sign and what not here or at least have a process to hold contributions until such questions are cleared.

###### Operation / Deployment

This is a very extensive case of FOSS compliance. Usually this is handled through central IT policy and is a very large effort. Thus, this is not addressed here.

This short illustration serves to give an intuition of the challenge:

- Any other cases have dealt with publication/distribution of source code and the exchange of modification of said source code.
- Operation addresses what happens if source code that has been compiled and turned into binary code is exchanged or services are created for it and then offered for access by third parties.
- Most (if not all) FOSS licenses trigger on distribution and differentiate in their conditions between binary and source code distribution.
- On distribution of binaries or creation of services third party FOSS libraries are not only merely referenced but they are combined into one work (simplification) which is distributed as a whole as a binary.
- Thus conditions such as "provide attribution" "provide the license text" "provide written offer of source code" etc. come into effect. Failure to fulfill these conditions can lead to loss of license or termination of licenses for the used third party FOSS packages.
- Results of fulfillment of the conditions can be seen e.g. smartphone apps in the "licenses" section, cars (thick booklets upon purchase or in the onboard entertainment system, etc.), etc. 

It's a lot of effort, there's quite some legal/technical analysis effort involved, it's ongoing work. An analysis of the risks of enforcement and possible damage that can be involved is recommended. This is beyond this contract nevertheless.

### Open Source: Simplified cross-company collaboration with boundaries and hats through an explicit, de-facto standardized framework

What people do with our code must not be our problem.

Our problem is to foresee and harden against certain unwanted competitive and reputation damage scenarios.  Our second problem is explicit expectation management to limit public frustration and encourage informed participation.

What is the contribution of Open Source for us?

#### Collaboration
- Collaboration between corporate entities has - within very limited boundaries - been possible beforehand. 
- It did include extensive "red lining" and "lawfare" beforehand. 
- Open Source - by means of its standardized licenses and very well tried mechanisms of collaboration and reasonably working social contracts - allows to shorten the red lining process and while providing some more legal clarity and cleaner, more explicit expectation management.
- The above facilitates cross-country collaboration and collaboration with small entities such as private individuals.
- Investment in legal questions remains but moves from sometimes repetitive work to reusable decisions as cases become more standardized. Ideally this can make work more interesting :wink:

#### Public value and Re-use

- Open Source allows to built a shared commons with defined liability and expectation scenarios
- This can then be re-used throughout various parties without extensive contract negotiations beforehand.
- This also allows third parties to take up work that has been abandoned by others but is considered to still contain value.
- Direct and detailed visibility of work approach, work results and ability to interact with those involved allows to build trust through review in what is created. This can be especially valuable for public bodies.
  - Corollary: It also is very (longtime) effective in nuking any trust that might have existed beforehand if done wrong. :popcorn:  
    - Often, if something published is morally debatable or connected to a politically controversial topic, this raises the likelihood of the negative outcome. 
    - Another approach raising the likelihood of the negative outcome is cutting corners and disrespecting other people's work. Reasonable approach to approach this: Be diligent, work proper and give credit where credit is due.
    - Corollary to the corollary: Haters gonna hate. Be prepared for some backlash but see if there's any merit and address it with reason. If there's no merit, there's no merit. Still try to be reasonable.  


