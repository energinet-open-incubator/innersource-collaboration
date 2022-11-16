# Introductory steps and questions from FOSS product management

## Intention and scope
This short document illustrates common topics of "running open source projects" in an introductory way.
It is phrased as mix of high(er) level questions and working instructions. 
It is by no means complete or will lead to a guaranteed, repeatable or even positive outcome.

It can provide some guidance and intuition on the work to be done.
Please extend this with and connect it to pre-existing technical and product management knowledge you may have.

## FOSS Product management - Term and differences
In the end, FOSS product management is still product management. 
It is, however, specialized in certain ways
- Your final, released FOSS product is open source code. 
	- To a certain degree a friendly atmosphere with a certain drive and intention towards a shared newcomers can understand is also part of the product. You could call it "the community" around the open source code.
- This style of product management is
	- highly technical. 
	- decentralized as in decisions are controlled by a "subset" of the community or often take them into account in a more direct interaction.
	- centered around an often more non-commercial, "public good" oriented set of goals.
		- The public good usually includes advancement of the goals of the community. Thus, a way to roughly elicit such goals together in the community is needed.  
		- This does not exclude having separate commercial offerings with classic commercial goals. To be viable, the FOSS offerings need to be valuable and useful on their own, without the classic commercial product to draw attention and collaborative investment from others.
- Your resources are not limited to "your engineering team" but can extend to external partner and contributors. 
	- Do not see them as external outsourced workers you can control or command as your own engineering team.
	- You need to find common incentives or ways that fulfil goals and value for external parties while still adding value to your product.
		- You usually can't control the schedule of execution, especially not in a way like scrum. If you need something done in controlled way like this, you either need hybrid partners or just do it scrum style and add it to the product. 
			- If you want to do this scrum style but openly, you need Open Source capable developers and product management to prevent embarrasment.

## How to work with this.
This guide lists 9 steps. 
Although they are to be executed mostly sequentially, there are iterations between the steps, especially e.g. step 2 and 3. 
Much of the entire cycle from 1-9 also will be your continuous adaption loop. 
Start with this. Try to understand the dynamics as you're doing the steps, figure out what works for you (see FOSS-common-success-criteria.md), adapt and continue.

# The steps
## 1 - starting FOSS product definition
- Component separation and definition
- Relation and boundaries between Energy Track&Trace ("the standard"), Project-Origin, and magic dust in the middle or around it
- Define individual purpose and story of those
- Think about possible separation / cutting points in these magic dust circles
- Think about an initial possible narrative / story that binds all those together in a plausible / believable way
  - The stickies can already provide some insight into peoples wishes and expectations

## 2 - Mapping purposes, stories etc to code
- Map separation and components onto code collections. (e.g. the registry / a blockchain library / ...) 
  - The final releasable product of FOSS is a carefully crafted code repository.
  - The final releasable product of non-FOSS can be a SaaS, webservice, hardware product, app, data, ... -> Important difference. 
  - A combination of the earlier two is possible, e.g. hosting the FOSS as a Saas. ~> This goes into strategy

## 3 - Starting to think about strategy
- Based on the envisioned separations:
  - What parts are commercially differentiating for your enterprise? How would the other participating companies answer this question? (You could ask them. Also: A short, written up 'why' can be useful) 
- Using common strategy sense and the FOSS strategy variations illustrated in the pre-read: 
  - What could be justified where? 
  - How could the parts be monetized, which parts are uninteresting to be monetized, etc....

- Based on this: Come up with hypothesis and ideas what to open and what not to open.
  - For all cases of "open":
    - Write an idea why it makes sense to open it
    - Think about how the business idea can be broken, what may not happen and what should happen to promote success
  - For the commercial/closed parts:
    - Same excercise as above, but also: How can the open things support the closed, how can the close support the open parts.

- See if the envisioned separations make sense or others come to mind.
- See if the definitions of the Relations and boundaries are clear enough for everyone or need extra definitions
  - It can help to think about target audiences, both in business and tech, and overlaps of those.
  - It can help to think about competitors, research their behavior, etc.

- It likely makes sense to leverage all the different minds and perspectives we have in the collaboration and write/discuss this openly, e.g. as open Miros, as iterative/reviewed text documents using GitHub, etc. 
  - It likely makes sense to do expectation management indicating readiness, state, open loops, etc. 
  - Also think about any sensitive material you might share. Try to work with a bias towards open, but not reckless. :wink: 

Steps 2 and 3 (and maybe 1) can be iterated back and forth until a stable enough first hypothesis and separation exists that you or all people with skin in the game are willing to try.

## 4 - Matching the hypothesis with the reality as we know it so far.
 - Does the output of steps 2&3 match our corporate goals?
 - Does it bode well with our collaboration partners interests as far as we know them?
 - Would you find this interesting to invest time and potentially money as an outsider? 
 - See if you could find outside people - to try your thoughts against.
   - Depending on the senstivity of the material "outsider" may have different definitions, e.g. an unrelated colleague or even an actual non-project participant. Act reasonbably. :wink:

 - Adapt the output of the previous steps with any of the reality insights here.

## 5 - Check separation and reasonable completeness.
- Use the individual parts and separate into
  - remains closed
  - publish with our partners first ("extended innersource" if you will)
  - world wide FOSS publication

- Each part now has
 - a classification as above
 - some current hypothesis around business strategy and must-not-happen/can happen/would be great if it happens
 - some ideas whether there is differentiating material in it.
 - Some handwavy argumentation that connects it to the others
 - A few thoughts on relationships, supporting, etc. and boundaries that separate it from the others. (Allowing a "which idea goes into which bucket" excercise)

In the previous steps and with additional outside work a common story and narrative has arisen that all of these parts sort of attach to and find a place in.

## 6 - Starting to apply common FOSS "tools" to our product thoughts
 - For each component that is supposed to become "world wide FOSS publication"
  - transform the information from step 5 into 
  - initial written up common governance expectations (e.g. way from user to trusted committer, who can become a TC in the first place, decision approaches, ...)
   - A document as in the ET&T project can help here. @lenucksi can also help with further discussions to turn expectations into written up expectation management.
  - select from the existing licenses to define a selection of outgoing licenses that would support the wishes from step 5
   - if there is already code: check if the incoming licenses allow for the desired outgoing licenses
   - We will need collaboration from our legal department (possibly also using the Digitalization Agencies' document on FOSS) here for the details. @lenucksi can help formulating questions for them, not with the actual legal expertise.

## 7 - Find people to fill roles that arose from step 6
- For each component, at least starting from the "extended innersource" rated ones:
  - Determine people to fill the positions determined from the governance discussions in step 5.
   - Likely this will be at least a TC for each repo.
   - Maybe there will be a separate Product Manager/Owner/... for a component
   - Reality is that both need to be able to take each others role in 60-75% of all decisions.
     - Often, especially in smaller components the TC and PO rolle will be fused in one person
   - One person can - given that the components are small enough - fulfill the roles for multiple components, i.e. be e.g. TC in 3 components.

 - If you ended up with board style governance for a component, you'll need to still have person (group of persons) to take the decisions and apply them. For that, they need to be clearly and explicitly written up. 

## 8 - Starting to think about FOSS marketing efforts
 - For all "world wide FOSS publication" artifacts:
  - Think again about target groups. Both technical and business oriented. Think about overlaps of these groups
  - Think about how to market to both groups. 
    - There is some difference between those groups in marketing approaches.
    - Listen to FOSS or technical people for the technical/developer focused marketing.
    - Of course, the other way round for the business focused markteting.
  - If in doubt, be humble and honest. Don't promise on one side what you can't fulfil on the other. In the end, it's all 100% transparent...
  - Everyone active in the project, especially also the technical people, will do marketing, communications, purchasing, etc. 
    - Empower them with the knowledge and skills to do so. There will not be centralized, controllable communication as with commercial projects.
    - It needs to feel authentic, honest and humble. Good developers will call absolutely any and all bluffs. Behave accordingly.

## 9 - Delivering all the work to the practical repositories and into the reality.
- If you haven't done so:
 - Write up the results of the work
 - Bring the results to the components' repositories, general org contents
   - This can be matching READMEs, contributors documentation, larger documentation pieces, descriptions of your work approach, setup of issue trackers, project boards, review automation of various kinds etc.
   - Prepare live demos where you can
   - Create matching websites and do according marketing, community hours, etc.

  - Bring up a repeatable process to safely publish "without takebacksies". 
    - This will likely include legal, IT security, and a business function high enough to ensure the "no takebacksies" effect.
    - Check again...now you could use the process to publish parts that aren't already published 
    - Use the skills and preparation you made before to now grow your product (and of course the potentially existing commercial products or offerings that are connected to the FOSS parts!).

- Regularly revisit the process and your assumptions and hypothesis to check them against the market and community feedback as well as potential competitor behavior and adapt accordingly.
- Regularly take some time to step back, record lessons learned, things that worked well, things that didn't and to enjoy that you hopefully grew a working product with a nice community :smile: :tada: 
