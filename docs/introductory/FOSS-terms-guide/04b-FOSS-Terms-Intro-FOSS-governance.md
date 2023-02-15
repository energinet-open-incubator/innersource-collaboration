# FOSS Governance: What to expect from a license and what not

What can be achieved with FOSS licenses is rather limited in the broader scope of interactions around Open Source Code. As the DAP (section 4.2ff) states, FOSS licenses are licenses, not contracts under Danish law.

Also, some parts are likely nothing that should be regulated legally but with tacit rules, i.e. a "social contract" (of course, such expectations can and often should be put into writing and could even be taken into account on legal discussions). 

Additionally, since the text of the existing OSI accepted FOSS licenses may not be changed (or else they loose acceptance and ability to be digitally controlled in a feasible way), the remaining parts are expected to be stated as "social contract".

A **social contract** is, much like the social contract of a society, accepted without explicit signature by the participants of a community (a special FOSS package or FOSS at large for more abstracts principles) upon engaging with this community.

Every participant accepts its restrictions even if they restrict some of their abilities to make a profit, behave in a certain way, etc.  

This field is what's known as **FOSS governance** or *"what do I want others to do and not do with the code that I put out there"*. 

## What you can't prevent

Something that is crucially part of Open Source is the **ability for people to take your work, duplicate it entirely and try to start a new community from it**. This is **called "forking"**. 
Here's when this usually happens:

- It often happens when **someone is unhappy about governance or direction** of the FOSS package. If they can make their place more attractive than yours, most people will move to place their contributions there and even deploy their fork and not yours. In that case you move from publisher to consumer of what you started. (Or end up continuing your work for yourself, without help or interest from others. Often with limited success.)
  - A variation of this is upstream trying to "suddenly" chance licenses or commercialize what hasn't been commercialized. (See Oracle, ElasticSearch, ...)
    - Another variation is someone trying to be "smart" and "take someone elses FOSS private and sell it" - often this ends up as a low success FOSS enforcement case.
    - In most Oracle cases the original upstream still exists but plays absolutely no role whatsoever anymore. 

  - Another variation is unexpected commercial or privacy damaging behavior of a FOSS package that was expected to be purely "uncommercial". This leads to the FLOSS purists creating a "pure, clean, FLOSS fork". They are usually not very popular. 
    - Don't do anything that could be considered privacy invasive. The usual FOSS demography ([see historical background](02-FOSS-Terms-Intro-Common-Terms.md)) is very sensitive here and there are enough people equipped with skill, funds, time and will to litigate and campaign for such a reason.  

- The same can happen if a publisher stops working on their package. It becomes **"abandoned"**. Another party takes it over and continues work on their fork, people move there. 
  - Sometimes access to the original package is explicitly handed over by the original authors who step down to the new stewards of that package. This is by far not the norm though.

Sometimes forks briefly exist and then converge to the original project again, or there is a back and forth between forks. However, sometimes forks deviate completely from the project they originated from.

If you choose a permissive license:

- People could start a commercial business based on your code and sell binaries made from your code without returning anything. They might also try to put you out of business or leach from your innovation. (A legal question would be to see how far the permissive licenses are enforceable and such a case would be allowed. A very much not legally-founded observation of common practice: As long as proper attribution is given this appears to be accepted.)  

In general, **diplomacy, awareness and understanding of "competitors" is a valuable skill to deal with these effects before they turn sour**. Sometimes it can't be prevented, so keep that in mind before to have the required aces up your sleeve to prevent commercial damage. Aces could be non-publication of certain aspects of a product, choice of license, use of CLA for certain parts, etc.  

## What you can try to control: Common FOSS governance questions

As stated above: Governance is a "social contract". The FOSS way of doing this is to write brief documents stating and explaining decision around the questions below, as well as e.g. what is expected from people offering contributions.

Depending on the size of the FOSS package and the number of involved people, this can range from a short 20 lines document to an elaborated process with all sorts of bells and whistles. 

A recommendation is to keep it pragmatic, simple and short and always offer an easy way to contact the package owners [(maintainers / trusted committers)](https://github.com/project-origin/origin-collaboration/blob/main/guides/innersource-short-role-descriptions.md) for questions.

### "Running the show", getting write access or "how to become a maintainer".

Open Source actively asks for contributions and work across corporate boundaries. 
Thus, a common question is what happens if an external party to the original publisher contributes/engages so much that one could consider them as "running the show" (with the original publisher). 

This is considered the **funnel from user to [contributor to *trusted committer*](https://github.com/project-origin/origin-collaboration/blob/main/guides/innersource-short-role-descriptions.md) or *maintainer***. The latter two have write access to the packages which is generally considered to be "they run the show".

**With write access they can decide which source code contributions get added to the source code and which don't.** They will have to justify that decision with the people making these contributions or else risk loss of contributors or even users. 

### Product development, roadmap - having a say on the future.

A trusted committer or maintainer is a mix of product manager/owner, technical lead,  engineering manager and general cat herder or secretary.
As mentioned they accept or deny contributions. Also, they bring the package forward in general. This is especially important if there's additional developers in the same company as the trusted committer. Having a roadmap or definition of the future, e.g. a vision and some principles facilitates such decisions and explanation of them to others greatly.
If there is more than one trusted committer, there needs to be a way to agree upon what gets accepted, what the future and road map looks like. This can range from very ad-hoc to full corporate board style. It can change and needs to be decided per package based on what fits by the trusted committers (and the corporations behind them if there are any).

If there are multiple coherent packages that make up a FOSS product, a product definition and associated strategy helps to inform decisions what contribution and what code part goes into which package.
Each package can have different governance approaches.

#### Clear expectation setting or: Preventing glass ceilings

Imagine you have a product you published as FOSS where **you want to have the full control of the future and be able to change direction quickly in radical ways** without having to align with others from outside your company. This might be case if you attempt to build a commercial offering from it (see GitLab etc.).
You might not be interested in having trusted committers from outside of your company, but be very interested in contributions as they might help you fix bugs or bring in good new ideas.

In such cases it is on you to make this clear to everyone upfront or else people might invest significant effort only to hit a "glass ceiling" at some point. This might lead to loosing them or even them forking your package - while they have very high knowledge and engagement in your product making success of the fork more likely

Imagine you are interested in **projecting an image of maximum vendor independence, trust and acceptance** - in such cases it might be desirable to have trusted committers from all major contributing entities. At the same time, in such cases reviews and acceptance decisions need to be a lot more rigid to ensure quality and actual independence. 

The [SFOSC](https://sfosc.org/docs/business-models/) offers some pre-packaged, "standardized" examples of how such governance structures can look like under various conditions. They can be taken as inspiration but should not be copied verbatim.

Any governance can evolve over time. Thus, if there are multiple trusted committers involved having a way to agreeably enable such an evolution is important.