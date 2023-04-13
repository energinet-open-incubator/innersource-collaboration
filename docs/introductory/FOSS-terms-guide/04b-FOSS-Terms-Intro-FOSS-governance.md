# FOSS Governance: What to expect from a license and what not

What can be achieved with FOSS licenses is rather limited in the broader scope of interactions around Open Source Code. As the [DAP] (section 4.2ff) states, FOSS licenses are licenses, not contracts under Danish law.

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

A recommendation is to keep it pragmatic, simple and short and always offer an easy way to contact the package owners (Maintainers/[Trusted Committer]s) for questions.

## Ownership and Responsibilities
When starting an open source project, it's important to understand that building a community around it is crucial for its success. As a company, you have certain responsibilities to ensure that your project not only gains traction but also thrives in the long run. Here are some of the key responsibilities you need to take:

- **Identify who's responsible for maintaining the project after launch, and how you'll share those tasks with your community**
      As your project grows, your community may need more than just code from you. Responding to issues and discussions, reviewing code, and evangelizing your project are all important tasks in an open source project. Your project should have sufficient internal resources to address and handle external inputs and contributions.
- **Allocate dedicated resources such as budget or staffing for promoting, operating and maintaining the project**
    Open source projects require a considerable investment of resources, including personnel, infrastructure, and funding. 
    As your community grows, managing community interactions becomes increasingly important. Ensure that someone is responsible for responding to issues and reviewing and merging pull requests. This person should be committed to helping maintain a positive and productive community around your project.
- **Involve frequent contributors, even if they're not employed by your company, in key aspects of the project**
  - Building a thriving open source community requires active engagement and contributions from people who are passionate about your project. By involving frequent contributors, even those who are not employed by your company, you can leverage their expertise and commitment to help drive the project forward.
- **Choose the right open source license and seek legal advice to avoid legal repercussions.**
  - Choosing the right open source license is critical to ensure that others can use, copy, modify, and contribute back to your project without repercussions. It also protects you from unpleasant legal situations. Seek legal advice to ensure that the chosen license aligns with your goals for the project.
- **Create a marketing plan for announcing and promoting the project.**
  - Announcing and promoting your open source project is essential to attracting contributors and building a community around it. A well-crafted marketing plan can help you get the word out and attract people who are interested in contributing to your project.

## Shared Ownership of a FOSS Project in a Partnership 
When several companies partner up on an open source project, there are several considerations that need to be taken into account to ensure smooth collaboration and alignment. Here are some important factors to keep in mind:

- **Define project goals and vision**: It's essential for all participating companies to agree on the project goals, vision, and roadmap before starting the collaboration. This helps to ensure that all parties have a shared understanding of the project's objectives, and can work towards a common goal.
- **Establish clear roles and responsibilities**: Establishing clear roles and responsibilities is critical for the success of the project. Each company should have clearly defined roles and responsibilities, with each party accountable for their respective areas of expertise.
- **Determine governance and decision-making processes**: To ensure effective collaboration, the project needs a clear governance model and decision-making processes. All participating companies should have an equal say in the project's governance, with clear processes for making decisions, resolving conflicts, and addressing issues that arise during the project.
- **Agree on intellectual property rights**: Intellectual property rights are an important consideration for any open source project. All participating companies need to agree on how to handle intellectual property rights, such as copyrights and patents, to avoid any potential legal disputes in the future.
- **Establish communication and collaboration channels**: Effective communication and collaboration channels are essential for the success of an open source project involving multiple companies. The project team should establish clear communication and collaboration channels, such as regular meetings, shared documentation, and a dedicated project management tool.
- **Align on technology stack and development processes**: It's important to align on the technology stack and development processes from the outset of the project. This helps to ensure that all companies are working with compatible technologies and development processes, reducing the risk of integration issues down the line.
- **Establish project milestones and timelines**: Finally, all participating companies should agree on project milestones and timelines. This helps to ensure that everyone is working towards the same goals and that the project stays on track. Regular check-ins and reviews can help to monitor progress and ensure that the project is moving forward as planned.

## Defining Roles and Access Rights
Defining a number of roles and their responsibilities and accesses can contribute to creating a transparent governanve on a FOSS project. 

- **User/Consumer**: A person who uses the FOSS source code provided in the FOSS project, but who does not actively contribute to it. The person is interested in the FOSS software being maintained, and may potentially participate in discussions and/or open calls on the FOSS project, and subscribe to mailing lists. 
- **Contributor**: A person who contributes to the FOSS project in the form of either, e.g., code, documentation or issues. The person has read access and can submit pull requests, issues and discussion posts, but does not have write access directly to the code and files contained in the FOSS project.
- **Internal Collaborator**: A person who is employed in a founding company/original publisher and has allocated ressources to contribute to the FOSS project. The person may, besides contributing asynchronously in the FOSS environment, be involved in a number of closed, synchronous sessions as well. The internal collaborator has read access and can submit pull requests.
- **Maintainer/Trusted Committer**: A person who has write access and is responsible for ensuring product quality, reducing barriers to making contributions, and by the [InnerSource Commons definition] also keeping the community healthy. This person can both be an employee from the original publisher or be an outside contributor, who has contributed so much, that they are granted with write access as well (see the section below). 
- **Community Manager**: A person acting in bigger FOSS projects, employed at the founding company, who is responsible for marketing and advocating for the FOSS porject, engaging different stakeholders and ensuring good developer relations. The person might also simultaneously be a Trusted Committer. 
- **Owner**: A person who has write access and determines which functionalities can be accepted as a contribution. The owner is responsible for defining and prioritizing requirements and stories for the community to implement, and interacts with Trusted Committers to make sure that a requested or contributed feature actually belongs to the product. In smaller projects, the Trusted Committer and the Owner is the same person. 


### Becoming a Trusted Committer

Open Source actively asks for contributions and work across corporate boundaries. 
Thus, a common question is what happens if an external party to the original publisher contributes/engages so much that one could consider them as "running the show" (in collaboration with the original publisher). At some point, the original publisher must consider whether it makes sense to grant the contributor write access, and hence making them a [Trusted Committer]. 

This is considered the funnel from user to [Contributor] to [Trusted Committer]. The latter has write access to the packages which is generally considered to be "they run the show".

**With write access they can decide which source code contributions get added to the source code and which don't.** They will have to justify that decision with the people making these contributions or else risk loss of contributors or even users. 

### Product development, roadmap - having a say on the future.

A [Trusted Committer] or maintainer is a mix of product manager/owner, technical lead,  engineering manager and general cat herder or secretary.
As mentioned they accept or deny contributions. Also, they bring the package forward in general. This is especially important if there's additional developers in the same company as the Trusted Committer. Having a roadmap or definition of the future, e.g. a vision and some principles facilitates such decisions and explanation of them to others greatly.

If there is more than one Trusted Committer, there needs to be a way to agree upon what gets accepted, what the future and road map looks like. This can range from very ad-hoc to full corporate board style. It can change and needs to be decided per package based on what fits by the trusted committers (and the corporations behind them if there are any).

If there are multiple coherent packages that make up a FOSS product, a product definition and associated strategy helps to inform decisions what contribution and what code part goes into which package.

Each package can have different governance approaches.

#### Clear expectation setting or: Preventing glass ceilings

Imagine you have a product you published as FOSS where **you want to have the full control of the future and be able to change direction quickly in radical ways** without having to align with others from outside your company. This might be case if you attempt to build a commercial offering from it (see GitLab etc.).
You might not be interested in having trusted committers from outside of your company, but be very interested in contributions as they might help you fix bugs or bring in good new ideas.

In such cases it is on you to make this clear to everyone upfront or else people might invest significant effort only to hit a "glass ceiling" at some point. This might lead to loosing them or even them forking your package - while they have very high knowledge and engagement in your product making success of the fork more likely

Imagine you are interested in **projecting an image of maximum vendor independence, trust and acceptance** - in such cases it might be desirable to have trusted committers from all major contributing entities. At the same time, in such cases reviews and acceptance decisions need to be a lot more rigid to ensure quality and actual independence. 

The [SFOSC](https://sfosc.org/docs/business-models/) offers some pre-packaged, "standardized" examples of how such governance structures can look like under various conditions. They can be taken as inspiration but should not be copied verbatim.

Any governance can evolve over time. Thus, if there are multiple Trusted Committers involved having a way to agreeably enable such an evolution is important.

<!-- Anchorlink style -->
[FOSS Strategy Guide]: https://github.com/project-origin/origin-collaboration/blob/main/docs/additional_reading/07-FOSS-Terms-Intro-FOSS-strategy.md
[EnerginetFOSS-memo]: https://github.com/project-origin/origin-collaboration/blob/main/docs/additional_reading/legal_memo/minutes_legal_notes_on_energinets_use_of_open_source.pdf
[Trusted Committer]: https://github.com/project-origin/origin-collaboration/blob/main/docs/introductory/innersource-short-role-descriptions.md#the-trusted-committer
[Contributor]: https://github.com/project-origin/origin-collaboration/blob/main/docs/introductory/innersource-short-role-descriptions.md#the-contributor
[DAP]: https://www.digitaliser.dk/resource/451301/artefact/retligeforholdvedopensource.pdf?artefact=true&PID=464845
[InnerSource Commons definition]:  https://github.com/project-origin/origin-collaboration/blob/main/docs/introductory/innersource-short-role-descriptions.md#the-trusted-committer
