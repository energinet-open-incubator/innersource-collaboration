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


