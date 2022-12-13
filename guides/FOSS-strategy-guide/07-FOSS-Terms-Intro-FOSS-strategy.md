# Intro to FOSS strategy

This document introduces certain aspects of business strategy and common behavioral expectations supporting those strategies in the FOSS domain.

It is strongly recommended to read the [Intro to FOSS Terms guide](../FOSS-Terms-guide/) beforehand to understand foundational concepts, boundaries, terms and mechanics of FOSS, i.e. Free and Open Source Software.

While the FOSS Terms guide addresses a more constraint, technical and legal driven perspective, this guide addresses a more business driven perspective. However, as FOSS is a mixture of software engineering (domain), legal (tools/mechanics) and business/social (strategy+incentive building, ways of working), attempting to neglect one of the aspects is a reasonably safe way to trouble.

## Overview 
Creating FOSS costs money (or at least time) as there are at least software engineers involved, often more and other roles. To some degree, such work can take place as a hobby of a software engineer. Such works can also grow in unimaginable ways, e.g. Linux, the hobby project of a Finnish computer science student.

Usually any larger work will need significant investment of time and thus money. Especially sustaining a software in the longer run, even more so if it is widely used, requires dedication. Often, maintenance work is far from attractive and thus does not attract hobbyists. Comparison: Nobody works for the municipal waste management services for free because it's such an attractive job. 

Thus, much of FOSS strategy consists of finding and keeping the resources to build things and to keep them alive. The difference between classic commercial products and FOSS products is that in-kind support from various parties profiting from the product is a rather common source of resources.

Often, in projects with a tall goal, time lines defined beyond "it's done when it's done" or a subject that is more valuable or enticing to commercial entities the bulk of the work is sponsored by said corporate entities, usually by paying the software engineers and other people involved.

## Challenges
This brings up certain challenges:

- How to justify the investment on the long run?
  - There is a tacit expectation that a FOSS effort (especially a company sponsored one) is cared for indefinitely. If not it will be considered "abandonware" and might be taken over by others if they consider it valuable. A good course of action is to be explicit in the expectation management towards users here.
  - Does it have to pay for itself (ROI>=1)?
  - Can it be cross-financed through another activity? If so, how and why?
- If participation by others is desired, making a clear case why they should do so, how and what they can achieve or expect is important. See the [FOSS governance chapter in the FOSS Terms guide]() for this too. 
- Usually corporate projects tend to strongly use a "us vs them" boundary and identity. FOSS *weakens* that boundary and identity. It usually does not remove it entirely. 
  - The middle ground and the boundary needs to be handled in a comfortable and predictable yet safe way. 
  - Usually corporate software projects and products are created in a strongly plan driven "agile" system. Interactions from the outside may in their originating organization be plan driven too, however, to you they look unplanned, can not be planned and appear like interruptions. Thus, integrating "Agile" and Open Source is another challenge. One that is addressed in another [guide](../opensource-and-agile-guide/).
- Participating in other people's FOSS efforts or publishing your own FOSS efforts is significant effort. 
  - You can't do shortcuts anymore as others will see all shortcuts you take. 
  - Communicating as briefly and implicitly as common with corporate projects will make it hard to impossible for external bystanders to participate. Which you might want.  

These challenges in general revolve around designing incentives, a classic part of business strategy. However, this variation is more interactive and participatory as opposed to a more transactional approach in other strategies. 

A common comparison is the agricultural cooperative or other non-profit cooperatives.

Other, strongly marketing driven, approaches such as one comparable to e.g. the "loss leader" strategy are existent too. Given that Energinet is a public entity, some restrictions regarding applicable strategies exist. See the [FOSS Terms guide on public sector specialties]() and the referenced Energinet legal memo for this.



## Common FOSS strategies

All FOSS strategies are - as business strategies in general - not cookie-cutter capable or guaranteed recipes for success. They are compressed abstractions of what has worked for some products and people in a certain context and time, possible more than once. (Red Hat as example is famous for having been a "once only" story.)

Deliberate strategic use of Open Source publication is the ultimate evolution of Open Source capabilities of any company. This can be expected only after years of continued evolution. See also page 10 in the [Linux Foundation OSPO study](https://8112310.fs1.hubspotusercontent-na1.net/hubfs/8112310/LF%20Research/Evolution%20of%20the%20Open%20Source%20Program%20Office%20-%20Report.pdf). You can always try and learn – but don't expect wonders.

The following collection isn't complete, precise or authoritative. Try to understand them and the dynamics, give it your best try, hope for the best try to record the results and evaluate the outcomes so you can learn and hone your expertise.

Take these leading questions to for all strategies:
- If you use someone else's FOSS: Why would they put it out for free and what follows for me from that? Is there any money made? Do they need to make money?
- If you publish FOSS for others to use: What do I expect others to do, why do I do this, how do I finance the extra effort, etc. 

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
You build something free, it becomes popular. Corporates start to use it. They  now need features your average SOHO/private user does not need, e.g. enterprise SSO integration or high availability. 
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

Your competitors or members of the general public may not like what you're doing. Or they like it, but they want your money without investing your effort. 

Thus, there are common counter strategies or ways how those could devolve. A few examples are illustrated here.



Making money by giving things away.

Kurzer Anriss der Möglichkeiten mit direktem Link Verweis auf die WP und das Intro Dokument -> Das ist am Schluss Business, nicht mehr Legal.

### Losing money by giving things away.

Hyperscaler fun, wie FOSS Lizenzen gegen einen gedreht werden. 

Punkt to be made: Be vigilant, understand the domain, see cautionary signs and react.
