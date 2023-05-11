# Introductory Suggestions for FOSS product management

## Table of Contents
1. [Intention and Scope](#intention-and-scope)
2. [FOSS Product Management](#foss-product-management)
3. [Working with the Suggestions](#working-with-the-suggestions)
4. [The Steps](#the-steps)
    - [Step 1: FOSS Product Definition](#step-1-foss-product-definition)
    - [Step 2: Mapping the Definition to Possible Code Collections](#step-2-mapping-the-definition-to-possible-code-collections)
    - [Step 3: Building a Strategy Hypothesis](#step-3-building-a-strategy-hypothesis)
    - [Step 4: Matching the Hypothesis with Reality](#step-4-matching-the-hypothesis-with-reality)
    - [Step 5: Separate Components in terms of Availability](#step-5-separate-components-in-terms-of-availability)
    - [Step 6: Apply Common FOSS "Tools" to the Components](#step-6-apply-common-foss-tools-to-the-components)
    - [Step 7: Apply Governance Structures](#step-7-apply-governance-structures)
    - [Step 8: Consider FOSS Marketing Efforts](#step-8-consider-foss-marketing-efforts)
    - [Step 9: Delivering the Work into Reality](#step-9-delivering-the-work-into-reality)

## Intention and Scope
This short document illustrates common topics that can be beneficial to go through when "running open source projects". 
It is phrased as mix of high(er) level questions and working instructions. 
It is by no means complete or will lead to a guaranteed, repeatable or even positive outcome.

It can provide some guidance and intuition on the work to be done.
Please extend this with pre-existing technical- and product-management knowledge you may have.

## FOSS Product Management
In the end, FOSS product management is still product management. 
It is, however, specialized in certain ways:
- Your final, released FOSS product is open source code. 
    - To some degree, a friendly atmosphere with a certain drive and intention towards newcomers (who then can understand what you are doing and possibly contribute)  is also part of the product. You could call it "the community" around the open source code.

Hence, this style of product management is
- Highly technical
- Decentralized as in decisions are controlled by a (subset of a) community or takes the community into account in a more direct interaction in decision-making.
- Centered around an often more non-commercial, "public good" oriented set of goals.
- Your resources are not limited to "your engineering team" and can extend to external partners and/or contributors. 
    - Do not see them as external outsourced workers you can control or command as your own engineering team.
    - You need to find common incentives or ways that fulfill goals and value for external parties while still adding value to your product.
    - You usually can't control the schedule of execution. If you need something done in controlled way, you either need hybrid partners or just do it using internal resources. 

The public good approach usually requires advancement of the community's goals. Thus, a way to roughly elicit such goals in the community is needed.  
    - This does not exclude having separate commercial offerings with classic commercial goals. However, to be viable, the FOSS offerings need to be valuable and useful on their own, without the classic commercial product to draw attention and collaborative investment from others.


## Working with the Suggestions
This document lists 9 overall steps to take in order to reach maturity in product definition and project management. 
Although they are to be executed mostly sequentially, it may be beneficial to do iterations between some steps, especially step 2 and step 3. 
Much of the entire cycle from 1-9 also will be your continuous adaption loop. 
Start with this. Try to understand the dynamics as you're doing the steps, figure out what works for you (see FOSS-common-success-criteria.md), adapt and continue.

## The Steps

### Step 1: FOSS Product Definition
- Component separation and definition of each component
    - Define the individual purpose and story of each component

- Context: Relation and boundaries to other projects, companies and/or organization
    - Define separations and interfaces to these
    - Think about an initial possible narrative / story that binds it all together and explains how your project provides value

### Step 2: Mapping the Definition to Possible Code Collections
- Map the component definitions and separations onto code collections. (different libraries/repositories) 
  - The final releasable product of FOSS is a carefully crafted code repository with publicly available source code.
  - The final releasable product of non-FOSS can be a services, e.g., SaaS, webservice, hardware product, app, or data. 
      - A combination of the earlier two is possible, e.g. hosting the FOSS as a Saas. However, this goes into strategy.

### Step 3: Building a Strategy Hypothesis
- Based on your product definition clarify:
  - Could some parts be monetized? 
      - Which parts are commercially differentiating for our enterprise?
      - A short, written up 'why' can be useful here
  - What could be justified where? 
  - Which parts are uninteresting to be monetized?
- Come up with hypotheses and ideas on what to open and what not to open.
  - For all cases of "open":
    - Write down why it makes sense to open it.
    - Evaluate if making it open will promote success, what may not happen and what you want to happen.
  - For all cases of "commercial"/"closed" parts:
    - Write down why it makes sense to close/commercialize it.
    - Evaluate if making it open will promote success, what may not happen and what you want to happen.
    - How can this closed part support the open parts and vice versa?
- Evaluate if the definitions of relations and boundaries are clear enough for everyone or need extra definitions
  - It can help to think about target audiences, both in business and tech, and overlaps of those.
  - It can help to think about competitors, research their behavior, etc.
  - Consider doing expectation management around readiness of making things open. 
  - Think about any sensitive material you might share. 

Steps 2 and 3 (and maybe 1) can be iterated back and forth until a stable enough first hypothesis and separation exists that you or all people with skin in the game are willing to try.

### Step 4: Matching the Hypothesis with Reality
 - Does the output of steps 2&3 match our corporate goals?
 - Does it bode well with any potential collaboration partners interests as far as we know them?
 - Will an outsider find this interesting to invest time and potentially money in? 
     - See if you could find outside people - to try your thoughts against.
     - "Outsider" may have different definitions, depending on the situation. It could be an unrelated colleague, but also some completely independent non-project participant. 

 Adapt the output of the previous steps with any of the reality insights here.

### Step 5: Separate Components in terms of Availability
- Separate your components into your planned availability:
  - Remains closed 
  - Published internally across the organization (InnerSource)
  - Published with partners ("extended InnerSource" if you will)
  - Worldwide FOSS publication

Each part now has
- An availability classification as above.
- A hypothesis around business strategy.
- An collection of argumentation points for following such strategy.
- An initial idea of events you assess a must-not-happen/can happen/would be great if it happens.
- A mapping of relationships and boundaries of your project from others. 

### Step 6: Apply Common FOSS "Tools" to the Components
- For each component that is supposed to become "world wide FOSS publication":
    - Write up initial expectations for governance structures (e.g. the path from user to contributor to trusted committer, who can become a TC in the first place, decision-making structures, contribution guidelines, etc.)
   - Define a selection of outgoing licenses that would support the wishes from step 5.
       - If there is already code: check if the incoming licenses allow for the desired outgoing licenses
       - Get help from the legal department to help choose one or several licenses to apply. @lenucksi can help formulating questions for them, not with the actual legal expertise.

### Step 7: Apply Governance Structures 
- For each component, at least starting from the "extended innersource" rated ones (rated in step 5):
  - Determine people to fill the positions defined in the governance structures in step 6.
   - Likely this will be at least one [Trusted Committer] for each repository/component.
   - Maybe there will be a separate [Product Owner] for each component as well. 
       - However, for smaller projects the Trusted Committer may take on this role as well. 
       - One person can - if the components are small enough - fulfill the roles for multiple components, i.e. be e.g. [Trusted Committer] in 3 components.

When you have chosen a person (or group of people) to take the decisions and apply them, remember to clearly and explicitly write this choice for governance down in an easy-to-find location to inform the community. 

### Step 8: Consider FOSS Marketing Efforts
- For all "world wide FOSS publication" (classification from step 5) artifacts:
    - Think about how to market to target groups. 
    - There is some difference  in marketing approaches between groups, depending on whether they are more technically focused or business-oriented.
- If in doubt, be humble and honest. Don't promise something that you can't fulfil. In the end, it's all 100% transparent, which will hold you accountable.
- Everyone active in the project, especially the technical people doing software development, will indirectly do marketing as well through their communications, purchases, actions etc. 
    - Empower them with the knowledge and skills to do so. There will not be centralized, controllable communication as with commercial projects. Media training may be required. 

### Step 9: Delivering the Work into Reality
- If you haven't done so:
    - Write up the results of the work
    - Bring the results to the components' repositories, or provide it as general organization content
        - This can include READMEs, contribution guidelines, decision-making policies, an open source policy, larger documentation pieces, setup of issue templates for issue tracking, project boards, review automation of various kinds, etc.
    - On the marketing-site, create matching websites and do according communication, community calls, participation in relevant events to promote the project, etc.
    - Bring up a repeatable process to safely publish "without takebacksies". 
        - This will likely include legal and IT security to mitigate risks

- Regularly revisit the process and your assumptions and hypothesis to check them against the market and community feedback as well as potential competitor behavior and adapt accordingly.
- Regularly take some time to step back, record lessons learned, things that worked well, things that didn't and to enjoy that you hopefully grew a working product with a nice community :smile: :tada: 

<!-- Anchorlink style --> 
[Trusted Committer]: https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/introductory/innersource-short-role-descriptions.md#the-trusted-committer
[Product Owner]: https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/introductory/innersource-short-role-descriptions.md#the-product-owner
