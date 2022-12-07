## Public Money, Public Code: Doing FOSS as a public body

Here, the DAP is a strongly recommended read as well as the [Energinet regulatory legal memo]().

As a publicly owned TSO that runs on public money, we are bound to additional special rules.

Those rules could from concerns of critical infrastructure operation (NIS2 derivatives) or strict regulations on the use of public money or non-competition regulations as public body.     

We have to interpret the regulations and rules here and for all product informing their strategy, see the [Energinet regulatory legal memo]() for non-competition rules. 

A possible interpretation could be to argue that Energinet is limited to providing and maintaining a public good that others (e.g. Danish companies such as Mjølner et al) could offer services around. 

In such a case it could be reasonable to take measures to ensure that the public good remains a public good and improvements by others are brought back to it. This could (but does not have to) lead to restrictive licenses for certain parts of FOSS packages published by us.

Rules coming from the IT security and NIS2 side could lead a need for special reviews of contributions or general regular reviews/audits or additional tooling to ensure quality and safety of the created product. This might also be a an source of liabilities we have against others.

The source/service separation is to be made here again: FOSS source code published by us and modified by others through contributions is inert and can not harm our critical infrastructure. Only when deployed and introduced to the critical parts of our infrastructure damage can occur. Thus upon passing this boundary additional checks need to be in place. This is an Operations and IT security topic though that is not addressed here.

- Corollary: If another TSO chooses to use deploy our published FOSS package it is their responsibility to ensure that it fits their critical infrastructure security checks.

- [] TODO: Add interpretation and links of boundaries of the  Energinet memo here and clear them with legal
- [] TODO: Add pointers to rules arising from NIS derivatives etc.

## Private Money, Public Code: Doing FOSS as a private entity

Not all TSOs (or other corporations) act as public bodies. Thus they may have to earn money with open source (e.g. to satisfy profit expectations of their shareholders).

This can lead to desires of monetizing Open Source in various ways. See the [strategy guide](../FOSS-strategy) and the SFOSC models for information on what interests and approaches might be interesting for them.

As a public body we likely do not need to monetize FOSS. 

To further interest in adoption of the public good we create, we might want to enable certain aspects of monetization in what we publish. This can be done by strategically selected governance decisions and matching use of FOSS licenses as well as matching boundary definitions of the FOSS packages and products.

In any case, this is an individual discussion that should be discussed individually. 

A common monetization would be to enable multiple parties to offer implementation consulting or operation assurance around our packages. However, they then have to build then necessary knowledge and ability to support and provide assurance. We can make our FOSS packages a friendly and cooperative place to collaborate and think about who decides about the roadmap/acceptance of patches (see above for considerations of who can become a trusted committer) but not much more.

Other options could be - depending on the architecture - to enable other companies to host our FOSS packages, as central instance or decentral instances offering certain services to others in exchange for compensation. Analog example: We develop an email protocol and server application, other operation of the software following this standard for money - think Gmail, United Internet, ... 

