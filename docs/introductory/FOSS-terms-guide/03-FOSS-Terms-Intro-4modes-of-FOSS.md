# The Four Modes of Open Source

This chapter provides a description of basic **FOSS domain concepts**. 

It mostly covers ways of **interaction with FOSS**. This interaction deals with the **collaborative modification of source code files in FOSS packages across corporate boundaries**. Exceptions are explicitly marked. 

Collaboration happens with people representing other corporate entities or private citizens.

Interaction with OSS can be separated into **four modes**: participation, consumption, contribution, and leadership.

It is common that people interacting are **not necessarily known by name** (usually just **pseudonym and email address**). They are likely to **only participate** for a brief or undefined period of time **until the goal or benefit they want to achieve for themselves is addressed**.

The resulting product, encompassing all the work from all its participants over time, remains there forever.

**Section 3ff of the [DAP]** addresses these four modes from a high-level legal perspective. Further aspects are addressed in other sections of the paper. 

An important terminology used for **perspective** here is:

- **We/Us**: Person employed by Energinet, person employed at a partner company or bound by a contract to work for Energinet
- **They**: Any other entity. Could, e.g., be: A person representing 50Hz/Elia, Elering, Statnet, an individual. The individual could also be employed by us but participating in their spare time as an individual.

## Orthogonal aspect of FOSS: The Ways of working
(**Note**: A full introductory guide on working in asynchronous environments is available [here](https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/introductory/acting_in_asynchronous_environments.md))

Contributors and authors of packages contributed to may reside in **vastly different time zones**, have significantly **different work times** and especially also may **not have time to address contributions immediately**.
There is **no built-in face-to-face communication** as with common software development, a client-lawyer interaction etc.
This leads to a **highly text-based, asynchronous, very explicit way of working** **emphasizing automation, self-explaining yet highly specialized tools and, well, a lot of text**. The advantage of text-based communication is that it allows easy searching, pin pointing, and commenting/review. (As well as translation in cases of language barriers.)

## Consumption

We take **FOSS source code or FOSS packages** (or binary code created from FOSS source code by us or a third party, e.g. Red Hat) **from a third party** (e.g. Linux, Kubernetes, Tomcat, ...) and:

- either add it into source code we create as part of a commercial product. We then compile the combined work, turning it into a binary and deploy this combined work. 
- take the pre-existing binary (Red Hat Enterprise Linux) or code and deploy it to render a service for us (e.g. a web server to host a web site)
- take the FOSS source code, modify it, compile and deploy the modified result to render a service for us. (e.g. Wordpress Blog with a Energinet theme)

The **resulting service can be created for pure internal use by us or it could be created to be accessible by us and third parties**. 

**Each third party FOSS package has one of the OSI certified licenses associated with it**. It is referred to as an ***incoming license***. The set of all licenses found in all packages is called the **set of incoming licenses**.

Often different packages use the same FOSS license. In a work with 500 third party FOSS packages in the dependency tree there will often only be a set of incoming licenses with 50 different incoming licenses.

([DAP] 3.2ff) 

## Participation
Additional to consuming FOSS, participation includes engagement in the Open Source community by attending conferences, mailing lists, news and updates, etc., to stay informed about software development on the consumed FOSS components. 



## Contribution
Any cross-entity collaboration resulting in changes to the source code files exchanged are called **contributions**. The person providing the changes is usually called ***contributor***. 

### Outgoing Contributions
When we consume code, the following journey to a contribution to other projects can happen:
- We find ***bugs*** (technical reasons for malfunctions in the program) while doing so, 
- fix them (change a few lines of text) and don't want to have to apply those changes to the foreign source code forever if the publisher updates their source code. 
- Hence, we offer the changes representing the fix (called a ***patch or diff*** - it's a redline effectively) to the original author of the source code from whom we took the code (or usually entire package) we consume.

This can also happen with **patches that not only fix a defect but add new functionality**. If the functionality fits their road map, is well crafted and they think they will be beneficial to all future users, i.e. is not just highly specific to us and our needs, they are likely to accept them.  

### Incoming Contributions

Incoming contributions are when we get contributions to source code package we have published. Basically, the "Outgoing Contributions" process happens, just with the roles of us and them reversed.

It is generally considered a sign of success of a published package to get incoming contributions. It will probably only happen after quite some marketing, raising popularity and resulting success, though.  

### Downstream and Upstream
There are two commonly used terms in the participation process that describe the positions.

- **Upstream**: is the "original work" / most authoritative source of the work
- **Downstream**: A derivation / modification of upstream / the "original work"
-  **Example:** In the *outgoing contribution process*, we are in the downstream position, fix a bug there and and try to **bring it upstream**, i.e. to the FOSS package we have used. Often "**upstreaming** a fix / feature / ..." is heard too.
  - In the incoming contribution process, the roles are reversed   

## Leadership

**We create source code with the intent to publish it to the world for use by them**. Usually **we continue to use this source code to consume it ourselves** too.

**We mark the source code files with a FOSS license and additional information** with the intent **to define** our liabilities against third parties, set expectations **what we expect others to do and not do with our published source code**. We assume that the FOSS license will make some of these expectations enforceable.

The **FOSS license we mark our source code with is called the *outgoing license***.

Usually such a publication happens by means of publication on a website like GitHub. 

**Once published, our ongoing work on this source code happens visible to the world** and we now interact with third parties regarding questions or requests for participation (see below).

This gives the world maximum transparency to each and every aspect of development around the package published.

Since the third parties are not bound to us contractually and thus may have different objectives, **we need to make sure that we carefully review what they offer and what we push to the outside** and see into any different objectives they may have and how those fit ours.  

([DAP] 3.3ff)



<!-- Anchorlink style -->
[FOSS Strategy Guide]: https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/additional_reading/07-FOSS-Terms-Intro-FOSS-strategy.md
[EnerginetFOSS-memo]: https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/additional_reading/legal_memo/minutes_legal_notes_on_energinets_use_of_open_source.pdf
[DAP]: https://www.digitaliser.dk/resource/451301/artefact/retligeforholdvedopensource.pdf?artefact=true&PID=464845
