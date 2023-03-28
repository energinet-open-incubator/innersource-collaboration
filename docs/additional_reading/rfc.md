# Request for Comments (RFC)

## Table of Contents

1. [Introduction](#introduction)
2. [Context](#context)
3. [RFCs in Open Source](#rfcs-in-open-source)
4. [How can RFCs be Useful for Us?](#how-can-rfcs-be-useful-for-us)
5. [RFCs as Idea Proposals](#rfcs-as-idea-proposals)
6. [RFCs as Decision Logs](#rfcs-as-decision-logs)

## Introduction

Requests for Comment (RFCs) are written, informal pieces of information. They can be assigned with a revision number, status, and/or category, and provides the basis of discussions and decisions on the topic of the RFC. 

<img src="https://github.com/project-origin/origin-collaboration/blob/main/docs/figures/RFC.png" width="60%"/>

## Context

The concept of RFCs is not new. 
They were invented in 1969 by Steve Crocker, with the intent to produce temporary, informal memos on internet protocols, without making official decisions or asserting authority, but rather to encourage others to contribute.  

RFCs are probably best known historically from their use by IETF to create internet standards. 
However, RFCs don't always become standards - They can be informational, experimental etc.  

## RFCs in Open Source 

RFCs are used widely in open source projects. 
One example is [Rust](https://github.com/GuillaumeGomez/rfcs), whose approach have inspired many. They use "lightweight RFCs" to achieve consensus on designs of substantial changes. 
They provide a guide (the README you arrive at, when following the previous link), that explains when and how an RFC must to be filled out in their project.

They are also popular in [Energy Track and Trace (ETT)](https://github.com/Energy-Track-and-Trace), which is a project Energinet is part of, to propose bigger, business-oriented ideas in a structured, documented way.  

## How can RFCs be Useful for Us? 

RFCs can have multiple different purposes in a project, but the concept of an RFC is in itself useful, as it creates a traceable, documented record of information. 
Hence, if you decide to actively use RFCs in your project, they can help create transparency around decisions made.   

  
## RFCs as Idea Proposals 

If you decide to use RFCs to propose new ideas, you can set up some additional attributes to make them useful in your project:  

- If assigned with a status, RFCs can be used in product governance, in terms of classifying the RFCs from, e.g., `proposal` to `accepted` or `declined`. 
- It can be used to develop an idea from concept to a well-defined, implementable feature, by allowing participants to discuss the idea, and collaborate on refining it. 
    - If going with this use-case, the RFC can at the same time function as a first draft to new documentation of the feature being implemented. 

## RFCs as Decision Logs 

It is very likely that some of the project decisions are made in meetings. In such case, RFCs can additionally act as decision logs, by recording the decision in a document and assigning it with an `accepted` (or `proposed` if not fully decided) status. Doing so will serve two purposes: 

- Create an opportunity to allow decisions to evolve in the Open Source community   
- Act as documentation of decisions made, such that everyone who didn't participate in the given meeting is informed. 

  
You can learn more about using RFCs in projects from this [InnerSource Commons RFC Pattern](https://patterns.innersourcecommons.org/p/transparent-cross-team-decision-making-using-rfcs) and from the [Youtube video about how BBC iPlayer and Sounds uses RFCs](https://www.youtube.com/watch?v=U6zlghE0HcE). 
