## Public Money, Public Code: As a TSO

Here, the [DAP](https://www.digitaliser.dk/resource/451301/artefact/retligeforholdvedopensource.pdf?artefact=true&PID=464845) is a strongly recommended read as well as the [EnerginetFOSS-memo](../../background_material/minutes_legal_notes_on_energinets_use_of_open_source.pdf).

As a publicly owned TSO that runs on public money, we are bound to additional special rules.

Those rules could from concerns of critical infrastructure operation (NIS2 derivatives) or strict regulations on the use of public money or non-competition regulations as public body.     

**Action Points**:

- Any regulation and rules that apply to us here must be analyzed and interpreted in the context of the given FOSS product. See the [EnerginetFOSS-memo](../../background_material/minutes_legal_notes_on_energinets_use_of_open_source.pdf) for a description of non-competition rules.
- One possible interpretation of the non-competition rules is “public money, public code”, which means that Energinet is limited to providing and maintaining a public good that others (e.g., corporate   companies) can offer services around
- It could be reasonable to take measures to ensure that the public good remains a public good and improvements by others are brought back to it. This could (but does not have to) lead to restrictive licenses for certain parts of FOSS packages published by us.
- A strategy or policy must be created to handle these rules. 
- Rules coming from the IT security and NIS2 side might lead to needing special reviews of contributions or using additional tooling to ensure quality and safety of the created product. 
- This might also be a source of liabilities we have against others.

The [open source, open service](#open-source-not-open-service) separation is relevant here, as by this definition, any FOSS source code published by us - even modified by others through contributions - is inert and cannot harm our critical infrastructure. Only when deployed and introduced to the critical parts of our infrastructure damage can occur.

**Action Point**:
- Upon passing the boundary from source code to deployment, additional checks need to be in place. However, this is an Operations and IT security topic, and hence it is not addressed here.
- In the case that another TSO chooses to use deploy our published FOSS package it is their responsibility to ensure that it fits their critical infrastructure security checks.


- [] TODO: Add interpretation and links of boundaries of the  Energinet memo here and clear them with legal
- [] TODO: Add pointers to rules arising from NIS derivatives etc.

## Private Money, Public Code - As a Private Entity

Not all TSOs (or other corporations) act as public bodies. Thus they may have to earn money with open source (e.g. to satisfy profit expectations of their shareholders).

This can lead to desires of monetizing Open Source in various ways. See the [strategy guide](../FOSS-strategy) and the [SFOSC models](https://sfosc.org/docs/business-models/) for information on what interests and approaches might be interesting for them.

As a public body we likely do not need to monetize FOSS. 
However, to further potential adoption of the public good we create, we might want to facilitate certain aspects of monetization in what we publish for other members of our economy. Thus we are "making the cake bigger for everyone".
To further interest in adoption of the public good we create, we might want to enable certain aspects of monetization in what we publish. This can be done by strategically selected governance decisions and matching use of FOSS licenses as well as matching boundary definitions of the FOSS packages and products.

A common monetization would be to enable multiple parties to offer implementation consulting or operation assurance around our packages. However, they must then acquire any necessary knowledge and ability to support and provide assurance. 

**Action Points**:
- We can contribute to this aspect by making our FOSS packages a friendly and cooperative place to collaborate 
- Think about who makes decisions in terms of the roadmap/acceptance of patches (see the [strategy guide](../FOSS-strategy-guide/)  or the [FOSS governance chapter](04b-FOSS-Terms-Intro-FOSS-governance.md)) for considerations of who can become a trusted committer).				 
- Another option is to enable other companies to host our FOSS packages, offering certain services to others in exchange for compensation. 
- Analog example: We develop an email protocol and server application, someone else the actual operation of the software following this standard for money (e.g., Gmail, or  United Internet).

