# Mythbusting a few common Open Source myths.

## Table of Contents
1. [Introduction](#introduction)
2. [FOSS is not secure](#foss-is-not-secure)
3. [FOSS is secure](#foss-is-secure)
4. [Open Source is "free as in beer"](#open-source-is-free-as-in-beer)
5. [You need to be in a foundation](#you-need-to-be-in-a-foundation)
6. [Build it and they will come](#build-it-and-they-will-come)
7. [You're done when you published something](#youre-done-when-you-published-something)


##  Introduction

There is a lot of talk in the street about what open source is or isn't, what it can do or can't do. Also, expectedly, some stories of silver bullets fly around.

Some of them have a kernel of truth, some of them are pure :cow2:  :poop: and some are truer than others. 
This document briefly presents and discusses a few common ones.



## FOSS is not secure
One concern within this topic is: _What happens if there are malicious actors keeping bugs for themselves to use them against you?_

To mitigate any risks in this aspect, you can create a company-wide open source policy, providing guidelines for, e.g., licensing, security measures, liabilities in the case of external contributions in open source projects owned by the company.
Train people who are in contact with Open Source on the topics of this policy, and ideally support them with tooling. It is too much to tackle without good tooling.  
<br/><br/>
Another often encountered concern within this topic is: _I cannot be sure that the FOSS components I use are safe to use_.

If you are using FOSS, you are using something that someone put on the street with a big warranty disclaimer. It might be good, it might be bad. 

You vet and control what you use yourself. Invest in the usual [Software Bill of Materials (SBOM)/Software Component Analysis (SCA) tooling](https://wiki.owasp.org/images/b/bd/Software_Composition_Analysis_OWASP_Stammtisch_-_Stanislav_Sivak.pdf) so you know what you're using. However, note that SCA is a larger topic in itself as it is the technical manifestation of multiple fields. 
To handle the resulting dependencies well, it is necessary to address each dependency individually, assessing its implications for you and your project when using it. 

Other practical actions to take in order to mitigate risks here are:
- Have an active ear on the projects mailing lists and in the communities whose products you use.  	
- Invest time in obtaining **open source sustainability**. Move away from a component if it does not fit with your policies anymore. 
    - If you really need it, you can take over the component if you have the resources.
    - Alternatively you have to reengineer to another component.

Some relevant links in the topic of Open Source/FOSS sustainability are: 
- [Article from Forbes](https://www.forbes.com/sites/forbesbusinesscouncil/2022/03/11/open-source-how-the-sector-has-changed/),
- [Blogpost from Pension Bee](https://www.pensionbee.com/blog/2022/august/open-source-software-sustainability-problems)
- [Article from OpenSource.com](https://opensource.com/article/22/11/sustainability-open-source)
- [Article from Project Management Planet](https://www.projectmanagementplanet.com/five-key-insights-for-open-source-projects-sustainability/). 
- [Blogpost from Human Who Codes](https://humanwhocodes.com/blog/2022/06/sponsoring-dependencies-open-source-sustainability/) 

## FOSS is secure

An often encountered myth is that FOSS is more secure than other software components. There is a [Linus Law](https://en.wikipedia.org/wiki/Linus%27s_law) stating that: 

 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "_With enough eyes, all bugs are shallow_".
<br/><br/>
But what if everyone mutually relies on the eyes of the others being there while not doing anything themselves? The law inverts.  


## Open Source is "free as in beer"
Another common myth is: _There are no strings attached, it‘s just sharing code. Is there really a community?_

Regarding legal ramifications (see the [FOSS Terms guide](https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/introductory/FOSS-terms-guide/01-FOSS-Terms-Intro-TOC.md): You don't want to pay up to 250k€ per case and deal with negative PR. Also, there are non-profit enforcement bodies with hefty endowments.) these additional aspects should be considered:

- If you mindlessly consume whatever is out there you are binding your business to the will of whoever made what you're using. You will not have any say in what ways they chose or if they just abandon their component without a word (they do, frequently so, sometimes even [destructively nuking it before leaving](https://www.theverge.com/2022/1/9/22874949/developer-corrupts-open-source-libraries-projects-affected)).
- Get involved with the people of the components that are critical to you and you can have more of a say or at least know earlier when it is time to move.
  - You'll find out that there's a lot of smaller or some bigger, more often than not friendly communities. And of course – commercial suppliers playing open source. You will know how to handle those. Sometimes even with those nice non-paid cooperative options exist.

## You need to be in a foundation

An often heard myth is: _All open source is owned by a foundation. Hence, you need to be in a foundation_.

In short, a lot of FOSS components you use are made by individuals, small teams or even corporates. It's often not a bad idea to use such components too, even if they are not owned by a foundation. However: Know what you're using. See the [FOSS is not secure](foss-is-not-secure) section above for more details on this. 

Foundations (non-profit corporate entities made to legally own and defend the FOSS intellectual property (IP) others gave them to steward) exist. In case of the [Apache Software Foundation](https://www.apache.org/) or [Eclipse foundation](https://www.eclipse.org/) they provide a vendor neutral home for a lot of IP. You can donate money to them. It's not the worst idea for a good number of cases. However, Reducing FOSS sustainability to sponsoring a (random) foundation is not a useful approach. 
  	
- If you play a "standards setting" game, at a later evolution stage moving to a foundation can be a good idea to signal vendor-independence and have some IP questions handled properly.  	

## Build it and they will come

Without marketing (business and developer focused, depending on the evolution stage and desired people) and product/market fit, they won't. Or only very late and very little.

- Marketing to developers and business people is critically different. Take care!
- This doesn't have to be a problem if your strategy, or the rationale for the funds you invested in bringing a FOSS work to the public, does not rely upon maximum adoption and receiving contributions but, e.g., employer branding or fulfilling the publication desires of your employees so they remain your employees. Short: Think about what you want to achieve and what follows from this.

## You're done when you published something

You are absolutely not. It's only the beginning of your public Open Source journey. You now get to apply all the skills you learned before.


<!-- Anchorlink style -->
[FOSS Terms Guide]: https://github.com/energinet-open-incubator/origin-collaboration/blob/main/docs/introductory/FOSS-terms-guide/01-FOSS-Terms-Intro-TOC.md

