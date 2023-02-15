# Intro to FOSS strategy

This document introduces certain aspects of business strategy and common behavioral expectations supporting those strategies in the FOSS domain.

It is strongly recommended to read the [Intro to FOSS Terms guide](https://github.com/project-origin/origin-collaboration/tree/main/docs/introductory/FOSS-terms-guide) beforehand to understand foundational concepts, boundaries, terms and mechanics of FOSS, i.e. Free and Open Source Software.

While the FOSS Terms guide addresses a more constraint, technical and legal driven perspective, this guide addresses a more business driven perspective. However, as FOSS is a mixture of software engineering (domain), legal (tools/mechanics) and business/social (strategy+incentive building, ways of working), attempting to neglect one of the aspects is a reasonably safe way to trouble.

## Overview 
Creating FOSS costs money (or at least time) as there are at least software engineers involved, but often also more and other roles. 
To some degree, such work can take place as a hobby of a software engineer. 
Such work can also grow in unimaginable ways, e.g. Linux, the hobby project of a Finnish computer science student.

Usually any larger work will need significant investment of time and thus money. Especially sustaining a software in the longer run, even more so if it is widely used, requires dedication. Often, maintenance work is far from attractive and thus does not attract hobbyists. Comparison: Nobody works for the municipal waste management services for free because it's such an attractive job. 

Thus, much of FOSS strategy consists of finding and keeping the resources to build things and to keep them alive. The difference between classic commercial products and FOSS products is that in-kind support from various parties profiting from the product is a rather common source of resources.

Often, in projects with a tall goal, timelines defined beyond "it's done when it's done" with a subject that is more valuable or enticing to commercial entities, the bulk of the work is sponsored by said corporate entities, usually by paying the software engineers and other people involved.

## Challenges
This brings up certain challenges:

- How to justify the investment on the long run?
  - There is a tacit expectation that a FOSS effort (especially a company sponsored one) is cared for indefinitely. If not it will be considered "abandonware" and might be taken over by others if they consider it valuable. A good course of action is to be explicit in the expectation management towards users here.
  - Does it have to pay for itself (ROI>=1)?
  - Can it be cross-financed through another activity? If so, how and why?
- If participation by others is desired, making a clear case why they should do so, how and what they can achieve or expect is important. See the [FOSS governance chapter in the FOSS Terms guide](https://github.com/project-origin/origin-collaboration/tree/main/docs/introductory/FOSS-terms-guide/04b-FOSS-Terms-Intro-FOSS-governance.md) for this too. 
- Usually corporate projects tend to strongly use a "us vs them" boundary and identity. FOSS *weakens* that boundary and identity. It usually does not remove it entirely. 
  - The middle ground and the boundary needs to be handled in a comfortable and predictable yet safe way. 
  - Usually corporate software projects and products are created in a strongly plan driven "agile" system. Interactions from the outside may in their originating organization be plan driven too, however, to you they look unplanned, can not be planned and appear like interruptions. Thus, integrating "Agile" and Open Source is another challenge. One that is addressed in another [guide](../opensource-and-agile-guide/).
- Participating in other people's FOSS efforts or publishing your own FOSS efforts is significant effort. 
  - You can't do shortcuts anymore as others will see all shortcuts you take. 
  - Communicating as briefly and implicitly as common with corporate projects will make it hard to impossible for external bystanders to participate. Which you might want.  

These challenges in general revolve around designing **incentives**, a classic part of business strategy. However, this variation is more interactive and participatory as opposed to a more transactional approach in other strategies. 

A common comparison is the agricultural cooperative or other non-profit cooperatives.

Other, strongly marketing driven, approaches such as one comparable to e.g. the ["loss leader" strategy](https://www.investopedia.com/terms/l/lossleader.asp) are existent too. Given that Energinet is a public entity, some restrictions regarding applicable strategies exist. See the [FOSS Terms guide on public sector specialties](https://github.com/project-origin/origin-collaboration/tree/main/docs/introductory/FOSS-terms-guide/06-FOSS-Terms-Intro-public-sector-specialties.md) and the referenced Energinet legal memo for this.



## Common FOSS strategies

All FOSS strategies are - as business strategies in general - not cookie-cutter capable or guaranteed recipes for success. They are compressed abstractions of what has worked for some products and people in a certain context and time, possible more than once. ([Red Hat](https://en.wikipedia.org/wiki/Red_Hat) as example is famous for having been a "once only" story.)

Deliberate strategic use of Open Source publication is the ultimate evolution of Open Source capabilities of any company. This can be expected only after years of continued evolution. See also page 10 in the [Linux Foundation OSPO study](https://8112310.fs1.hubspotusercontent-na1.net/hubfs/8112310/LF%20Research/Evolution%20of%20the%20Open%20Source%20Program%20Office%20-%20Report.pdf). You can always try and learn – but don't expect wonders.

The following collection of strategies creating incentives isn't complete, precise or authoritative. They are also illustrated in a very abbreviated, shortened way. Try to understand them and the dynamics, give it your best try, hope for the best try to record the results and evaluate the outcomes so you can learn and hone your expertise.

The following leading questions should be evaluated for all potential strategies:
- If you use someone else's FOSS: Why would they put it out for free and what follows for me from that? Is there any money made? Do they need to make money?
- If you publish FOSS for others to use: What do you expect others to do, why do you do this, how do you finance the extra effort, etc. 

There's a set of articles around this, see there if you want to read more:

- [Wikipedia on FOSS strategies](https://en.wikipedia.org/wiki/Business_models_for_open-source_software)
- [TODO] Paper on FOSS strategies
- [TODO] Summary of other approache sources / deduplicate

### **Influencing/Setting** **standards to sell into**
(Using Energy Track & Trace as example) Energy Track&Trace tries to establish a standard that Energinet could build implementations for. Or operate infrastructure that makes use of such standards. 
- All of it assumes that the standard sees widespread adoption and thus demand for products that cater to it.
- Another desirable effect could be that only the presence of a common standard makes a given problem solvable. Thus, the standard enables new, innovative business that has not been possible before. 
- Examples: 
  - Internet standards such as SIP (telephony), Kubernetes, etc.
  - Map data collection, car telemetry data across car manufacturers

### Service & Support
You build something free, it becomes popular because it is useful. As the expert on the component you sell professional services, customization, and support and assurance contracts in case of issues in operation.
- A variation on this: You charge the first customer asking for a certain customization or addition of a feature and make the feature free for all after completion (or with a delay). 
  - This can lead to a game of "who's the first to ask and thus pay" that can be detrimental to the product. It's more frequently seen in FLOSS than in FOSS.
- Examples: Red Hat, Ubuntu, GitLab (to some degree), any company with support contracts on OSS

### Open Core
You build something free, it becomes popular. Corporates start to use it. They now need features your average SOHO/private user does not need, e.g. enterprise SSO integration or high availability. 
You sell those add-on components as commercial products with a good price tag. Usually you will combine this with Service & Support. You can also upsell this into a cloud SaaS product.
- Examples: GitLab, commercial FOSS distributions (Kafka vs. Confluence), Elastic Stack products (see below: the hyperscaler dilemma)

### Widget frosting
It‘s back to the 70s with this one. You don‘t care about software, but about selling your hardware. So you provide the awesomeness on top if only people buy your hardware.
This can lead to people making your product more awesome or you growing an enthusiast / modder community that can be interesting from a pricing perspective or even lead to innovations you can make part of your product.
- Examples: 
  - Intel's optimized compilers for HPC usage, to some degree: Apple‘s MacOS (the lower layers are open source – Darwin. ), …
  - PinePhone (enthusiast smartphone), Fairphone (part of the general approach)
  - Halfmatching: Android aftermarket firmware distributions (Lineage/Cyanogen/...) introduced certain features where comparable features were seen not too long after in the Android platform mainstream.

### Loss Leader: Devaluing your competitors offerings

 A service can be sold as a commercial, closed product (e.g. a container cluster operation tooling). You offer a mostly done product for free, devaluing your competitors offerings and destroying their business. 

You sell services and hosting for your product.

- Example: 	Kubernetes, Google Cloud Platform, ElasticSearch vs. Open Search (~AWS, Hyperscaler dilemma),  	
- To some degree: patent free video and audio codecs saving you license costs and bandwidth in your data centers (AVIF, H.264 etc. vs. 	Youtube etc.) 		
- See also: Forks

### Breaking up vendor lockins/turning markets from vendor to purchaser driven

You are bound to non-interoperating software from a small set of vendors that exploit all opportunities for vendor lock-in (e.g. cloud providers such as AWS, Azure, GCP). You obviously don't like that as they will use their price-setting power. You attempt to create a base product for such a domain that is popular enough to see widespread adoption resulting in the majority of tenders requesting support for the base product thus establishing a defacto standard forcing interoperability on the vendors attempting vendor lockin.

- Example: 
  - Attempts exist with Gaia-X, products from the Linux Foundation Energy, etc.
  - It could be argued that Kubernetes partially derives its popularity from that property of enabling cloud provider independence in theory.  	

- Making this work is a very, very long shot with not necessarily a light at the end of the tunnel...

### Commoditizing the complement
You want to sell a product that needs certain infrastructure. You want maximum adoption of the infrastructure. You don‘t want to care about maintenance and adaptation of the infrastructure to new environments. So you give away a piece of infrastructure that is  extremely useful on its own, make it easy to adapt to new environments, and offer certification and services on top that people really want once they have the infrastructure.
- Examples: 
  - Android, Chrome, …
    - Google wants to sell ads, not port their operating system to the next crazy ARM core from wherever.
    - They offer certification for Google services once its good enough and don‘t care that years from the start Sony DSLRs run Android as long as they don‘t have to invest resources there. 

  - To some degree: Kubernetes – selling Google cloud services and setting a standard 		eliminating competitors.


## Common counter strategies

Your competitors or members of the general public might not like what you're doing. Or they like it, but they want your money without investing your effort. 

Thus, there are common counter strategies or ways how those could devolve. A few examples are illustrated here.

### Open Once, Open Always
Once you stick an OSI license on an artifact and make it publicly visible on the internet, there is no way back. If you have a so called „permissive“ license on it (e.g. MIT, Apache2) even if you control the complete IP - and could thus decide to make it private or more restrictive – the freely licensed code will prevail and may be used by anyone as long as they abide to the terms of the license. Taking artifacts „private“ again will also lead to strong negative public reactions depending on how popular your artifact was before.

### Forks
This has already briefly been mentioned in the [FOSS Terms Guide governance section](https://github.com/project-origin/origin-collaboration/tree/main/docs/introductory/FOSS-terms-guide/04b-FOSS-Terms-Intro-FOSS-governance.md) but it is a fundamental effect of Open Source, so it's mentioned again here with a derived effect that had some high profile occurances in the recent past.

Usually this is the consequence of attempting to restrict or „take private“ an artifact that was popular enough. Sometimes it even suffices to decide for an unpopular way with a large enough part of the user base to have them take your artifact and develop it further themselves. 
While forking is one of the basic intended mechanisms of open source, if control of the direction of the product, revenue from the product in any of the ways illustrated above is critical to your business/part of your business strategy attempting to diplomatically keep things together is often a good idea. 
Forks can quickly surpass the original artifact in popularity, leaving the original in the dust with a lot of effort invested but no leverage anymore. 
- Examples: Nextcloud/Owncloud, Jenkins/Hudson, ElasticSearch/OpenSearch, OpenOffice/LibreOffice, Gitea/Gogs
- The **hyperscaler dilemma**: 
  - Imagine you follow an OpenCore / Service/Support / maybe parts of SaaS business strategy. 
  - Your license allows others to offer commercial hosting for others of your product (think AWS hosting Elastic Search). 
  - A competitor bigger and with larger economies of scale comes along and kills your SaaS business, your Service/Support offerings by offering what you offer cheaper and more convenient. 
  - What do you do? You could try to restrict the „commercial hosting“ ability even further. If the competitor has enough resources, they will fork your existing product and continue development on their own. They can fully open their code because it has no value to them as their SaaS offering and integration into their SaaS environment pays for it.
  - Examples: ElasticSearch/OpenSearch, Redis, MongoDB, ...

### Unpopular Open Core communities

Open Core requires you to control your core and to exert some control or ensure incentives for your non-open supplements to stay economically valuable.
This can quickly lead to communities that do not feel authentic or lead people to get the impression of being the „useful idiot“ providing free work for a corporate that is exploiting them. It can work, but it is a very thin and delicate path to walk.
- Camunda follows this to some degree with success. So does Mattermost.

### People breaking the Open Core supplements
Related to the above – imagine an Open Core product that sells specific high availability or enterprise authentication supplements.
An enterprise using the core product figures that the main product is useful enough to them that they need the supplements but their calculations and resources show that building the desired supplement themselves is cheaper than buying it for them. They decide to „publish what they build for the greater good“. 
You now have no-cost competition in your supplements you rely on to realize parts of your revenue. This could also be done by the enterprise to convince/nudge the Open Core company to integrate the built functionality into the core as a face-keeping way out for your company that at the same time removes the need to maintain what they built for the enterprise.

### Losing your own standard
You‘re trying to play the standardization strategy to make your plans be the default approach for everyone. You have invested x people and use board style governance based on majority. 
A bigger player (MS, Google, IBM, …) invests more people and money and manages to overtake your majority in the board. You now have lost (majority) control over your standard.

## Marketing (or: build it and they won't come)
There's a common saying: "Build it and they will come".
It is about as true and false at the same time as the "Open Source is more secure because when the code is open it's being constantly reviewed and all bugs are found automagically".

The reality is that especially if you have a corporate focused product that does not have ultimate novelty, solves a really bad hemorrage a gazillion of engineers have or is "technically sexy" (read: buzzword complete regarding a recent enough hot buzzword) that there will be a really large amount of other product competing for people short attention spans. 

This means that marketing will be required. Since the product you are marketing effectively is code, and you want adoption for said code, you will need to market to developers. 
Also, of course, to support allocation of resources for them, you will need to also market to business. 
Especially in the earlier development stages, where there is no polished product the primary target group will be developers.
Good documentation, technical depth, technically well made execution and something that is technically interesting (and of course buzzword complete to some degree) will often attract developers. Plus a friendly community where they can directly get technical answers. 
So don't build a "talk to sales" front-end, a ticket system or technically clueless product manager in between.  
Listening to what your developers would find interesting can often help.
