# The Open Source domain - What's in it?

## Disclaimer

None of the following is legal advice or to be interpreted as such. 

The following introduces certain aspects of the Open Source (and, based on the work approaches introduced by Open Source, by that InnerSource) domain to further understanding of terms and field.

It raises, without being exhaustive or complete, certain questions around common risk items that are brought up for further legal analysis. Any risk parts are to be interpreted as question around possible risk to be analyzed and cleared up not statement of fact.

It further explains select technical matter in a strongly abstracted and simplified manner. Due to this abstraction, the information may not be suitable to fully decide certain specific legal situations. Detailed technical explanation and analysis is likely to be required in practical application. 

Any examples used are hypothetical and strongly simplified to provide an intuition of the matter explained.

The information is based on experience, common risk items being brought up in a German or US context, as well as information provided by the Danish digitalization agency in the [legal analysis document]().

Interpretation ans risk can significantly differ in Danish law and thus detailed legal analysis of the topics and possible resulting follow-up topics is strongly recommended. See [IT Retten]() book.

It is strictly recommended to seek advice from a FOSS specialized lawyer prior to consuming, deploying, publishing, or participating in Open Source or doing the same with commercial software using or embedding any Open Source component.

Authors notice: The consultancy mandate does not include legal advice, FOSS compliance consulting or advice on FOSS publication beyond technical, ways-of-working and common domain expectations. Any further advice, especially of legal nature, implicit or explicit, needs to be sourced from the relevant partners, e.g. a specialized lawyer. 

## Common Terms

Open Source is a combination of a cooperative/network-oriented business strategy/tactics with specific work methods and approaches.

It is realized through uncommon application of (mostly) intellectual property law legislation and means of technical automation.

Everything is applied to the field of software creation, modification and maintenance. The domain of deployment or application of software is not limited and thus, Open Source can find commercial application also with hardware.

To understand the field, certain technical terms and concepts need to be defined and understood.

### Historical and political background shaping visible phenomena, goals and  expectations

It has been created in a political environment strongly highlighting a non-commercial, liberal and self-sovereign agenda. 

Today, open source is a strongly commercially used approach, all trade practices, accepted rules, expectations and stewardship of the underlying legal tools is done through independent non-profit bodies largely running on the same agenda. Resupply of the pool of new talent with open source skills is to a large degree powered by the attractiveness of said agenda to the individual. It is highly recommended to align with this agenda where possible. The concept of "public money, public code" encourages this too.   

#### Open Source, FOSS, FLOSS
Open Source Software is often referred to as OSS.
OSS where the authors want to highlight the mentioned political background is called "Free and Open Source Software" FOSS.
OSS where the authors don't feel that FOSS does't not sufficiently highlight the political background is called FLOSS. 
In the end, all of it is Open Source Software as illustrated below, just with differently strict expectations on how corporate involvement is supposed to look like and what behaviours such software may show.

### Source Code, Compilation, Binary Files, Deployment

These are foundational technical terms from the process of software creation.

#### Source Code

Plain text files containing programming language text in a strictly human readable format. These files can be compared to "Blue prints" for mechanical engineering. Often just abbreviated as "code".

Common "languages" are C#, Java, Javascript, Python, C, Go etc.

A small piece of software can easily contain thousands of such text files.

These are written by programmers.

#### Compilation

The transformation of said text files into one or more binary files. 

As with a blue print a machine needs to be constructed from a blue print to "execute" said blue print. 

With source code the "execution"/"building" equivalent is called "compilation", followed by "linking" and includes the application of another program (in binary format, called a "compiler" or "transpiler") to the all required text files to "build" (the term is in fact also used) the program, i.e. transform it into binary format.

Sometimes, the compiler adds additional text files that were not directly supplied by programmers as source code.

#### Binary files

Sometimes also called "binary code", "binary" or "executable".

Non human readable files that contain data that can be read by a specific computer architecture. The computer loads&executes those enabling the computer to run Word.exe, Google.com, a thermostat, a car, an app, etc.

Difference to transforming a substation blue print into a substation: Compilation happens once per computer architecture and can then be copied to thousands of computers. However, compilation is required every time the source code has changed. (Thus: A new deployment is required to put changes in the source code in production, see below.)

A normal user has no interest in source code and does not see the source code but only the binary code upon executing the program of their choice.

It could be argued that a modern website also is mostly binary code due to the excessive amount of interactive features included in modern websites. Those are created using "transpiled" Javascript code.

#### Packages

Applicable to both binary files and source code.

A set of either text (or binary files) that are required to provide a specific feature.

A package has one or many associated owners and - given sufficient originality - is a work of art eligible to intellectual property protection. 

Two (strongly simplified) examples: The Linux kernel (about 2000-3000 text files in source, about 10 files in binary), Numpy (a popular package data scientists use, e.g. for grid forecasting models), Word (Tenthousands of source code files noone outside of Microsoft gets to see, 1 file Word.exe plus 100s of support files in binary) 

#### Deployment

The transformation from source code to something rendering practical service to a human being.

The programmers' main source code (all required packages) are combined with external packages, compiled and further packaged (currently very popular: "Docker containers"), copied to a target computer and then started. 

Critical difference: Only from here, ongoing cost for machines is incurred and data is processed. Any step beforehand causes negligible storage costs and miniscule computation costs. 

Examples:

- Word. IT copied it to your laptop and you run it there
- A smartphone app: Same, you download and run this on your smartphone
- A thermostat: Assembled by manufacturer, they copy it the device, once powered up it runs the final binary package
- A website/Google.com: Complicated packaging/assembly process, resulting packages copied to multiple computers in a Google datacenter, Google copies a package (the website you see) to your computer (in the browser, e.g. Edge/Chromium/Firefox) once you invoke Google.com, you run the website, website and Google servcers communicate, you get the information you want.
- A car: A datacenter on wheels, effectively all of the above.

### Real-life software creation today (Supply chain) or: Making money on the shoulders of giants.

In the 1980s and partially in the 1990s a program and function for a computer of material value could have been created from scratch by a limited number of engineers.

Today, most software engineering assembles enormous amounts of packages made by foreign parties and adds their own specific innovation on top of this. Commonly the relation between foreign source code and original, new source code is from 70 to 95% foreign to original source code. 

This also goes for packages that are added, i.e. those packages also contain enormous amounts of foreign packages.

Such "foreign code" / "foreign packages" are called dependencies. The dependencies of dependencies are called "transitive dependencies". The entire list of dependencies down through all transitive dependencies is called the "dependency tree".

Very small common software today (small websites, demonstrators, reusable visual components for a website) are made out of at least 200-500 individual packages.

Packages can be purchased from manufacturers (commercial off-the-shelf software, e.g. Word, SAP, a specialized forecasting library), custom created (by your own engineers, by externally contracted engineers) or procured as open source - meaning: an engineer downloads them from the internet and combines them into his work.

## Open Source, not Open Service

This is a crucial difference. 

As illustrated above, source code and binaries only cost storage space (think about the cost of a USB stick or memory card) and are inert, i.e. especially not able to process data on their own.

Once deployed, the code turns into a service. (In the case of web application like Google.com, deploying the code to make it a service is also referred to as "hosting".)

The service is able to process data, render services to users that can be sold and thus make money. However, running the service costs money incurs liabilities to the people whose data is processed, is usually contractually coupled with service level expectations etc.

Open Source absolutely exclusively refers to distributing the source code to third parties. 

There is no such thing as "Open Service" in the domain of Open Source. 

Once a person or company has the source code of an application they can make a service from it and of course: offer the service to the public for free if they choose so. However, all of the above liabilities, maintenance effort and all the bills arising from it become their problem. The person(s)/company offering the source code to the public is in no way involved here - they may even not be alive anymore. 

Hosting open source applications and charging money for enabling access to them is one of the main income streams of all cloud providers such as Azure, Google Cloud or Amazon Web Services. 

Often they add friendly user interfaces or modify them to be more comfortable or integrate with other commercial offerings they might have.  See [responsibilities and expectations] for what follows from this.

In the following everything only and explicitly talks about Open Source, not any form of deployment or service.

The exception is when "Operation" is explicitly mentioned - this refers to Open Source Software that has been turned into a service, standalone or combined with commercial code by Energinet. 



## 3 Modes of Open Source and 1 orthogonal approach making it all possible.

Interaction with OSS can be separated into three modes. They are briefly described below.

All of these, unless explicitly noted, refer to Source Code. In other words: Collaborative modification and creation of text files across corporate boundaries across nations. Collaboration happens with people representing other corporate entities or private citizens.

It is common that such people are not necessarily known by name (usually just pseudonym and email address). They are likely to only participate for a brief or undefined period of time until the goal or benefit they want to achieve for themselves is addressed.

The resulting product remains there forever, containing all the work of all its participants over time.

Perspectives used here:

- We/Us: Person employed by Energinet or bound by a countract to work for Energinet
- They: Any other entity. Could be here: A person representing e.g. 50Hz/Elia, Elering, Statnet, an individual. The individual could also be employed by us but participating in their spare time as an indivudual.

### Consumption

We take FOSS source code (or binary code created from FOSS source code by a third party, e.g. Red Hat) from a third party (e.g. Linux, Kubernetes, Tomcat, ...) and

- either add it into source code we create as part of a commercial product. We then compile the combined work, turning it into a binary and deploy this combined work.  
- take the binary or code and deploy it to render a service for us (e.g. a web server to host a web site)
- take the FOSS source code, modify it, compile and deploy the modified result to render a service for us.

The resulting service can be created for pure internal use by us or it could be created to be accessible by us and third parties. 

Each third party FOSS packages has one of the OSI certified licenses associated with it. This is called the incoming license. The set of all licenses found in alle packages is called the set of incoming licenses.

### Publication

We create source code with the intent to publish it to the world for use by them. Usually we continue to use this source code to consume it ourselves too.

We mark the source code files with a FOSS license and additional information with the intent to define our liabilities against third parties, set expectations what we expect others to do and not do with our published source code. We assume that the FOSS license will make some of these expectations enforceable.

The FOSS license we mark our source code with is called the outgoing license.

Usually such a publication happens by means of publication on a website like GitHub. 

Once published, our continuous work on this source code happens visible to the world and we now interact with third parties regarding questions or requests for participation. (see below). Since the third parties are not bound to us contractually and thus may have different objectives, we need to make sure that we carefully review what they offer and see into any different objectives they may have and how those fit ours.  

### Participation

The other two modes took foreign source code and used it (consumption) or had us provide source code to the world for others to use them (publication). There was no actual collaboration addressed.

Any cross-entity collaboration is called participation and the changes to the source code files exchanged are called contributions. The person providing the changes is usually called contributor. 

#### Participating in other people's projects (Outgoing contributions)

We consume code, find bugs (technical reasons for malfunctions in the program) while doing so, fix them (change a few lines of text) and don't want to have to apply those changes to the foreign source code forever. Hence, we offer the changes representing the fix (called a patch or diff - it's a redline effectively) to the original author of the source code from whom we took the code (or usually entire package) we consume.

This can also happen with patches that not only fix a defect but add new functionality. If the functionality fits their road map, is well crafted and will be beneficial to all future users, i.e. is not just highly specific to use and our needs, they are likely to accept them.  

#### Other people participating in one's own project (Incoming contributions)

We published a source code package.

The "Outgoing contributions" process happens, just with the roles of us and them reversed.

It is generally considered a sign of success of a published package to get incoming contributions. It will only happen after quite some marketing, raising popularity and well, resulting success, though.  

### Orthogonal approach: Ways of working

Contributors and package contributed to may reside in vastly different time zones, have significantly different work times and especially also may not have time to address contributions immediately.

This leads to a highly text-based, asynchronous, very explicit way of working emphasizing automation, self-explaining yet highly specialized tools and, well, a lot of text. Text allows easy searching, pin pointing, and commenting/review. (As well as translation in cases of language barriers.)

The practical lingua franca of Open Source is English, some small non-english language Open Source communities exist (Japan, France) however usually deviating from English strongly reduces the addressable market and likelihood of receiving participation. 

## "FOSS Licenses": Legal (intellectual property law) as a technical tool

Here, the [legal analysis document][] is a strongly recommended read.

### Basic effects and practices: 

- Entities publishing code do so for various reasons and with various expectations. These range from strong commercial motivations to increasing ones reputation to just risk free learning a technical subject in a hands-on way, etc.
- They hope to be able to enforce some of these motivations legally. 
- Other expectations are covered by implicit social code, explicit requests to people and sometimes ...raising shit storms on perceived violations against the perceived violators. This section only aims to cover legal aspects.
- As seen in the [supply chain]() section 100s of packages are part of any application or package. Also, the authors are engineers and thus not legally educated or interested. Due to the counter parties not being known highly standardized licenses (not contracts according to the legal analysis document) are used.
  - Those standard licenses are certified by the OSI. They are not changed or negotiated in use.
  - They are commonly classified into permissive (MIT, Apache2), restrictive (GPL, MPL, ...) and arguably "crazy" (WTFPL).
    - permissive intends to ensure reputation of the source code's authors
    - restrictive intends to ensure continued evolution of the source code by ensuring modifications/improvements are not kept by the modifying parties. Also, it tries to ensure reputation. 
    - Crazy: Engineers were fed up by legalese and drafted contracts to mock the concept of contracts.
  - All licenses try to exclude liability for the authors of the source code as much as possible. According to the legal analysis document this has limited effectivity in Denmark.
  - Some try to protect against software patents, try to protect trademarks (or brands or the publishers reputation, ...) that might be covered in the code.
  - Many terminate on violation of the conditions.
    - Some contain historical feuds leading to inability to be combined with others (Apache 2 vs. GPL2)
  - Some have an "update clause". Some license texts have versions (GPL2, GPL3, ...), some contain language where the intent was to "switch" to a newer version upon release of a new version of the license. (GPLv2+).
  - Almost none of the contain a choice of legal system clause. Thus they have to be interpreted under the local legal system - Denmark in our case.  

Often, the conditions depend on technicalities, thus technical interpretation and a legal-technical collaboration is important here. Specialized FOSS lawyers are used to this. 

There are some books on this for German and English interpretations for common scenarios, I know of none for the Danish system. The legal analysis document provides a hint to two books for Denmark.  

### Sources of legal impact from the licenses

#### Liability
Upon publishing of source code we will apply a FOSS license. 
It is the nature of software (and of course everything else that contains software), especially software that can be accessed in an unfinished state, that it will contain lots of defects and may lead to ugly losses and damages if people deploy it. 
We need to know how to best limit our liability using the FOSS licenses and appropriate marking of source code to ensure the licenses we choose to apply are as effective possible towards our goals.

The same goes for outgoing contributions - the patches we provide could lead to defects in the package accepting them. If that package is used by others these defects could cause damages/harm to them.
We can not apply or choose a FOSS license of our choice upon outgoing contributions. 
We need to know how our liability upon contribution looks like and how we can best limit it. (Or from which actions to refrain as the liability can not be limited enough.)

#### Warranty
We consume code, are subject to losses or damage due to a bug in the package we consume.
Can we claim damages against the authors? Two cases come up:

- We have a support contract with them, e.g. Red Hat Enterprise Linux
- We don't, i.e. we just downloaded source code or a binary from the internet and deployed it.

This effectively is the inverse of the Liability situation illustrated above.

#### Legal use of open source packages

As illustrated above, the FOSS licenses are conditional. 

Thus, to be able to publish or consume legal software (and not illegally distribute foreign intellectual property) we need to abide by those conditions.

To abide by those conditions, we need 

1. a) to know what packages we employ and 

2. b) what conditions from 

3. c) which packages we need to abide by. 

4. There is software generating such lists. Since the licenses are standardized, the set of conditions is manageable, even if 100s of individual packages are involved.   


A condition are to attribute the authors on a finished product in a certain way (permissive licenses). Another common conditions is to provide changes or source code (restrictive licenses).

Some conditions might be unacceptable.

In some cases combination of certain packages based on their licenses may be impossible. (The licenses conditions' are mutually exclusive). We may need to clear certain cases of this. 

The FOSS licenses often provide proposals how they would like to see those conditions filled. There is common, technical trade customs to fulfill the conditions. 

We will need to clear with legal if the trade cusotms legally fulfills the conditions under Danish law. We might need to find the smallest possible fulfilling execution in certain cases. 

This process is called FOSS compliance.

We will need to address this based on a legal risk estimation based on legal reality and current legislation around intellectual property law in Denmark as this the evolution towards here is usually an ongoing process.

#### Software patents and trademarks
Some software implemented innovations can be patented. According to the [legal analysis document]() Denmark does not do software patents but the exist in reality nevertheless.

Some licenses have certain aspects of patent protection or terminate on patents claims. 
An evaluation of the risks and chances here, especially given novel and innovative material being developed by us, is strongly advised. It might be desirable to ensure that certain common material is not patented to remain accessible by all interested parties.

The same goes with foreign trademarks or trademarked material embedded by us. We need to either remove any such material to prevent abuse or atain knowledge around boundaries here.
Some licenses contain certain trademark provisions. If used, evaluating their effects under Danish law would be interesting. (ASF 2?)

#### IP ownership, coherent IP ownership (DCO, CLA, CAA)

We saw that a OSS package is a work of multiple authors from multiple entities. They will have multiple goals, goals that might evolve to be mutually exclusive or hard to combine.

Also, people might violate the boundaries of use that was intended by the original group authors or tacitly accepted by other people that contributed to it later on. Violations could be

- selling as commercial software for a lot of money what was supposed to not be sold, especially not without providing the source code (variations on restrictive licenses).
- abusing trademarks or affiliations "Endorsed by Energinet" where that might not be the case. Distribution of our FOSS published software with malicious code that is then attributed to Energinet. (Something the ASF tries to prevent)
- Claiming software patents against the publishers (there a termination-on-patent-enforcement clause in some FOSS licenses)
- Not giving us the due credit or claiming our work as their own work. (Classic FOSS compliance enforcement)
- People contributing code to our packages they do not have the legal rights to contribute, resulting in an undistributable / illegal package for us. (Something the DCO tries to address)

Enforcement might require ability to speak for all authors. Or it might not. The [legal analysis document] writes about this. The ASF tries to enable defending patent, trademark and compliance violations on behalf of the authors by requiring sign-off of a special document prior to contributing, the ASF CLA. 

Another case, common with commercial/profit-oriented publishers (e.g. GitLab, MySQL), would be to have the ability to offer a product based on FOSS source code  with a "normal" full commercial contract and a (usually very restrictive) FOSS license. Thus, commercial entitites can choose to abide by the strong restrictive rules or buy the commercial license to e.g. be free to embed the product into a commercial offering (as much as the contract allows that).

For this, they also need the ability to license, sublicense, relicense, etc. all of the source code as they see fit. This is usually also done by requiring sign-off of a special contract (CLA) requesting these rights from contributors or even requiring sign-over of the IP to the other entity (CAA). 

Usually, FOSS packages requiring a CLA or even CAA see significant a drop in contributions due to the additional red-tape involved. Often trying to get a corporate entity to sign such a CLA takes long delaying contributions significantly. 

Depending on the desired outcome, it might make sense to use such a contract.


### What to expect from a license and what not - FOSS Governance

Based on their nature what can be achieved with FOSS licenses is rather limited. As the [legal analysis document]() states, FOSS licenses are licenses, not contracts under Danish law.

Also, some parts are likely nothing that should be regulated legally but with tacit rules, i.e. a "social contract" (of course, such expectations can be put into writing and could even be taken into account on legal discussions). 

Additionally, since the text of the existing OSI accepted FOSS licenses may not be changed (or else they loose acceptance and ability to be digitally controlled in a feasible way), remaining parts are expected to be stated as "social contract".

This field is what's known as FOSS governance. 

#### What you can't prevent

Something that crucially part of Open Source is the ability for people to take your work, duplicate it entirely and try to start a new community from it. This is called "forking". 
Here's when this happens:
- It often happens when someone is unhappy about governance or direction of the package. If they can make their place more attractive than yours, most people will move to place their contributions there and even deploy their fork and not yours. In that case you move from publisher to consumer of what you started. (Or end up continuing your work for yourself, without help or interest from others.)
- The same can happen if a publishers stops working on their package, it becomes "abandoned". Another party takes it over and continues work, people move there.
- Sometimes these forks deviate completely, sometimes they briefly exist and then converge again or there is a back and forth between forks.

If you choose a permissive license:
- People could start a commercial business based on your code and sell binaries made from your code without returning anything. They might also try to put you out of business or leach from your innovation. (A legal question would be to see how far the permissive licenses are enforceable and such a case would be allowed. My unlegal observation: As long as proper attribution is given this appears to be accepted.)  

In general, diplomacy and awareness and understanding of "competitors" is a valuable skill to deal with these effects before they turn sour. Sometimes it can't be prevented, so keep that in mind before to have the required aces up your sleeve to prevent commercial damage. Aces could be non-publication of certain aspects of a product, choice of license, use of CLA for certain parts, etc.  

#### What common FOSS governance questions are

##### "Running the show" or getting write access.
Open Source actively asks for contributions and work across corporate boundaries. 
Thus, a common question is what happens if a party external to the original publisher contributes so much and with such a high quality or show very high engagement that one could consider that "they run the show" (with the original publisher). 

This is considered the funnel from user to contributor to trusted committer or maintainer. The latter two have write access to the packages which is generally considered to be "they run the show".

With write access they can decide what source code contributions get added to the source code and what don't. They will have to justify that decision with the people making these contributions or else risk loss of contributors or even users. 

##### Product development, roadmap - having a say on the future.

A trusted committer or maintainer is a mix of product manager/owner, technical lead,  engineering manager and general cat herder or secretary.
As mentioned they accept or deny contributions. Also they bring the package forward in general. This is especially important if there's additional developers in the same company as the trusted committer. Having a roadmap or definition of the future, e.g. a vision and some principles facilitates such decisions and explanation of them to others greatly.
If there is more than one trusted committer, there needs to be a way to agree upon what gets accepted, what the future and roadmap looks like. This can range from very ad-hoc to full corporate board style. It can change and needs to be decided based on what fits by the trusted committers (and the corporations behind them if there are any).

If there are multiple coherent packages that make up a FOSS product, a product definition and associated strategy helps to inform decisions what contribution and what code part goes into which package.
Each package can have different governance approaches.

Imagine you have a product you published as FOSS where you want to have the full control of the future and be able to chance that quickly in radical ways without having to align with others from outside your company. This might be case if you attempt to build a commercial offering from it (see GitLab etc.).
You might not be interested in having trusted committers from outside of your company, but be very interested in contributions as they might help you fix bugs or bring in good new ideas.

In such cases it is on you to make this clear to everyone upfront or else people might invest significant effort only to hit a "glass ceiling" at some point. This might lead to loosing them or even them forking your package - while they have very high knowledge and engagement in your product making success or the fork more likely.

Imagine you are interested in projecting an image of maximum vendor independence, trust and acceptance - in such cases it might be desirable to have trusted committers from all major contributing entities. At the same time, in such cases reviews and acceptance decisions need to be a lot more rigid to ensure quality and actual independence. 

The SFOSC offers some pre-packaged, "standardized" examples of how such governances can look like under various conditions. They can be taken as inspiration but should not be copied verbatim.

Any governance can evolve over time. Thus, if there are multiple trusted committers involved having a way to agreeably enable such an evolution is important.

##### Technical tools for product choices
This deals with strategically using certain FOSS license features hoping to achieve certain effects.
All of the below is strictly not legal advice but "FOSS license folklore", may not work under Danish law and should be closely discussed with specialized legal counsel to evaluate if they actually work in the desired way. 

You publish code, offer a SaaS product based on it and don't want others to also offer a SaaS product just adding minor changes: The was the design principle of the AGPL, it was killed by hyperscalers by hosting the unmodified product, leading to source-available/non-OSI certified licenses such as the license change of ElasticSearch. Tread very carefully here. 

You want to force others to publish the modifications they made? This is what the GPL/restrictive class was designed for. However, you'll need to a) find changes, b) they actually need to publish them or, if they do not, you need to prove that they don't and have to and sue them based on this. The extent to which this is possible may differ based on legal system court and case details. Again: There's a lot of good will and diplomacy involved in FOSS. Try to prevent having to enforce things here.

You need to ensure certain patent and trademark issues: Certain licenses contain language to protect what you have here. Another approach would be to remove any trademark, visual IP etc. from what you publish preventing obvious, easy abuse in the first place.
Discuss the actual protection ability with specialized legal counsel. 

You want to prevent your source code/package from being combined with certain other source code? There are certain incompatibilities built into certain licenses. A famous example being GPL and CDDL, very similar in concept but uncombinable. Made to prevent inclusion of Sun/Oracle property into the Linux kernel. Has been circumvented in various technical and legla ways these days. 
Try to avoid this if possible at all.

You want to enable maximum adoption without any care of what happens to what you created, some liabilty protection as long as you are attributed properly. "without any care" included code being commercialized resulting in a competitor arising from this, code being used against you, code being integrated into ethically questionable endeavors, etc. This is the raison d'etre of the permissive licenses such as MIT or BSD.

If your legal system provides this: Public domain. You negate even that you created this, you don't want attribution, it's just out there. Use at your own risk. 


### FOSS licenses work on code, Creative Common work on data.

What you can do with source code, you can do with data.
Data might be other text (like this one here), images, raw material for images (e.g. design templates), or raw data such as a energy system forecasting data (e.g. to train AIs with it).

There are similar standardized  licenses for this, with one of the most popular being the Creative Commons licenses. 
All legal effects listed above apply here as well. A detailed legal evaluation is required here if they are supposed to be used. The [legal analysis document]() does not write about the creative commons.
The licenses also have shorthands indicating the template that is used.

Common variations are (abbreviated according to the website, see the full license text for the legal details. See a specialized counsel to see into actual enforceability or other related issues): 
- Do you want to prevent changed versions from being distributed: ND attribute
- Do you want to prevent commercial use: NC attribute
- Do you want to enforce changes being published under the same license: SA attribute
- Attribution is always required with the following attribute: BY


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

## Public Money, Public Code: Doing FOSS as a public body

Here, the [legal analysis document][] is a strongly recommended read as well as the [Energinet regulatory legal memo]().

As a publicly owned TSO that runs on public money, we are bound to additional special rules.

Those rules could from concerns of critical infrastructure operation (NIS2 derivatives) or strict regulations on the use of public money or non-competition regulations as public body.     

We have to interprete the regulations and rules here and for all product informing their strategy, see the [Energinet regulatory legal memo]() for non-competition rules. 

A possible interpretation could be to argue that Energinet is limited to providing and maintaining a public good that others (e.g. Danish companies such as Mjølner et al) could offer services around. 

In such a case it could be reasonable to take measures to ensure that the public good remains a public good and improvements by others are brought back to it. This could (but does not have to) lead to restrictive licenses for certain parts of FOSS packages published by us.

Rules coming from the IT security and NIS2 side could lead a need for special reviews of contributions or general regular reviews/audits or additional tooling to ensure quality and safety of the created product. This might also be a an source of liabilities we have against others.

The source/service separation is to be made here again: FOSS source code published by us and modified by others through contributions is inert and can not harm our critical infrastructure. Only when deployed and introduced to the critical parts of our infrastructure damage can occur. Thus upon passing this boundary additional checks need to be in place. This is an Operations and IT security topic though that is not addressed here.

- Corollary: If another TSO chooses to use deploy our published FOSS package it is their responsibility to ensure that it fits their critical infrastructure security checks.

- [] TODO: Add interpretation and links of boundaries of the  Energinet memo here and clear them with legal
- [] TODO: Add pointers to rules arising from NIS derivatives etc.

## Private Money, Public Code: Doing FOSS as a private entity

Not all TSOs (or other corporations) act as public bodies. Thus they may have to earn money with open source (e.g. to satisfy profit expectations of their shareholders).

This can lead to desires of monetizing Open Source in various ways. See the strategy guide and the SFOSC models for information on what interests and approaches might be interesting for them.

As a public body we likely do not need to monetize FOSS. 

To further interest in adoption of the public good we create, we might want to enable certain aspects of monetization in what we publish. This can be done by strategically selected governance decisions and matching use of FOSS licenses as well as matching boundary definitions of the FOSS packages and products.

In any case, this is an individual discussion that should be discussed individually. 

A common monetization would be to enable multiple parties to offer implementation consulting or operation assurance around our packages. However, they then have to build then necessary knowledge and ability to support and provide assurance. We can make our FOSS packages a friendly and cooperative place to collaborate and think about who decides about the roadmap/acceptance of patches (see above for considerations of who can become a trusted committer) but not much more.

Other options could be - depending on the architecture - to enable other companies to host our FOSS packages, as central instance or decentral instances offering certain services to others in exchange for compensation. Analog example: We develop an email protocol and server application, other operation of the software following this standard for money - think Gmail, United Internet, ... 

## FOSS strategy: Making money by giving things away.

Kurzer Anriss der Möglichkeiten mit direktem Link Verweis auf die WP und das Intro Dokument -> Das ist am Schluss Business, nicht mehr Legal.

### Losing money by giving things away.

Hyperscaler fun, wie FOSS Lizenzen gegen einen gedreht werden. 

Punkt to be made: Be vigilant, understand the domain, see cautionary signs and react.
