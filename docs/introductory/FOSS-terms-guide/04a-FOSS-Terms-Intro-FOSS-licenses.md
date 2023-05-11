# "FOSS Licenses": Law (intellectual property law) as a technical tool

As explained in [chapter two: 3 modes of FOSS](03-FOSS-Terms-Intro-3modes-of-FOSS.md) a FOSS package has a FOSS license put on it. 

These are standardized English language license texts written by engineers and (some) improved by intellectual property lawyers. In nearly all cases they have been written with the US jurisdiction in mind. 

Many of them have been written in the 1990s or early 2000s. This leads to terms and mechanisms used being written with 90s or 2000s technology in mind. This results in some challenges to interpretation of those terms with "modern" technlogy, such as clouds or APIs.

They do not state any selection of court of legal system. 

There is no negotiation around them, it's accept the terms or refrain from usage.

License texts approved by the [Open Source Initiative (OSI)](https://opensource.org/licenses) are considered Open Source today. 

While anyone can draft such a license, 90% of FOSS packages use OSI approved FOSS licenses. There is a minority of crazy cases. 

All of these licenses try to exert a maximum liability limitation and enable at least the [four freedoms](https://fsfe.org).

1. Freedom to use it 
2. Freedom to study it (i.e. see, analyze and learn from the source code)
3. Freedom to modify it
4. Freedom to copy and distribute it in modifed or unmodified versions 

**Section 4ff and 2.1.2ff of the [DAP] is especially relevant here.

According to the [DAP] (4.2ff), licenses appear to be one-sided dealings imposed as condition by the intellectual property owner as opposed to contracts where a mutual agreement to a two-sided exchange to benefits and obligations happens.   

This chapter has two sections: 

- Effects that arise from **FOSS licenses**. And what is commonly expected to be covered by them. This is covered in this document. 
- Effects that are not covered by FOSS licenses and common ways of regulating them. This part is called [**FOSS Governance**](04b-FOSS-Terms-Intro-FOSS-governance.md).

## FOSS licenses: Basic effects and practices

Entities publishing code do so for various reasons and with various expectations. These range from strong commercial motivations to increasing ones reputation to just learning a technical subject in a hands-on way, etc.

The creators of the opened source code hope to be able to enforce some of expectations arising from these motivations legally should someone violate them. 

Other parts of these expectations are covered 

- by implicit social code inherent to the FOSS domain, 
- explicit requests to people (often in documents accompanying the source code) 
- and sometimes ...raising shit storms on perceived violations against the perceived violators. 

This section only aims to cover challenges arising from the legal aspects. The [next section](04b-FOSS-Terms-Intro-FOSS-governance.md) addresses some of the social expectations as listed above.  

### Licenses as tools and automation

As seen in the [supply chain section](02-FOSS-Terms-Intro-Common-Terms.md) 100s of packages are part of any application or package. Also, the authors are usually engineers and thus not legally educated or interested. 

- Engineers see the licenses as tool and seek to apply them in a standardized way that does not require involvement of a lawyer before integrating a new package.
- Due to the enormous amount of licenses involved (see the dependency tree sizes above) it is common to apply automated extraction and consolidation of applicable license text to any application being built. 
  - There are some efforts to enable automated checking for license condition adherence. They are not perfect but can remove the most repetitive work.
  -  Automation and "lawyer-free application" would likely not be possible without the use of standardized unchanged licenses.


### Classification: Restrictive vs. Permissive

The OSI accepted licenses are commonly classified into **permissive** (MIT, Apache2, BSD, ...), **restrictive** (GPL, MPL, ...) and arguably *"crazy"* (WTFPL, ...) (although the crazy ones might not be directly recognized by the OSI).

The classification is made based on the effects they trigger and the initial motivation by the authors.

**Permissive** intends to ensure **reputation** of the source code's authors. 

- It's comparable to academic motivation from publication in journals. ("Academic" has been a previous name of that class.)  
- A tacit assumption is that "the authors have a good salary, so they don't need to care about monetizing this source code".

**Restrictive** intends to ensure continued evolution of the source code by ensuring modifications/improvements are not kept by the modifying parties.

- Here, a comparison would be a cooperative or shared public good that should remain a shared public good and may not be monopolized by any party.
- Usually the tacit assumption is that "the authors need to make a living providing service & support around this." or "this is strongly noncommercial in a 'by the people, for the people, away with the evil corporate/government overlords!' sentiment" and any attempt to commercialize is strongly frowned upon.
- Of course, furthering the authors reputation is included here too.
- The elements of the license intended to ensure the return of any modification to the original package are called "**Copy*left***-Clause" (as a pun on Copy*right*) (See also the DAP 1.1.4ff, 2.1.3ff).
- The most **famous example** is **Linux**. 

**Crazy**: Engineers were fed up by legalese and drafted contracts to mock the concept of contracts.

- The [WTFPL](https://en.wikipedia.org/wiki/WTFPL) is the best example. 
- Others tried to [introduce "good" and "evil" as legal concepts](https://heathermeeker.com/2019/11/09/good-and-not-evil-the-advent-of-ethos-licensing/) and prohibit the use for "evil".
- Those licenses end up on reputable packages and then have to be dealt with too. 
  - A common opinion heard here is that they would be either permissive, public domain or "we don't know, don't integrate this".
  - "don't integrate this" is probably a reasonable course of action.

Every now and then licenses appear on source code that claims to be FOSS but whose licenses are **not certified by the OSI**.

- Those often have more similarities with custom contracts or commercial software licenses, like the MS EULA.
- Often they include draconian conditions that go further than the most restrictive FOSS license.
- Some consider them the [**"Source available" class**](https://en.wikipedia.org/wiki/Source-available_software). It's like a museum or show room: Viewing permitted, touching prohibited.  
  - Example:  [ElasticSearch turned SSPL](https://opensource.org/sspl-not-open-source)  

- As a general sentiment: **If it's not OSI certified, don't use it** or do a full legal review.

### Shared common expectations and historical artifacts.

All licenses try to exclude liability for the authors of the source code as much as possible. According to the DAP this has limited effectivity in Denmark, see section 4.3ff, 2.1.6ff.

Also, all require active acknowledgement of the use and the license used. See DAP 2.1.5, 2.1.4.

Some try to protect against software patents, try to protect trademarks (or brands or the publishers reputation, etc. See MPL, Apache for an example) that might be covered in the code or surrounding material. (See DAP 2.2.1 for the GPL example)

Usually they are intended to terminate on violation of the conditions. Some allow for reinstatement of the license (e.g. MPL, see DAP 2.2.9), some don't. If you don't have a license you must not use or distribute the source code.
- Some contain historical feuds leading to intended inability to be combined with others (Apache vs. GPL2) based on automatic termination of combination.

Some have an **"update clause".** Some license texts have versions (GPL2, GPL3, ...), some contain language where the intent was to "switch" to a newer version upon release of a new version of the license. (GPLv2+, see DAP 2.2.2).

- The newer versions can have more or less drastic differences to the old ones. This can trigger some legal uncertainty.

Often, the conditions depend on technicalities, thus technical interpretation and a legal-technical collaboration is important here. Specialized FOSS lawyers are used to this. 

- A classic example is the term "derived work" - when is a work by one author a derivation of the work of another author upon combination of the two?   Often this was argued on grounds of linking, compilation and different ways of combination into one or multiple binaries from the source code. (See DAP footnotes 20 and 9. )  

There are some books on this for German and English interpretations for common scenarios, I know of none for the Danish system. The DAP provides a hint to two books for Denmark and is a great resource in itself, however not able or intended to replace detailed legal consultation.

- Denmark: Possibly [IT-Retten](https://bibliotek.dk/da/work/870970-basis%3A26085950)
  - Denmark: See also the literature appendix of the DAP.

- US law: [Open Source for business](https://www.amazon.com/dp/B086G6XDM1)
- German law:  [Jäger / Metzger](https://www.beck-shop.de/jaeger-metzger-open-source-software/product/26549144)

## FOSS licenses: Sources of legal impact from the licenses

### Liability
Upon publishing of source code we will apply a FOSS license. 
It is the nature of software (and of course everything else that contains software), especially software that can be accessed in an unfinished state, that it will contain lots of defects and may lead to ugly losses and damages if people deploy it. 
We need to know how to best limit our liability using the FOSS licenses and appropriate marking of source code to ensure the licenses we choose to apply are as effective possible towards our goals.

The same goes for [outgoing contributions](03-FOSS-Terms-Intro-3modes-of-FOSS.md) - the patches we provide could lead to defects in the package accepting them. If that package is used by others these defects could cause damages/harm to them.
We can not apply or choose a FOSS license of our choice upon outgoing contributions. 
We need to know how our liability upon contribution looks like and how we can best limit it. (Or from which actions to refrain as the liability can not be limited enough.)

### Warranty
We consume code, are subject to losses or damage due to a bug in the package we consume.
Can we claim damages against the authors? Two cases come up:

- We have a support contract with them, e.g. Red Hat Enterprise Linux
- We don't, i.e. we just downloaded source code or a binary from the internet and deployed it.

This effectively is the inverse of the Liability situation illustrated above.

The common "social contract" expectation here is that we vet and validate FOSS software before introducing it to our area of influence. And don't use it if  does not fit our purpose or quality expectations but don't blindly use and then try to sue.

The second "social contract" expectation is that we report all real defects (especially those that could impact others) in a qualified way to the packages author. 

### FOSS compliance: Ensuring legal consumption of open source packages

As illustrated above, the FOSS licenses are conditional. 

Thus, to be able to publish or consume legal software (and not illegally distribute foreign intellectual property) we need to abide by those conditions.

To abide by those conditions, we need 

1. to know what packages we employ and 
2. what conditions from 
3. which packages we need to abide by. 

There is software generating such lists. Since the licenses are standardized, the set of conditions is manageable, even if 100s of individual packages are involved. A common example of such software is the [OSS review toolkit](https://github.com/oss-review-toolkit/ort) (FOSS itself) or Whitesource (commercial).   

A common condition is to attribute the authors on a finished product in a certain way (often found in permissive licenses). Another common conditions is to provide changes or source code (restrictive licenses).

<!-- insert image of third party notices here or link to Posteo attribution page -->

Some conditions might be unacceptable to us.

In some cases combination of certain packages based on their licenses may be impossible. (The licenses conditions' are mutually exclusive). We may need to clear certain cases of this. 

The FOSS licenses often provide proposals how they would like to see those conditions filled. There is common, technical trade customs to fulfill the conditions. 

We will need to clear with legal if the trade customs legally fulfill the conditions under Danish law. We might need to find the smallest possible fulfilling execution in certain cases. 

Often the conditions to fulfill differ between cases where source code (e.g. a FOSS package we publish in source code) is distributed or binary code (e.g. we release an application or web service in binary/executable form) is distributed.

A short illustration what distribution is and what it isn't is given in the DAP section 1.2ff. Many conditions only apply upon distribution. Thus, without distribution often lesser work ensues.

This process is called **FOSS compliance.** See also [responsibilities and expectations](05-FOSS-Terms-Intro-responsibilities-and-expectations.md) for this. 

We will need to address this based on a legal risk estimation based on legal reality and current legislation around intellectual property law in Denmark as this the evolution towards here is usually an ongoing process.

### Software patents and trademarks
Some software implemented innovations can be patented. According to the [EnerginetFOSS-memo] (Section 1.3.2ff) Denmark does not do software patents but the exist in reality nevertheless.

Some licenses have certain aspects of patent protection or terminate on patents claims. (e.g. GPL class, DAP Section 2.2.1, 2.2.2ff )
An evaluation of the risks and chances here, especially given novel and innovative material being developed by us, is strongly advised. It might be desirable to ensure that certain common material is not patented to remain accessible by all interested parties.

The same goes with foreign trademarks or trademarked material embedded by us. We need to either remove any such material to prevent abuse or atain knowledge around boundaries here.
Some licenses contain certain trademark provisions. If used, evaluating their effects under Danish law would be interesting.

### IP ownership, coherent IP ownership (DCO, CLA, CAA)

We saw that a OSS package is a work of multiple authors from multiple entities. They will have multiple goals, goals that might evolve to be mutually exclusive or hard to combine.

Also, people might violate the boundaries of use that was intended by the original group authors or tacitly accepted by other people that contributed to it later on. Examples of **Violations** could be

- selling as commercial software for a lot of money what was supposed to not be sold, especially not without providing the source code (variations on restrictive licenses).
- abusing trademarks or affiliations like "Endorsed by Energinet" where that might not be the case. Distribution of our FOSS published software with malicious code that is then attributed to Energinet. (Something the ASF tries to prevent, see also the DAP section 3.3ff)
- Claiming software patents against the publishers (there a termination-on-patent-enforcement clause in some FOSS licenses)
- Not giving us the due credit or claiming our work as their own work. (Classic FOSS compliance enforcement example)
- People contributing code to our packages they do not have the legal rights to contribute, resulting in an undistributable / illegal package for us. 

Enforcement might require ability to speak for all authors. Or it might not. See also DAP section 1.2.4. The ASF tries to enable defending patent, trademark and compliance violations on behalf of the authors by requiring sign-off of a special document prior to contributing, the [ASF Contributor License Agreement (CLA)](https://www.apache.org/licenses/contributor-agreements.html). 

Another case, called **"dual-licensing"** common with commercial/profit-oriented publishers (e.g. GitLab, MySQL), would be to have the ability to offer a product based on FOSS source code with a "normal" full commercial contract and a (usually very restrictive) FOSS license. Thus, commercial entitites can choose to abide by the strong restrictive rules or buy the commercial license to e.g. be free to embed the product into a commercial offering (as much as the contract allows that).

For this, they also need the ability to license, sublicense, relicense, etc. all of the source code as they see fit. This is usually also done by requiring sign-off of a special contract (**CLA**) requesting these rights from contributors or even requiring sign-over of the Intellectual Property (IP) to the other entity in a Copyright Assignment Agreement (**CAA**). 

Usually, FOSS packages requiring a CLA or even CAA see significant a drop in contributions due to the additional red-tape involved. Often trying to get a corporate entity to sign such a CLA takes long, hence delaying contributions significantly. 

Depending on the desired outcome, it might make sense to use such a contract when publishing FOSS packages ourselves.

#### Technical tools to enforce product strategy choices - and why they're less powerful than you think.
This deals with strategically using certain FOSS license features hoping to achieve certain effects.
It also points out why usually none of these short circuit argumentations have the effect they're chosen for unless there is proper product definition, strategy and at least some minimal definition around governance. 
All of the below is **strictly not legal advice but *"FOSS license folklore"***, may not work under Danish law and should be closely discussed with specialized legal counsel to evaluate if they actually work in the desired way. 

##### AGPL (network copyleft)
You publish code, offer a Software as a Service (SaaS) product based on it and don't want others to also offer a SaaS product just adding minor changes: This was the design principle of the AGPL. 
It was killed by hyperscalers through hosting the unmodified FOSS products. This lead to radical source-available/non-OSI certified licenses such as the [ElasticSearch turned SSPL](https://opensource.org/sspl-not-open-source) case. Tread very carefully here. 

##### GPL (strong copyleft)
You want to force others to publish the modifications they made? This is what the GPL/restrictive class was designed for. 

However, you'll need to 

1. Find changes, 

2. They actually need to publish them or, if they do not, you need to prove that they have some and don't publish them and then have to sue them based on this and win. The latter takes very long and is rather costly.

The extent to which this is possible may differ based on legal system court and case details. Again: There's a lot of good will and diplomacy involved in FOSS. Try to prevent having to enforce things. And have a watertight case and rocksolid FOSS compliance if you do.

##### Trademarks and patents
You need to ensure certain patent and trademark issues: Certain licenses contain language to protect what you have here. 
Another approach would be to remove any trademark, visual IP etc. from what you publish preventing obvious, easy abuse in the first place. See also the DAP 3.3.1.f

Unfortunately, this also applies if code you published (or otherwise created and use) implements an idea patented by others. Software patents are an ugly minefield. Discuss any patent related questions and challenges with a specialized legal counsel before its too late.

There are "non-aggression pacts" reciprocally pledging each others patents to prevent law suits such as the [OIN](https://openinventionnetwork.com/). Joining them might be a course of action worth evaluating. 

##### Being nasty - CDDL etc. 
You want to prevent your source code/package from being combined with certain other source code? There are certain incompatibilities built into certain licenses. A famous example being GPL and CDDL, very similar in concept but uncombinable. 
Made to prevent inclusion of Sun/Oracle property (ZFS) into the Linux kernel. Has been circumvented in various technical and legal(ly accepted) ways these days. (As in: The author is not aware of any successful law suits against it and e.g. Canonical (behind Ubuntu Linux) distributes a combination of Linux and ZFS for a longer period of time.) 
Try to avoid this if possible at all.

##### Permissive licenses
You want to enable maximum adoption without any care of what happens to what you created, some liabilty protection as long as you are attributed properly.
Unfortunately "without any care" includes code being commercialized resulting in a competitor arising from this, code being used against you, code being integrated into ethically questionable endeavors, etc. 
This is the raison d'etre of the permissive licenses such as MIT or BSD.
Be very careful about actually achievable liability limitations and whether those licenses are actually possible given your dependency tree. And have a good product definition.

##### Public domain
If your legal system provides this: Public domain. You negate that you even created this, you don't want attribution, it's just out there. Use at your own risk. 

## FOSS licenses are for code, Creative Commons are for data.

What you can do with source code, you can do with data.
Data might be other text (like this one here), images, raw material for images (e.g. design templates), or raw data such as an energy system forecasting data (e.g. Excel/CSV files to train AIs with it).

There are similar standardized  licenses for this, with one of the most popular being the [Creative Commons licenses](https://creativecommons.org/about/cclicenses/). 
All legal effects listed above apply here as well. A detailed legal evaluation is required here if they are supposed to be used. The [EnerginetFOSS-memo] does not write about the creative commons.
The licenses also have shorthands indicating the template that is used.

Common variations are (abbreviated according to the website, see the full license texts for the legal details. Contact a specialized legal counsel to see into actual enforceability, details or other related issues): 
- Do you want to prevent changed versions from being distributed: ND attribute
- Do you want to prevent commercial use: NC attribute
- Do you want to enforce changes being published under the same license: SA attribute
- Attribution is always required with the following attribute: BY

The Creative Commons steering body provides [further documentation for these variations](https://creativecommons.org/licenses/?lang=en).

<!-- Anchorlink style -->
[FOSS Strategy Guide]: https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/additional_reading/07-FOSS-Terms-Intro-FOSS-strategy.md
[EnerginetFOSS-memo]: https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/additional_reading/legal_memo/minutes_legal_notes_on_energinets_use_of_open_source.pdf
[DAP]: https://www.digitaliser.dk/resource/451301/artefact/retligeforholdvedopensource.pdf?artefact=true&PID=464845
