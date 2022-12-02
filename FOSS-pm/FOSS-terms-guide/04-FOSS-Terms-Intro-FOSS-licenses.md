# "FOSS Licenses": Law (intellectual property law) as a technical tool

As explained in [chapter two: 3 modes of FOSS](03-FOSS-Terms-Intro-3modes-of-FOSS.md) a FOSS package has a FOSS license put on it. 

These are standardized English language license texts written by engineers and (some) improved by intellectual property lawyers. In nearly all cases they have been written with the US jurisdiction in mind. Many of them have been written in the 1990s or early 2000s. 

They do not state any selection of court of legal system. There is no negotiation around them, it's accept or refrain from usage.

License texts approved by the [Open Source Initiative (OSI)]() are considered Open Source today. 

While anyone can draft such a license, 90% of FOSS packages use OSI approved FOSS licenses. There is a minority of crazy cases. 

All of these licenses try to exert a maximum liability limitation and enable at least the [four freedoms]().

See the [legal analysis document][] for a short review.

This chapter has two sections: 

- Effects that arise from **FOSS licenses**. And what is commonly expected to be covered by them. 
- Effects that are not covered by FOSS licenses and common ways of regulating them. This part is called **FOSS Governance**.

## Basic effects and practices: 

- Entities publishing code do so for various reasons and with various expectations. These range from strong commercial motivations to increasing ones reputation to just risk free learning a technical subject in a hands-on way, etc.
- They hope to be able to enforce some of these motivations legally. 
- Other expectations are covered by implicit social code, explicit requests to people and sometimes ...raising shit storms on perceived violations against the perceived violators. This section only aims to cover legal aspects.
- As seen in the [supply chain]() section 100s of packages are part of any application or package. Also, the authors are engineers and thus not legally educated or interested. Due to the counter parties not being known highly standardized licenses (not contracts according to the legal analysis document) are used.
  - Those standard licenses are certified by the OSI. They are not changed or negotiated in use.
  - They are commonly classified into **permissive** (MIT, Apache2), **restrictive** (GPL, MPL, ...) and arguably *"crazy"* (WTFPL).
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

## Sources of legal impact from the licenses

### Liability
Upon publishing of source code we will apply a FOSS license. 
It is the nature of software (and of course everything else that contains software), especially software that can be accessed in an unfinished state, that it will contain lots of defects and may lead to ugly losses and damages if people deploy it. 
We need to know how to best limit our liability using the FOSS licenses and appropriate marking of source code to ensure the licenses we choose to apply are as effective possible towards our goals.

The same goes for outgoing contributions - the patches we provide could lead to defects in the package accepting them. If that package is used by others these defects could cause damages/harm to them.
We can not apply or choose a FOSS license of our choice upon outgoing contributions. 
We need to know how our liability upon contribution looks like and how we can best limit it. (Or from which actions to refrain as the liability can not be limited enough.)

### Warranty
We consume code, are subject to losses or damage due to a bug in the package we consume.
Can we claim damages against the authors? Two cases come up:

- We have a support contract with them, e.g. Red Hat Enterprise Linux
- We don't, i.e. we just downloaded source code or a binary from the internet and deployed it.

This effectively is the inverse of the Liability situation illustrated above.

### Legal use of open source packages

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

### Software patents and trademarks
Some software implemented innovations can be patented. According to the [legal analysis document]() Denmark does not do software patents but the exist in reality nevertheless.

Some licenses have certain aspects of patent protection or terminate on patents claims. 
An evaluation of the risks and chances here, especially given novel and innovative material being developed by us, is strongly advised. It might be desirable to ensure that certain common material is not patented to remain accessible by all interested parties.

The same goes with foreign trademarks or trademarked material embedded by us. We need to either remove any such material to prevent abuse or atain knowledge around boundaries here.
Some licenses contain certain trademark provisions. If used, evaluating their effects under Danish law would be interesting. (ASF 2?)

### IP ownership, coherent IP ownership (DCO, CLA, CAA)

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


## What to expect from a license and what not - FOSS Governance

Based on their nature what can be achieved with FOSS licenses is rather limited. As the [legal analysis document]() states, FOSS licenses are licenses, not contracts under Danish law.

Also, some parts are likely nothing that should be regulated legally but with tacit rules, i.e. a "social contract" (of course, such expectations can be put into writing and could even be taken into account on legal discussions). 

Additionally, since the text of the existing OSI accepted FOSS licenses may not be changed (or else they loose acceptance and ability to be digitally controlled in a feasible way), remaining parts are expected to be stated as "social contract".

This field is what's known as FOSS governance. 

### What you can't prevent

Something that crucially part of Open Source is the ability for people to take your work, duplicate it entirely and try to start a new community from it. This is called "forking". 
Here's when this happens:
- It often happens when someone is unhappy about governance or direction of the package. If they can make their place more attractive than yours, most people will move to place their contributions there and even deploy their fork and not yours. In that case you move from publisher to consumer of what you started. (Or end up continuing your work for yourself, without help or interest from others.)
- The same can happen if a publishers stops working on their package, it becomes "abandoned". Another party takes it over and continues work, people move there.
Sometimes forks briefly exist and then converge to the original project again, or there is a back and forth between forks. However, sometimes forks deviate completely from the project they originated from.

If you choose a permissive license:
- People could start a commercial business based on your code and sell binaries made from your code without returning anything. They might also try to put you out of business or leach from your innovation. (A legal question would be to see how far the permissive licenses are enforceable and such a case would be allowed. My unlegal observation: As long as proper attribution is given this appears to be accepted.)  

In general, diplomacy and awareness and understanding of "competitors" is a valuable skill to deal with these effects before they turn sour. Sometimes it can't be prevented, so keep that in mind before to have the required aces up your sleeve to prevent commercial damage. Aces could be non-publication of certain aspects of a product, choice of license, use of CLA for certain parts, etc.  

### What common FOSS governance questions are

#### "Running the show" or getting write access.
Open Source actively asks for contributions and work across corporate boundaries. 
Thus, a common question is what happens if an external party to the original publisher contributes/engages so much that one could consider them as "running the show" (with the original publisher). 

This is considered the funnel from user to contributor to trusted committer or maintainer. The latter two have write access to the packages which is generally considered to be "they run the show".

With write access they can decide what source code contributions get added to the source code and what don't. They will have to justify that decision with the people making these contributions or else risk loss of contributors or even users. 

#### Product development, roadmap - having a say on the future.

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

#### Technical tools for product choices
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


## FOSS licenses work on code, Creative Common work on data.

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