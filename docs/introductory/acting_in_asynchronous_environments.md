# How to handle asynchronous environments

## Table of Contents

1. [Introduction](#introduction)
2. [Motivation](#motivation)
3. [Communicating Asynchronously](#communicating-asynchronously)
    - [Creating Useful Documentation](#creating-useful-documentation)
4. [Expectable Social Effects](#expectable-social-effects)
    - [Difficult People and Freeloaders](#difficult-people-and-freeloaders)
    - [Cultural Differences and Diplomacy](#cultural-differences-and-diplomacy)
    - [Participant Churn](#participant-churn)
5. [Summary](#summary)

## Introduction

Corporate software development (from ideation to creation of code and final operation of the envisioned solution) usually happens in co-location and with lots of face-to-face communication. Agile is famous to highlight these two aspects.

Sometimes you will work with "externals" (i.e. people you contracted but who're not directly/permanently employed by your company) who still usually are pretty close by, e.g. the next bigger (or smaller) town. You will have countless meetings, some with effect, others with the just the effect of being social glue making certain aspects of the work easier. 

Seldom, or more often if you are part of a multinational corporate, you will work with people in other timezones. Meetings at funny times will be had, lots of mails will be written.  Sometimes funny effects of cross-cultural communication will be experienced. Maybe every once in a while you'll even board a plane and visit each other only to condemn the jetlag for 3 weeks after the meeting. (Sure, beer was absolutely not a factor in play. Of course.)
Still, you can usually build on quite a bit of shared corporate culture and goals that will facilitate collaboration and set some common expectations. 

Imagine that FOSS and Open Source is the continuation of the multinational corporate example ad extremum. But without the binding shared corporate culture and goals. 
(Technically, there is roughly a shared culture of FOSS - it's the historical political underpinnings and customs that arose from this.)
The next part tells a short story to illustrate this a bit more.

## Motivation 
Why are asynchronous environments important in FOSS / Open Source?

Imagine you develop software (or another product) and each of you is on their own island. Also, every communication takes about 12 hours to be transmitted. Usually, you only get low bandwidth channels, so mostly text is transmitted. Sometimes faster, but not really.
You meet once or twice a year for the big congregation. Presentations will be had; beer will be drunk and food will be eaten.

Often random people see your island group and hear that mystical, useful artifacts come from that group of islands.
They'll drop often clueless communication on any of the islands. In it, they're trying to make sense from the communication, stories or other artifact pieces they overheard or found from the island group.

This of course is an exaggeration but nevertheless is pretty close to a lot of what happened in open source. 
These days, some transmit times lowered, there‘s sometimes even more bandwidth (Teams, Zoom). 
The number of islands rose and some of the islands got more crowded, i.e. more than one person is one it (corporations participating in FOSS and thus having a more direct link between people, sometimes even in the same office).

## Communicating Asynchronously
How did people deal with this, what remained and what is expected?

- Everything is text-based. Almost all of the interactions happen in **public channels** (Mailinglists, GitHub issue trackers, Slack, …) **visible to the entire world**, and thus random bystanders too. 
- All of the interactions are **recorded for perpetuity**, are **searchable** and **each** interaction / **message has a permanent, stable link** that allows to link to them from other messages or other formats of interaction.
- If 1:1 interactions, voice or in-person interactions happened, summaries and minutes are provided to the public channels if there was anything of public value in it.

The material arising from this approach is called **passive documentation**.
_Passive_ because it just comes into being en passant while the actual work is being done. 
**Active documentation** would be documentation you write with the intent of being documentation, illustrating bigger picture aspects, specific concise parts, etc. 
You'll need both and each one has their own value but you'll quickly learn the value of passive documentation. You can even link back and forth between both formats.

- Having most of the conversations public requires you to think about what you write or publish. Your developers will be advocates and spokespersons for your company. 
    - They'll need to know what can be disclosed, and what can't. Accept this, empower and train them and you'll get highly valuable skills, maybe even find good developer relations and less challenges in Open Source interactions.

### Creating Useful Documentation 
You, your [Trusted Committer]s and project members' time will be the limiting factor in Open Source projects. 
The more "self-onboarding" capable your documentation/project in itself is and the better your approach to passive documentation is, the less impact on your, your trusted committers' and other project members' time will be. These approaches serve as a multiplicator. In the following, some practical suggestions are provided on how to obtain a useful Open Source documentation:

- Expect that communication turnaround times may take long. Thus, be as explicit and complete as you can in the material you write. This way, less questions arise blocking on communication roundtrip times.
- Imagine a person finding some communication, or a specific message. This information should, with *reasonable* effort, enable the person to onboard themselves and ask (semi-)intelligent questions without having ever spoken to any of your project members. 
    - If you keep getting the same questions, Use FAQ documents/discussion channels (frequently asked questions) or improve other documentation with regards to exactly the questions you're getting.
- Automation keeps everything alive without time investment. Automate as much as you can.
    - This includes quality checks, parts of deployment and reviews. You can also to some degree automate your decision structures or support them with small processes such as checklists everyone can use or workflow automation. 
        - This will also allow you to easier add new [Trusted Committer]s or have someone act in your place if needed (in the case of sickness, different time zones, etc...)
- FOSS is event driven, as is your inbox. You check both regularly (with the intervals being different) and act if there is something to do. Do the same with your Slacks, GitHub inboxes, Miros etc. related to your Open Source project.

Sometimes it can help to state the time zone you‘re in and a rough estimation of how reactions times usually look like so people can adapt their expectations.

## Expectable Social Effects
### Difficult People and Freeloaders

Caveat: Clueless people will come. People that see FOSS as free work that they‘re entitled to and whose authors time they are just as entitled to because they themselves are obviously the center of the universe. General jerks will appear. 
They exist. Ignore those people. 

It is ok for FOSS to require some work from others to make use of it. If you intend to sell things, you‘ll obviously make things a bit more comfortable at some points to lower the barriers of entry. Which is fine and represents marketing. But even then, you‘ll very likely have some expectations from your prospected customers.
It is good practice to try to understand people's problems and help people and help them to help themselves to some degree. They should appear to have invested some reasonable amount of effort though.

### Cultural Differences and Diplomacy

You might hit some cultural differences that look like conflicts. Something that often helps is to take a look and try to understand the context and situation, try to be friendly, as well as explicit and transparent in your expectations and approach as possible and permissible. 
If it helps it helps, if it doesn‘t it doesn‘t. At least you tried, maybe there is something to be learnt from it. Diplomacy also helps.

Summary: Be nice, helpful and reasonable and expect the same. There's enough jerks on the Internet, you don't need to cater to them and you shouldn't become one.

### Participant Churn 

People often stay as long as they need to "scratch their itch", but not longer. If they had a pleasant experience they might return and a fruitful collaboration may begin. You may even find future employees that are already onboarded and capable of dealing with exactly what you need.

Often people come, do something, go away and return a year later. You might do the same. It's exactly what one can expect from Open Source. By having good passive and active documentation, automation and explicitly documented decisions approaches (see above) this intermittent contribution and activity becomes possible and unproblematic. 


## Summary
Compared to software development in a corporate, software development in the FOSS environment is run almost entirely asynchronously. 
Asynchronously here refers to the almost non-existence of face-to-face conversations, colocation, "agile ceremonies" and the frequent presence of large time-zone differences and not knowing the people you are interacting with personally.

Putting some effort into setting up an asynchronous environment can be highly advantageous. If participants in your FOSS project had a pleasant experience, they might return, and a fruitful collaboration may begin. Hence, some time should be invested in making “self-onboarding” easy and comfortable, from using the documentation. 

In an asynchronous environment, information and communication are all text-based, including:
- **Active** documentation (documents written to illustrate bigger picture aspects, specific concise parts, etc.), 
- **Passive** documentation (interactions visible on public channels, and summaries and minutes published from face-to-face interactions deemed to have some public value to them).

By having good passive and active documentation, automation and explicitly documented decisions approaches, intermittent contribution and activity becomes possible and unproblematic.

To obtain a well-functioning asynchronous environment, consider the following summarized points:

- All interactions should be recorded for perpetuity and be searchable. In the tools used, such as Github, Miro, Slack, each interaction / message has a permanent, stable link that allows to link to them from other messages or other formats of interaction. 
- Communication turnaround times take long. Thus, be as explicit and complete as you can in what write. A person finding the communication archives, or a specific message, should, with reasonable effort, be able to onboard themselves and ask (semi-)intelligent questions without having ever spoken to any project member.
- As most conversations are public, your developers will be advocates and spokespersons for your company. They'll need to know what can be disclosed, what can't etc. Accept this, empower and train them in PR and communications topics and you'll get highly valuable skills, maybe even find good developer relations people and less challenges in Open Source interactions. 
- The more „self-onboarding“ capable your documentation/project in itself is and the better your approach to passive documentation is, the less impact on your, your trusted committers' and other project members' time will be.
- It is good practice to try to understand people's problems and help people and help them to help themselves to some degree. They should appear to have invested some reasonable amount of effort though.
- If you keep getting the same questions - Use FAQ documents (frequently asked questions) or improve other documentation with regards to exactly the questions you're getting.
- You might hit some cultural differences that look like conflicts. Try to be friendly, as well as explicit and transparent in your expectations and approach as possible and permissible. 
- Automate as much as you can. This includes quality checks, parts of deployment and reviews that can be automated. You can also to some degree automate your decision structures or support them with small processes such as checklists everyone can use or workflow automation. 
- FOSS is event driven, as is your inbox. You check both regularly (with the intervals being different) and act if there is something to do. Do the same with your Slacks, GitHub inboxes, Miros etc. 

<!-- anchorlink style use -->
[Trusted Committer]: https://github.com/project-origin/origin-collaboration/blob/main/docs/introductory/innersource-short-role-descriptions.md#the-trusted-committer
