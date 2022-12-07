# Common Terms

Open Source encompasses a **combination of** a cooperative/network-oriented **business strategy/tactics with specific work methods** and approaches.

It is **realized through** uncommon application of (mostly) **intellectual property law** legislation and means of **technical automation**.

Everything is **applied to the field of software creation, modification and maintenance**.

The domain of deployment or application of software is not limited and thus, Open Source can find commercial application also with hardware.

To understand the field, certain technical terms and concepts need to be defined and understood.

Additionally context is provided by acknowledging the historical context explaining the why's of certain decisions and approaches. 

## Historical and political background shaping visible phenomena, goals and  expectations

Open source has been created in a political environment strongly highlighting a non-commercial, liberal and self-sovereign agenda. 

All trade practices, accepted rules, expectations and stewardship of the underlying legal tools is done through independent non-profit bodies largely running on the same agenda mentioned above. 

Today, open source has become a strongly commercially used approach as well. It represents the bedrock of all software engineering today. Even Microsoft strongly participates in non-Microsoft Open Source Software and is very active in publishing their own Open Source Software.

It is recommended to align with the before-mentioned liberal and self-sovereign agenda where possible, as the pool of talents with Open Source skills is s largely powered by the attractiveness of said agenda. Incidentally, this agenda is consistent with the concept of "public money, public code", which is highly applicable to Energinet as a TSO. 

The[Danish digitalization agency paper]() has a short section on this too, see section 1.1.1.
Our["Energinet Open Source as TSO" memo]() also highlights the connection to "public money, public code" in section xyz . <!-- TODO add proper reference here -->   


### Open Source, FOSS, FLOSS
**Open Source Software** is often referred to as **OSS**.
OSS where the authors want to highlight the mentioned political background is called **"Free and Open Source Software" FOSS**.
OSS where the authors don't feel that FOSS sufficiently highlights the political background is called FLOSS. 
In the end, all of it is Open Source Software as illustrated below. They only differ in their strict expectations on how corporate involvement is supposed to look like and the behaviors around such software.

This guide generally uses **FOSS** to refer to software and **Open Source** to the approach to work. 

## Basic technical terms: Source Code, Compilation, Binary Files, Deployment

These are foundational technical terms from the process of software creation. 

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

- Three (strongly simplified) examples: 
  - The [Linux kernel](https://kernel.org) (about 2000-3000 text files in source, about 10 files in binary), 
  - [Numpy]() (a popular package data scientists use, e.g. for grid forecasting models), 
  - Microsoft Word (Tenthousands of source code files noone outside of Microsoft gets to see, 1 file Word.exe plus 100s of support files in binary) 

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

## Real-life software creation today (Supply chain) or: Making money on the shoulders of giants.

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
 

- **Source code and binaries** only cost storage space (think about the cost of a USB stick or memory card) and **are inert**, i.e. especially **not able to process data on their own**.

- **Only once deployed, the code turns into a *service***. 
  - In the case of web application like Google.com, deploying the code to make it a service is also referred to as ***"hosting"***.

A **service** is able to process data, render services to users that can be sold, and thus make money. 

- However, running the service costs money, incurring liabilities to the people whose data is processed. This is usually contractually coupled with service level expectations etc.



***Open Source absolutely exclusively refers to distributing the source code to third parties.*** 

Hence, there is no such thing as "Open Service" in the domain of Open Source. 



## Hosting and "free(mium) services"

- Once a person or company has the source code of an application they can create a service from it.
  - Of course, they can offer the service to the public for free if they choose so. 
  - However, **all of the above liabilities, maintenance effort and all the bills arising from it become problems for the person or company hosting the service**. 
  - The **person(s)/company offering the source code to the public is in no way involved here**.
    - They may even not be alive anymore or remember that they wrote the source code for it. 



- Hosting open source applications and charging money for enabling access to them is one of the main income streams of all cloud providers such as Azure, Google Cloud or Amazon Web Services. 
  - Often they add friendly user interfaces or modify them to be more comfortable or integrate with other commercial offerings they might have.  See [responsibilities and expectations](05-FOSS-Terms-Intro-responsibilities-and-expectations.md) for what follows from this.

- In the **following sections everything only and explicitly talks about Open Source, not any form of deployment or service**.
   - Exceptions are explicitly mentioned. The main exception is **"Operation"**.  
     - Operation refers to Open Source Software that has been turned into a service, standalone or combined with commercial code by Energinet. 
