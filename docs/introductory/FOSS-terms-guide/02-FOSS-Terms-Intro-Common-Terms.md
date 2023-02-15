# Common Terms

Open Source encompasses a **combination of** a cooperative/network-oriented **business strategy/tactics with specific work methods** and approaches.

It is **realized through** uncommon application of (mostly) **intellectual property law** legislation and means of **technical automation**.

Everything is **applied to the field of software creation, modification and maintenance**.

The domain of deployment or application of software is not limited and thus, Open Source can find commercial application also with hardware.

To understand the field, certain technical terms and concepts need to be defined and understood.

Additionally context is provided by acknowledging the historical context explaining the why's of certain decisions and approaches. 

## Historical Background

Open source has been created in a political environment strongly highlighting a non-commercial, liberal and self-sovereign agenda. 

All trade practices, accepted rules, expectations and stewardship of the underlying legal tools is done through independent non-profit bodies largely running on the same agenda mentioned above. 

Today, open source has become a strongly commercially used approach as well. It represents the bedrock of all software engineering today. Even Microsoft strongly participates in non-Microsoft Open Source Software and is very active in publishing their own Open Source Software.

It is recommended to align with the before-mentioned liberal and self-sovereign agenda where possible, as the pool of talents with Open Source skills is s largely powered by the attractiveness of said agenda. Incidentally, this agenda is consistent with the concept of "public money, public code", which is highly applicable to Energinet as a TSO. 

The [DAP]((https://www.digitaliser.dk/resource/451301/artefact/retligeforholdvedopensource.pdf?artefact=true&PID=464845)) document has a short section on this too, see section 1.1.1.
Our ["EnerginetFOSS-memo](https://github.com/project-origin/origin-collaboration/blob/main/docs/additional_reading/legal_memo/legal_memo_README.md) document also highlights the connection to "public money, public code" in [section 06 "FOSS and the public sector / TSOs"](06-FOSS-Terms-Intro-public-sector-specialties.md). 


### Open Source, FOSS, FLOSS
**Open Source Software** is often referred to as **OSS**.
OSS where the authors want to highlight the mentioned political background is called **"Free and Open Source Software" FOSS**.
OSS where the authors don't feel that FOSS sufficiently highlights the political background is called FLOSS. 
In the end, all of it is Open Source Software as illustrated below. They only differ in their strict expectations on how corporate involvement is supposed to look like and the behaviors around such software.

This guide generally uses **FOSS** to refer to software and **Open Source** to the approach to work. 

### InnerSource

The next chapter will address practical domain terms of FOSS. 
It will, among other things, declare that FOSS consists of a **specific way of working**.
Also, it will state that **collaboration across corporate entities** (or individuals and corporate entitites) is defining for FOSS. 
 
There is a derivative of FOSS, growing in popularity the last few years. It is called **InnerSource**, sometimes also written as Inner Source. 

#### How does InnerSource differ from Open Source and where does it overlap?

InnerSource refers to the **use of FOSS (Open Source) ways of working inside the boundaries of one corporate**, e.g. just between Energinet employees.
The "cross entity collaboration" here refers to collaboration between e.g. teams in different business units but still the same corporation.

What is common to be shared? 
 - Work on a library that everyone uses, e.g. a design system.
 - Work on a common analytics library, a common build support functions package used by e.g. DevOps people across multiple projects.

**How are things often shared?**
 - Team A (called a **"Guest Team"**) found a bug or found a feature that they think could be beneficial for everyone using Team B's (called the **"Host Team"**) product/library etc.
 - Team B declared that they are open to contributions from others.
 - Team A now either directly creates a pull request (in the case of a small bug fix) or briefly informs Team B about their plans to contribute something and they discuss if its fits and how it's best done.
 - Team A builds the changes and pull requests it to Team B's project. A knowledgeable person from Team B reviews the changes and mentors the person from Team A for any needed changes they should make such that the change fits well into Team B's product. Team A makes said changes until it's good to be included.  Once that's done, Team B includes ("merges") the changes Team A made into their product.
 - It is common to have someone from Team A answer to all questions around the new change for 30 days. (Called "30 days of warranty") to ensure a smooth handover. After 30 days, the change is maintained by Team B as if they had made it.
 - Everyone won. Ideally more people than just the ones involved got a bug fixed or a feature added that is beneficial for them, less wasteful planning and silo-jumping/escalation was needed, some communication bridges (direct relations between people) have been established or improved, etc.

**How can I plan this in my Agile?**
 - Software developers' time is often highly utilized. It is a belief often seen that only a coding developer is a good developer.
 - Wouldn't this interruption from the outside or communication stuff reduce their coding time and thus make things less effective?
 - As it turned out: This is actually not very likely.
 - Since you would have to do the work yourself anyway (if its fixing a bug at your side instead, or building a work around, or escalating to another team, etc.). So you would plan the work anyway. 
 - What you do now, is that you include the work of contributing elsewhere and doing work that benefits you, however "lives" in another product/team just like you would plan work that you're doing in your product/team.
 - To handle incoming requests (after all, other people fixing your bugs still benefits you - the same goes with features being added for you) you just plan them the same way. Also, it has turned out to often be beneficial to leave a certain amount of slack in the planning to enable developers to handle open unplannable work (known unknowns).

In InnerSource the entire time, no code leaves the corporate boundaries. Nothing is published to the outside world. 
You can, of course, decide that you want to turn something that lived as a dedicated InnerSource product/library so far as Open Source. That is a different effort and change of modalities though.

In an ideal case, developers and non-developers can learn a good part of the ways of working of FOSS in a safe way (without the risks from publication and potentially hostile outside people) through InnerSource experience.

The rest of this guide deals with FOSS / OpenSource, i.e. the non-inside corporate boundary only application. 
If you want to learn more about InnerSource and its ways of working, see [this guide](https://innersourcecommons.org/learningpath) for more.

## Fundamental Technical Terms

These are foundational technical terms from the process of software creation. A good understanding of these terms will be highly valuable for decision-making in terms of licensing, strategy and governance, described in the later sections.  

Software creation refers to everything in the realization of a digital asset such as a smartphone app or piece of hardware like a thermostat once a set of features realizable by software engineers has been defined. 

### Source Code or "Code"

This term refers to plain text files containing programming language text in a strictly human readable format. 
  - These files can be **compared to "Blue prints"** for mechanical engineering.

- Common "languages" are C#, Java, Javascript, Python, C, Go etc.

- A **small piece of software can easily consist of thousands of such text files**.

- These are **written by programmers**.

### Binary files or "binary", "binary code", "executable"

**Non-human/computer readable files** that contain data that can be read and used by a computer. The source code is translated to a binary file by a **compiler**, which transforms the source code to commands that can be executed directly by the computer.
  - A computer loads and executes the binaries, thus enabling the computer to run Word.exe, Google.com, a thermostat, a car, an app, etc.
  - Usually, binary files can only be used by the specific computer architecture they were meant for. A computer architecture is a specific design of the electrical computer system inside the computer, comparable to the difference between a motor that runs on diesel, gasoline or is electrical. Examples of different computer architectures are x86 (Laptops) and ARM (Smartphones, Macs).

- It could be argued that a modern website also is mostly binary code due to the excessive amount of interactive features included in modern websites.

### Compilation

- A **process that transforms source code text files into one or more binary files**. 

Compilation is required every time the source code has changed, to apply the changes made.
    - (Thus: A new deployment is required to put changes in the source code in production, see below.) 

With source code the "executing/building of the functionalities" written in the source code, is called compilation. 
  - The program used for compilation is called a **"Compiler"**.
  - The compiler **translates and combines all required source code (text) files** **to** **"build"** the program, i.e. **transform it into binary format**.
  - The **result may be one more or binary files**. Sometimes, multiple binary files are combined into one, sometimes multiple binary files are the final result.

- Sometimes, the compiler adds additional text files that were not directly supplied by programmers as source code.

### Packages

- This term is **applicable to both binary files and source code**.

- A **package is a set of** either text/source code (or binary) **files** that are **required to provide a specific feature**.
  - The set may also contain only one file.

- A package **has one or many associated owners** and - given sufficient originality - **is a work of art eligible to intellectual property protection**. 

- A **FOSS package** is a package, just that all of its contents are FOSS. 

- Three (strongly simplified) examples: 
  - The [Linux kernel](https://kernel.org) (about 2000-3000 text files in source, about 10 files in binary) (*A FOSS package*)
  - [Numpy](https://numpy.org/) (a popular package data scientists use, e.g. for grid forecasting models) (*A FOSS package*)
  - Microsoft Word (Tenthousands of source code files noone outside of Microsoft gets to see, 1 file Word.exe plus 100s of support files in binary) (Very much *not a FOSS package*) 

### Deployment

Describes the **transformation from source code to something rendering practical service to a human being**.

- **Requires** the **compilation** step.
- The **resulting binary files are then deployed**.
- The **result of the deployment is a service**.

The **programmers' main source code** (all required packages) are **combined with external packages, compiled and further packaged** (currently very popular: "Docker containers"), **copied to a target computer and then started**. 

**Critical difference:** 

- **Only from here, ongoing cost for machines is incurred and data is processed**.
- Any step beforehand causes negligible storage costs and minuscule computation costs. 

Examples:

- Word. IT copied it to your laptop and you run it there
- A smartphone app: Same, you download and run this on your smartphone
- A thermostat: Assembled by manufacturer, they copy it the device, once powered up it runs the final binary package
- A website/Google.com: Complicated packaging/assembly process, resulting packages copied to multiple computers in a Google datacenter, Google copies a package (the website you see) to your computer (in the browser, e.g. Edge/Chromium/Firefox) once you invoke Google.com, you run the website, website and Google servcers communicate, you get the information you want.
- A car: A datacenter on wheels, effectively all of the above.

## Dependencies

- In the 1980s and partially in the 1990s a program and function for a computer of material value could have been created from scratch by a limited number of engineers.

- Today, **most software engineering assembles enormous amounts of packages made by foreign parties and adds their own specific innovation on top** of this. 
  - Commonly the **relation between foreign source code and original, new source code is from 70 to 95% foreign to original** source code. 


- This also goes for packages that are added, i.e. those packages also contain enormous amounts of foreign packages.

- Such **"foreign code" / "foreign packages" are called *dependencies***. The **dependencies of dependencies are called *"transitive dependencies"***. 
  - The **entire list of dependencies down through all transitive dependencies** is called the ***"dependency tree"***.

- Very **small common software today** (small websites, demonstrators, reusable visual components for a website) have a **dependency tree consisting of 200-500 packages**.



- Packages can be 
  - purchased from manufacturers (commercial off-the-shelf software, e.g. Word, SAP, a specialized forecasting library), 
  - custom created (by your own engineers, by externally contracted engineers) or 
  - procured as open source - meaning: an engineer downloads them from the Internet and combines them into their work.



# Open Source, not Open Service
There exists an erroneous confusion of the two terms **Open Source** and **Open Service**. However, there is a crucial difference between them.


- **Source code and binaries** only cost storage space (and thus are almost free of monetary cost - think "cost of a usb stick"). They are **inert** and hence not able to process data on their own.

- Once the source code is deployed, it turns into a ***service***. 
  - In the case of web application like Google.com, deploying the code to a service is also referred to as ***"hosting"***.

A **service** is able to process data, render services to users that can be sold, and thus a company can make money from it. 

- However, running the service costs money, incurring liabilities to the people whose data is processed. This is usually contractually coupled with service level expectations etc.



***Open Source absolutely exclusively refers to distributing the source code to third parties.*** 

Hence, there is no such thing as "Open Service" in the domain of Open Source. 







- Hosting open source applications and charging money for enabling access to them is one of the main income streams of all cloud providers such as Azure, Google Cloud or Amazon Web Services. 
  - Often they add friendly user interfaces or modify them to be more comfortable or integrate with other commercial offerings they might have.  See [responsibilities and expectations](05-FOSS-Terms-Intro-responsibilities-and-expectations.md) for what follows from this.

- In the **following sections everything only and explicitly talks about Open Source, not any form of deployment or service**.
   - Exceptions are explicitly mentioned. The main exception is **"Operation"**.  
     - Operation refers to Open Source Software that has been turned into a service, standalone or combined with commercial code by Energinet. 
