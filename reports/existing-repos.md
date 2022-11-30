# Analysis of current content of project-origin GitHub organization repos

## Usage instructions

This is the result of a short, non-in-depth analysis of the repos in the aforementioned GitHub organization based on the view of a bystander who has not been involved in past of current efforts around this GitHub organization at the time of writing. 

Hence, the content is not complete, all-encompassing or final. It may help in the housekeeping process though.

Please make sure to discuss the results with people involved in the respective repository as much as they are still available or people that might know more before taking any destructive actions. 



## Analysis regarding the general GitHub organization:

- It appears that **2FA (Two-factor authentication**, i.e. the same as with the MS Teams auth) **is not active**. I recommend to activate it. 
  It'll then require every member to have 2FA active on their account, which they should be accustomed to anyway from other services.
  - This is now tracked as #6.


- Some of the **public repositories appeared to contain rather Energinet specific configuration parts**, i.e. some Azure templates / configs / ...

  - In the case of **public repositories those should ideally be free from non-generic content**. 
    Non-generic here refers to content that is only valuable / required in the context of the originating organization, here: Energinet.

  - While it is certainly possible and possibly not even risky under certain conditions, it does look "untidy" / "people were just throwing things around with a care, without giving others a thought" / "not meant for others yet". We should **aim to clean things up the more we're looking for outside recognition**. 

  - **Risks** may arise in such cases from potentially **confidential information being included by accident**, such as keys, infrastructure knowledge, etc. **Extra care should be given to avoiding specifically this**.
    - There is a class of tools one can try for that purpose, results are mixed and most likely not complete, but likely better than nothing. Ideally this is supported to some degree by the IT sec people.


- As a possibly **desirable target state**: 

  - If one wants to include configuration etc., those parts should be as generic as possible and well documented, i.e. doing expectation management and making it clear that it' s meant for others to use with some clear value being provided. 

  - In another case a clear "it's the kitchen sink, don't expect anything" could be used as expectation set. 


Not setting the right expectations might lead to negative reactions from users and thus unpleasant communications.

A good amount of code has been published. 
- GitHub offers - free for public repositories - a function called "**Dependabot**" that **enables automatic dependency update pull requests with security updates** for libraries for some languages. It's usually more useful than harmful and I'd **recommend to activate it for the org and all repositories**. 
- Energinet is a critical infrastructure company and should set a good example of visibly looking to care for IT security topics, especially with Open Source efforts. Also, if possible support from the local IT sec people might be useful/desirable.
- It might also be valuable to **provide a default .gitignore with common names of files containing known to often contain sensitive material** in it to prevent those from being committed.
The mentioned secret scanning tools above are probably also a good idea to get integrated.
- Work towards providing legal safety and knowledge especially given already published repositories.
  - This is now tracked in: #72, tangentially related are: doc material in #94, policy request in #80 


- Marking repositories as "inactive" by marking them as "archived" is a good practice.

### People active in the GitHub-Org:

See into updating the [participants.md](https://github.com/project-origin/origin-collaboration/blob/main/participants.md) with all partipating people and check the repositories and GitHub ACLs for any alignments with a desired state that might be needed or are unexpected.


## Repositories
In none of the following the issue trackers or pull request system was used in any meaningful way. Thus, a most likely complete backup could be created by mirroring the respective repository.

If there is meaningful activity in any of the GitHub parts, moving the repository to a different GitHub organization could also be an option.

### Repositories that are only privately visible and marked as archived are:

- **tobedeleted_dh Last changed: 03/2020** 
  - Possibly review the contents and either mirror&zip, move to another org or just delete this. One could also put it as zz-$theoldname, as GitHub sorts by name by default.
- **tobedeleted_id Last changed: 04/2020** 
  - Same as the last one.
- **backup-tools Last changed: 11/2020** 
  - Appears to be backup tooling for a specific installation - maybe the now public repositories? 
  - What makes it private and archived, but not marked for deletion? Is there some use in it? 

### Repositories that are only privately visible but active, i.e. not archived are:

- **origin-collaboration** 
  - this is our collaboration organization repository.
- **monolith-frontend - last change 21.6.2022**
  - It's an empty repo that only has been populated with an MIT license. 
  - Apparently is the dual for the public monolith repo.
- **demo-repository - last change in 09/2022** 
  - Appears to be a repository for internal GitHub training or to showcase how to use GitHub for others. 
  - Made by Martin Schmidt and Jakob Bork. Can we reuse this as further training material? Could be valuable.

### Repositories that are public

- In general **most repositories here are equipped with a [MIT license](https://en.wikipedia.org/wiki/MIT_License)** **file**, thus making them full open source. 

  - MIT is one of the most permissive licenses there are. There is very little commercial restriction on what anyone may do with what has been published here. They can even recommercialize anything published there with very little constraints.

  - Has there been any acknowledgement of this in a wider group / the business owner of this at the point of publication?
    - #94 builds material to enable understanding and processing of the legal evaluation of the context of such licenses. The evaluation will need to evolve lawyers, possible also IP/IT specialized ones.


- In general there are reasonably large chunks of code published here. 

  - **A scan for secrets etc. as illustrated above should be conducted to see if there's anything public that shouldn't be public**. There's tools and your maybe someone from your IT sec department for this.

  - There is a risk that publication is not possible under the MIT license if certain dependencies are included as there are some combinations of FOSS licensed libraries being used that can not be combined into certain target licenses. This is a topic that can (and possibly should) be discussed with your legal department. 
    - See also #94 for this.

#### Repositories that are public and marked as archived are:

- Most of those have been created by Martin Schmidt and Jakob Kristensen. 
- This appears like a more or less complete set of GitHub projects a in more or less prototypal state. Is this the "old teams project"? 
- Most of it is made with Python and some Javascript.
- The GitHub issue trackers and pull request systems have only been used very little. 



- Two complete Python projects with little information about them but a lot of commits and recent activity. This looks like this might be worth a deeper look as it might have been an important part / often discussed / worked on of the project? 

  - **account-service - last changed: 31.1.2022**

  - **datahub-service - last changed: 3.2.2022**




- Looks like a more or less complete Angular project with front&backend. Question is if this an Angular stub example project or something custom made by us. 
  In the first case: Good that we use the stubs, but do we need to make them public? In the second case: Can we give those projects a better name?
  - **example-frontend - last changed: 28.1.2022** 
    - Quite a few commits there, there are Azure deployment scripts in it - is this non-generic content (see above)?
  - **example-backend - last changed: 29.9.2021** 
    - Belongs to the above? Complete Python project.

- The following repositories looks pretty Energinet specific. Is it generic enough to be valuable to make public? Maybe we should consider taking this private again? Also, the mentioned secrets scanning etc. is recommended.
  - **deployment-scripts - last  changed: 24.9.2021** 
    - Describes a Kubernetes deployment to Azure.
  - **pipeline-templates - last  changed: 24.9.2021** 
    - Describes a good bit of Azure pipelines. There are a lot of commits here. 
    - However, **there's no license on this repo**, i.e. this is proprietary intellectual property that happens to be visible to the public. This looks like a limbo state to me. **Does this need to be public?**



- **hello-world - last changed: 25.1.2021**
  - appears to have represented a SDK meant for others (non-project members) to built on-top of / familiarize themselves with what the project built. 
  - Generally such approaches valuable and should be built well and with decisive user/community focus so they pull people in. 
  - The example website mentioned in the README 404s unfortunately. There is an external contributor with a pull request. **(Great, where did that person come from?)** 
    - It hasn't seen attention unfortunately though. It does not fix the website 404 too, though. This looks slightly abandoned.



- The following are a number of additional Python services - maybe microservices? - only touched in 2020. What made them stop in 2020?
  Also, if this is set public a secret scan should be conducted. It might be valuable to reconsider what parts of this need to be public?
  - **datahub_processor - last changed: 9.9.2020** 
    - How is this related to the datahub-service which has still been changed in 2022?
  - **identity-service - last changed: 11.11.2020** 
    - Complete looking Python project with a good bit of  commits
  - **fake-eloverblik - last changed: 28.10.2020** -> Old, appears to be a complete project, Python, little commits.
  - **ledger-sdk-python - last changed: 9.9.2020** 
    - Complete looking Python project with some commits
  - **energy-type-service - last changed: 8.9.2020** 
    - Complete looking Python project with some commits
  - **swagger-ui - last changed: 25.8.2020** 
  - Is this potentially just a generated output by Swagger for the API provided by the project? 
  - If so, would it possibly be more valuable to add "how to generate" instructions and the original API such that this does not get outdated? And what value for the future is there?
  - **ledger-dto-python - last changed: 7.7.2020** 
    - Complete looking Python project with little commits



#### Repositories that are public are:

All **these repositories are active ambassadors of the project origin** (and thus Energinet) and thus should look and feel as good as possible to trigger adoption and interest. The audience is both a developer (with and without some business inclination) and somewhat technically inclined business audience.
**Highlighted (pinned) is the registry project. Thus, this project should look the most welcoming and self-explanatory as this is the project that will get the most clicks from new observers.**
For all repositories Dependabot and a security scanning tool should be active.

- **.github:** 
  - This sets templates and basic settings for the entire GitHub org. 
  - It might be a good idea to place relevant points to the documentation repo there as this contains a good bit of documentation parts. 
  - It might also be a useful idea to also highlight the documentation repo if the content is still relevant.

- **documentation - last changed: 19.1.2022**: 
  - Points to a deployment that does not appear to exist anymore, i.e. 404s. 
    - This should be addressed. 
    - The TLS certificate of the deployment does not match the URL of the deployment and thus leads to TLs warnings - this should also be fixed. 
    - Alternatively, this should be removed for now as it leaves an abandoned look.
  - The documentation looks useful / like something a user could want to read. 
    - One could also take advantage of the GitHub wiki function to have it rendered pretty or tooling such as a Hugo/readthedocs to have pretty looking static website rendered from it. 

- **registry**
  - A .net project - unlike all the other Python projects.
  - **This is licensed as Apache2, not MIT.** 
    - Has there been a reason for this choice? 
    - Both are valid permissive FOSS licenses, but maybe there's been a reason to choose one the one set of project and the other one for this?
    - The pull request system is used, which is good.
    - Recommendation for future approaches once more public visibility is desired: 
      - @MartinSchmidt and @wisbech are working on this one. There a large, long pull running requests with little comments. 
      - Often it is valuable (and easier) for others to read and to merge to work in smaller pull requests that are merged more often. Those can be thematically coupled by issues etc.
      - This might not be trivial to put into practice, but is a good ideal to strive towards to.
    - How does the registry relate to the other large repo monolith?
- **monolith** **last changed: 21.6.2022**
  - The present README file appears to be aimed at outside contributors - which is nice - however still refers to historic knowledge that those might not have.
  - Python project.
  - How does this relate to the registry repository?
- **location-based-declaration** **last changed: 10.8.2022**
  - Small Python and JS project. 
  - Many contributors and commits but little content and description. This might also be important. 
