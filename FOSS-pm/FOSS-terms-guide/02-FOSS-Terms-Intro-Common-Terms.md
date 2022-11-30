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


