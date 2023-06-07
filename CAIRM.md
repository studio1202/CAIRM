
# CAIRM PROJECT CHARTER (DRAFT)

## EXECUTIVE SUMMARY

This paper proposes a new collaborative regulatory process called CAIRM (Collaborative Agile Intuitive Regulation Management). CAIRM is specifically aimed at helping regulate new complex, rapidly evolving, pervasive and disruptive fields like that of Artificial Intelligence (AI). "Cairm" is an old Irish word meaning "where" and it is here intended as "where [we want to go]".

CAIRM is based on the premise that most voters are not familiar with the regulated technology or its implications, and they are not willing to devote much time to the regulatory process. CAIRM is therefore structured to be simple for voters, while at the same time providing to more engaged actors the power of a Risk Management system with added flexibility and reusability. CAIRM is also reusable and expandable with minimal effort.

Within CAIRM all heavy lifting is delegated to field subject matter experts and volunteers, empowered by a dedicated software framework and Large Language Model (LLM) AI systems. It is they who build the framework and draft regulations. Voters can instead freely choose their desired level of commitment: committed voters can participate in discussions; proficient, less committed voters can directly vote on regulations; non-proficient voters can instead either delegate their vote or they can express their needs, letting the system automatically transfer their vote from users's needs to those regulations that address them.

CAIRM was partly inspired by Information Technology:
*   From IT security Risk Management (RM) it borrows the flow leading from needs to regulations
*   From Agile software development it borrows the capability to cope with frequent changes
*   From SQL databases it borrows the idea of maintaining a coherent voting state at all times
*   From social networks it borrows a comments and rating system (with added features)

CAIRM is an open methodology conceived by Enos D'Andrea <cairm@edlabs.it>. Everyone is free to distribute it, use it and develop related software.

## OPENAI'S GRANT

This paper was originally intended as an application to the [Democratic Input to AI](https://openai.com/blog/democratic-inputs-to-ai) grant by OpenAI, an American artificial intelligence (AI) research laboratory. The program awards ten $100,000 grants "to fund experiments in setting up a democratic process for deciding what rules AI systems should follow, within the bounds defined by the law". Such processes should prove capable of establishing which rules AI, AGI and ultimately superintelligence systems should follow, supporting and complementing rather than substituting AI government regulation. In the context of the grant, advancements in the democratic process matter more than the sample answers and regulations produced during testing.

The proposal must be submitted by 2023-06-24. Selection is notified on 2023-07-16. The pilot including user participation (at least 500 uers) and feedback must be delivered by 2023-10-20. Within just three months the grantee is expected to: refine the process; design, develop and test the software; put the software in production; engage public; support operations; gather results; gather user feedback; report back on the outcome.

## CHALLENGES

In addition to the usual regulatory challenges, regulating complex and rapidly evolving fields like AI presents a whole new set of specific challenges. AI is dynamic, unpredictable and it might be difficult or even impossible to control. AI technologies are used within the regulatory process, exposing it to conflict of interests. For these reasons a dedicated methodology is required.

Regulatory challenges:
*   Not specific to AI:
    *   Anonymous voting (e.g. for preventing retaliation and mass-surveillance)
    *   Resilience to manipulation by interest groups (e.g. regulatory capture, monopoly)
    *   Representation: adequate representation and protection of minorities and majorities
    *   Negative effects on individuals not participating in votes or specific topics
    *   Unforseen Cost and negative effects of deliberated solutions
    *   Access: access to digital voting platforms by poor or segregated communities
    *   Interference: address inappropriate participation (e.g. trolling, fake accounts)
    *   Participation washing (i.e. only pretend to consider inputs)
    *   Self-regulation of individuals (e.g. do you want to pay taxes and fines?)
    *   Prevent over-regulation (which might  limit productivity and innovation)
    *   Scalability
    *   (others)
*   Specific to AI:
    *   Pervasiveness: AI affects almost all human fields
    *   Complexity: regulated field is so complex even most experts don't know it fully
    *   Dynamism: rapid changes in the regulated technology and its many applications
    *   Exponential growth: technology with unknown scenarios (narrow AI > AGI, super AI)
    *   Retrospective: regulation arrives after the technology is widespread
    *   New topic: regulation cannot rely on a significant body of information
    *   Point of no return: potentially irreversible scenarios
    *   Used technologies: LLM tools used in the process can influence voters
    *   Inevitability: AI might be difficult or impossible to control or slow down
    *   Insufficiently informed participants: esp. of non-technical subject matter experts
    *   Prevent unrelated technological advancements in other fields (e.g. medical)
    *   Access: access to global legislative processes from poor and censored countries
    *   (others)

## METHODOLOGY

CAIRM is fundamentally a social network with integrated Risk Management (RM) business logic. In it users, together with more privileged actors optionally supported by AI LLM systems, can create, manage, connect, discuss and eventually select risk components.

Voters are unlikely to be proficient with regulated fields (such as that of AI), just like in RM frameworks business owners are usually not unfamiliar with IT security. As in RM frameworks CAIRM voters start by expressing their needs. Differently from RM frameworks however, CAIRM users can also vote on the other risk components and they can optionally contribute to their creation.

User participation is structured so it does not interfere with the work on the rest of the framework by researchers and subject matter experts. On the contrary users could contribute to highlight problems such as the subject matter expert availability bias. Another peculiarity of CAIRM is that when external changes occur, the system can create a new set of regulations based on a former set with just minimal effort.

At the moment of writing, CAIRM only exists in theory. It is not yet provided as a software or service. Should this application to the aforementioned grant be accepted, a dedicated software will be created and released as open source. A dedicated information system will also be setup to host a pilot project, testing the effectiveness of the methodology, refining it and applying any useful adjustments that fall within allowed constraints.

### Risk components

CAIRM relies on categories of risk components, each having relations to some of the other categories. Risk components of a certain category can therefore be linked to risk components of some other categories, resulting in a navigable directional network of relations that goes from NEEDS towards SOLUTIONS.

Risk components:
*   NEEDS are situations or events that must be achieved or preserved
*   VULNERABILITIES are aspects of NEEDS liable to be misused or damaged
*   THREATS are voluntary or involuntary events that can exploit VULNERABILITIES
*   RISKS are the probability of THREATS exploiting VULNERABILITIES negatively impacting NEEDS
*   SOLUTIONS are aimed at reducing the likelyhood of RISKS to protect NEEDS

Each category will be precisely defined within the software with its name and description, in order to be legible and actionable. Names and descriptions can be adapted to the context, for example during a regulatory process a SOLUTION can be called "regulation" while during during an IT security audit it can be called "security control".

### Actors

CAIRM relies on multiple user roles for managing permissions. Most roles can be assigned by default and are only removed if misused, but this can change depending on the context. Upon registration users can also be asked to declare (and possibly demonstrate) any affiliation to institutions with possible conflicts of interest (e.g. stakeholder, government, organizer etc.).

Roles:
*   Non-privileged:
    *   VOTER: can vote on risk components
    *   DELEGATE: can be delegated to vote for others (pending acceptance)
    *   DEBATER: can comment and respond to comments
    *   PROPOSER: can propose risk components and relations
    *   AFFILIATE: its contents are tagged, cannot be privileged
*   Privileged:
    *   RESEARCHER: can edit and aggregate risk components
    *   MODERATOR: can moderate contents, can restrict user privileges
    *   ADMINISTRATOR: can assign/remove roles, can administer the platform

Roles *should* ideally be fine grained as a matrix, so users can be assigned permissions for individual role/component type. That would allow to easily reuse the platform in contexts where users should be more or less limited.

Anonymity is only allowed for individual voting, while all other actions (including voting by delegates) *must* be pseudonymized. Affiliates *must* be publicly tagged as such, so they can participate in discussions without suspects of manipulation. Affiliation *should* be verified. Privileged users *must* be strongly identified and authenticated.

Roles *should* also take into consideration the following:
*   Representation of minorities (by location, age, familiarity with regulated field etc.)
*   Representation of majorities (e.g. when a solution is only discussed by a minority)
*   Validation of researchers (e.g. subject matter experts and external researchers)
*   Training of users in regulated and related fields

### Software

In essence CAIRM is a social network with embedded risk management business logic.

Users interact asynchronously by editing risk management components, by connecting them, and by commenting on them, while the platform enforces a risk management business logic. Modifications and votes on risk components and their relations eventually reach a stable state wihout external intervention, at which point SOLUTIONS can be extracted.

An essential part of the business logic deals with modifications. After risk components or their relations are modified, the system walks through the risk chain, marking for revison those risk components which depend on modified ones. Once the required risk components have been manually revalidated, the remaining depending components are automatically revalidated.

Business logic:
*   Core
    *   Invalidate votes for [heavily] modified risk components
    *   Tag for review risk components that were affected by modifications
    *   Transfer votes from NEEDS to SOLUTIONS by walking through relations
    *   Search for existing contents (e.g. when inserting new content)
*   Optional
    *   Prevent DoS, automation and similar attacks
    *   Avoid polarisation (e.g. favouring most voted solutions)
    *   Foster participation on others' ideas (e.g. by mandating distributed peer review)
    *   AI-provided support services (see dedicated chapter)

Regulatory processes involve a large user base, so the software must be highly scalable (e.g. microservices and noSQL database).

The platform should be self-regulating. Active users are supposed to discourage bad behaviour by other active users through votes, comments and in extreme cases reporting. A dedicated business logic should foster security, for example a system scheduler could regularly perform statistical checks for user collusion reporting possible abuses to moderators.

### AI systems

The software could be supported by multiple AI LLM systems to improve its usability and effectiveness. It is essential that such systems do not negatively affect operations, for example by accidentally or deliberately inserting biased opinions and dark patterns that could influence users.

Possible use of AI LLM:
*   Suggest which risk components are similar
*   Propose aggregation of similar risk components
*   Detect logical fallacies in user responses
*   Propose improvements to risk components (e.g. based on length, clarity etc.)
*   Play the devil's advocate for the sake of brainstorming ideas
*   Detect angry posts to prevent unnecessary flames (e.g. ask user confirmation)

Possible mitigations to prevent LLM misuse:
*   LLM trained with official data (e.g. legal, scientific)
*   Using multiple LLMs and comparing user voting statistics on their proposals
*   LLM exclusion from content creation

## PILOT

As part of the aforementioned penAI grant, a working system must run a pilot engaging at least 500 participants by October 20, 2023. Since this project focuses on the metodology and not on the end results, and since the public selection process is common to other proposed solutions from which it can be borrowed, it will not be formally refined nor documented. Should the required user base not be reached, user participation will be incentivized by means of monetary or psychological rewards (e.g. gamification).

### Software

The pilot software will be developed using the following technologies:
*   Agile test-driven workflow, for easier debugging
*   Public repository, for collaboration
*   Python, for rapid prototyping
*   Microservices, for scalability
*   SpaCy, a python libraryfor searching text through tokens
*   One DB among ElasticSearch, MongoDB or PostgreSQL (to be decided)
*   GPT API or other LLMs, for supporting text functions 
    *   Aggregation of similar proposal
    *   Detect fallacies

### User participation

Participating Users can be either sent a personal invitation, or they can be allowed to freely register (possibly awaiting account validation before they can participate). Authentication will be available through passwords with optional TOTP and selected OAuth providers. As in other cases it was observed that retention is increased when users feel they are part of a community, internal discussion groups can be created based on users' affiliation or personal preference.

Participation *should* be encouraged via a scoring system, e.g. one rewarding participation and quality while discouraging quantity and mistakes. In order to balance the effect between those volunteering and those just voting, people could be given a limited number of votes to be distributed across all solutions.

Future AGI and super AI systems might also be considered for participation, at least providing suggestions.

### Pilot results

The results of the pilot will be extracted system at a predefined date. Risk components will be compared with those initially provided as sample.

### Sample risk components

CAIRM risk components can be created during the process, however starting the initial data works as an example, so the system can be used intuitively without significant training. For the purpose of this AI pilot a small initial dataset was created by the researcher. Each risk component can be modified or deleted. The initial relations between the data are not included in this text and will be established from within the software platform.

*   Risk component type:
    *   Risk component category: item 1, item 2, ...

Sample data provided as examples:
*   NEEDS
    *   Safety: right to life and health, combat local and online crime
    *   Peace: in communities, regions, nations, world
    *   Communities: protect local, distributed, online minorities (e.g. LGBTQ)
    *   Well being: quality of life, dignity, liberty, privacy, democracy, equality, 
    *   Education: school, morality, culture, art
    *   Vulnerable individuals: elderly, children, technophobics, w/cognitive impairment
    *   Economic: famine, poverty, social divide, right to work and fair pay
    *   Freedom: of thought, of speech, of religion
    *   Stability: economic, environmental, market, political, social
    *   Regulation: act in time, be effective prevent excesses
    *   Media: reliable news, reliable medias
    *   Science: benefit from present and future AI, avert imminent scientific risk
    *   AI rights: AGI rights?, superAI rights
*   VULNERABILITIES
    *   Psychological manipulability of individuals and/or communities
    *   Unavailability and/or cost of medical and/or psychological support
    *   Vulnerabilities of information systems
    *   The inner workings and weights of neural networks are unknown
    *   AI training on copyrighted data
    *   AI training can insert harmful or hate content
    *   Reliance of regulation on AI
*   THREATS
    *   Economic: market-driven decisions
    *   Substitution of humans: education, helpdesk
    *   Automatic inference from media: gender, race, emotion, identity etc.
    *   Self-regulation: by lobbies, by malicious/faulty AI, by malicious future AGI
    *   Social: censorship, hate speech, censorship
    *   Psychological: social engineering, fake news, social divide
    *   Regulatory: excessive regulation, inadequate regulation
    *   AI creation: biased training, malicious training, malicious personalization
    *   AI operation: malicious use, unpredictability, hallucinations, bias
    *   Environmental: AI power consumption, datacenter construction
    *   AI evolution: AGI, superintelligence
    *   Deepfakes: images, audio, video
    *   Copyright infringment: images, music, movies, trademarks, copyrights, patents
*   RISKS
    *   Disinformation loops
    *   Society: job loss, poverty, unrest
    *   Conflicts of interests (AI lobbies)
    *   Prevent useful technological advancements
    *   Dehumanization of society
    *   Loss of control over critical infrastructure
    *   Manipulation of public opinion
    *   Manipulation of regolatory authority
    *   Market disruptions
*   SOLUTIONS
    *   AI users and impacted individuals SHOULD be able to influence AI system behaviour
    *   Dedicated AIs SHOULD be developed to spot deepfakes, fake news and similar unwanted content    
    *   Critical systems should only employ certified AIs which MUST log sources for training data
    *   Certifications MUST be established for certifying AI within critical systems
    *   Critical services SHOULD use certified AI systems
    *   Services powered by AI MUST be labelled
    *   AI certification: certify AI training and operational parameters for critical systems

#### Use of AI

This specific CAIRM pilot on AI limits AI usage for multiple reasons:
*   Limit the workload ensuring pilot success
*   Avoid biased suggestions from LLM training (e.g. LLM favourable or contrary to AI)
*   Avoid dark patterns that might psychologically influence discussion and voting

Future versions of this pilot and/or other CAIRM projects are welcome to use AI in all phases provided that it is
*   Supervised by humans (this could be reevaluated when certified AI systems will exist)
*   Monitored for bias by using multiple AI systems and comparing their statistical influence on deliberations.

### User feedback*

After the pilot a poll will be lauched among all participating users. Participation is optional, should it be  insufficient it may be incentivated through rewards.

Evaluation will include
*   Participant satisfaction on UI, efficiency and effectiveness of the process, quality of results
*   Shifts from initial polarization
*   Optionally
    *   Shifts based on use of different LLMs
    *   (possibly others)

### Deliverables

All deliverables and internal documentation will be written in English.

Pilot deliverables:
*   Informational website describing the methodology
*   Web application and/or web mobile APP for discussion and deliberation
*   Final report including
    *   Insight on proposed solutions
    *   Aggregated/anonymized results
    *   User feedback
*   Presentation at conference(s) and/or publicly posted video

### Risks*

The pilot project is subject to many risks which jeopardize its completion and/or its quality.

The project might not be completed in time, in which case no money would be received. In that case to cover costs the software will not be released as open source but as SAAS. The methodology will remain publicly distributable but derivative works will be discouraged.

### Budget*

The project grant mounts to 100.000 $. All the money will be accounted for with original receipts, which will be scanned, anonymized and will be available for verification upon request. Amounts include taxes. Any money not spent for its reserved use will be redirected towards one of the other uses, or used eventually to disseminate the results (e.g. travel to give conferences).

Estimated budget use:
*   10.000 $ (20 days x 250 $/day) refinement of the business logic
*   10.000 $ (20 days x 250 $/day) software design
*    5.000 $ dedicated local IT system for LLM/AI experimentation + energy costs
*    5.000 $ (100 hours x 50 $/hour) ext. consultations on AI, legal
*   40.000 $ (160 days x 250 $/day) application development
*    5.000 $ (6 days x 500 $/day) ext. consultations on application development
*    5.000 $ (25 days x 200 $/day) public engagement work, e.g. supervision and moderation
*   10.000 $ public engagement costs, e.g. ads, rewarded participation
*    2.000 $ IT cloud infrastructure costs, e.g. hosting, housing, applications, LLM APIs etc.
*    3.000 $ (150 hours x 20 $/hour) IT infrastructure operation and maintenance
*    5.000 $ ext. security consulting, e.g. audit and penetration testing

### Team*

The lead author of this proposal is not a formal researcher (let alone a renowned one). However he is faimiliar with many fields: current state of AI, capabilities and security of IT systems, social sciences, futurism, psychology. These and other fields provide him with a privileged viewpoint to interface with field-matter experts and to correlate knowledge proposing an olistic solution.

Roles:
*   Project lead: Enos D'Andrea
*   Project assistant: **TODO**
*   AI consulting: **TODO**
*   System administrator: **TODO**
*   Software development: Enos D'Andrea, ChatGPT **TODO**
*   Software development consulting: **TODO**
*   Social and pshychology science consulting: **TODO**
*   Legal consultant: **TODO**
*   SEO for voting phase: **TODO**
*   DPO: Enos D'Andrea
*   Security consulting: Enos D'Andrea **TODO**
