## Public Money, Public Code: As a TSO

Here, the [DAP](https://www.digitaliser.dk/resource/451301/artefact/retligeforholdvedopensource.pdf?artefact=true&PID=464845) is a strongly recommended read as well as the [EnerginetFOSS-memo](https://github.com/project-origin/origin-collaboration/blob/main/docs/additional_reading/legal_memo/legal_memo_README.md).

As a publicly owned TSO that runs on public money, we are bound to additional special rules.

Those rules could from concerns of critical infrastructure operation (NIS2 derivatives) or strict regulations on the use of public money or non-competition regulations as public body.     

At a first glance, the following sections of the [EnerginetFOSS-memo](https://github.com/project-origin/origin-collaboration/blob/main/docs/additional_reading/legal_memo/legal_memo_README.md) appear to be especially relevant:
(Authors entirely not legally founded opinion, i.e. folklore that we need to get checked.) 

Section 4.2.1: In my interpretation we need to be able to argue the inverse of these things for each product. 
- An interpretation could be "make the cake bigger for everyone". 
  - Publishing a product others can sell services (support, hosting, ...) upon, i.e. creating a new market could - my 2 Øre for it - be one option.
  - We will not act as an active participant of the market, but just provide the good that creates the market. (And maybe some fair rules that no one commercial participant monopolizes the market? Regulated markets should be Energinet's thing I guess... :wink: )  
  - This requires the other parties to be have sufficient knowledge to do the above. 
    - Which they usually end up with if they're actively involved in creating and maintaining the good.
  - A concern regarding "market creation" arises from section 5, paragraph 4-6 (and section 7) in such that they require to check if there is already a market / good that we would displace with our publication before publishing.

- Technically I see that 3.2 applies, but I would argue that 3.2 does not make the crucial Service/Source code separation. Thus leading to an exclusion that possibly does not have to be one.  
- It restricts the fields of application to those listed in 4.1 (Could the outcome of the last bullet point change this?). 

- We can support our claims by arguing that we give back to the public what we made with the public' money (Section 6, paragraph 6,7). (Additional doc relevant [here](https://www.digitaliser.dk/resource/2212763/artefact/OpenSource-softwareidetoffentlige.pdf?artefact=true&PID=2212766))
- Section 6, paragraph 9 argues that participation in existing FOSS has reduced need for checks, as 'there already is FOSS for this in the market'.

Nevertheless - see the action points for needed actions to see if the last paragraph holds and what details pertain to it.


**Action Points**:

- Any regulation and rules that apply to us here must be analyzed and interpreted in the context of the given FOSS product. See the [EnerginetFOSS-memo](https://github.com/project-origin/origin-collaboration/blob/main/docs/additional_reading/legal_memo/legal_memo_README.md) for a description of non-competition rules.
- One possible interpretation of the non-competition rules is “public money, public code”, which means that Energinet is limited to providing and maintaining a public good that others (e.g., corporate   companies) can offer services around
- It could be reasonable to take measures to ensure that the public good remains a public good and improvements by others are brought back to it. This could (but does not have to) lead to restrictive licenses for certain parts of FOSS packages published by us.
- A strategy or policy must be created to handle these rules. 
- Rules coming from the IT security and NIS2 side might lead to needing special reviews of contributions or using additional tooling to ensure quality and safety of the created product. 
- This might also be a source of liabilities we have against others.

The [open source, open service](#open-source-not-open-service) separation is relevant here, as by this definition, any FOSS source code published by us - even modified by others through contributions - is inert and cannot harm our critical infrastructure. Only when deployed and introduced to the critical parts of our infrastructure damage can occur.


**Action Point**:
- Upon passing the boundary from source code to deployment, additional checks need to be in place. However, this is an Operations and IT security topic, and hence it is not addressed here.
- In the case that another TSO chooses to use deploy our published FOSS package it is their responsibility to ensure that it fits their critical infrastructure security checks.


- [] TODO: Clear interpretation of boundaries of the Energinet with legal
- [] TODO: Add pointers to rules arising from NIS derivatives etc.

## Private Money, Public Code - As a Private Entity

Not all TSOs (or other corporations) act as public bodies. Thus they may have to earn money with open source (e.g. to satisfy profit expectations of their shareholders).

This can lead to desires of monetizing Open Source in various ways. See the [strategy guide](https://github.com/project-origin/origin-collaboration/blob/main/docs/additional_reading/07-FOSS-Terms-Intro-FOSS-strategy.md) and the [SFOSC models](https://sfosc.org/docs/business-models/) for information on what interests and approaches might be interesting for them.

As a public body we likely do not need to monetize FOSS. 
However, to further potential adoption of the public good we create, we might want to facilitate certain aspects of monetization in what we publish for other members of our economy. Thus we are "making the cake bigger for everyone".
To further interest in adoption of the public good we create, we might want to enable certain aspects of monetization in what we publish. This can be done by strategically selected governance decisions and matching use of FOSS licenses as well as matching boundary definitions of the FOSS packages and products.

A common monetization would be to enable multiple parties to offer implementation consulting or operation assurance around our packages. However, they must then acquire any necessary knowledge and ability to support and provide assurance. 

**Action Points**:
- We can contribute to this aspect by making our FOSS packages a friendly and cooperative place to collaborate 
- Think about who makes decisions in terms of the roadmap/acceptance of patches (see the [strategy guide](https://github.com/project-origin/origin-collaboration/blob/main/docs/additional_reading/07-FOSS-Terms-Intro-FOSS-strategy.md)  or the [FOSS governance chapter](04b-FOSS-Terms-Intro-FOSS-governance.md)) for considerations of who can become a trusted committer).				 
- Another option is to enable other companies to host our FOSS packages, offering certain services to others in exchange for compensation. 
- Analog example: We develop an email protocol and server application, someone else the actual operation of the software following this standard for money (e.g., Gmail, or  United Internet).

