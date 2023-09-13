---
title: "Foundational competencies and responsibilities of an RSE"
geometry: margin=2.5cm
author:
  - Heidi Seibold
  - Florian Goth
  - Jan Linxweiler
  - Jan Philipp Thiele
  - Jeremy Cohen
  - Renato Alves
  - Samantha Wittke
  - Jean-Noël Grad
  - Fredo Erxleben
  - Magnus Hagdorn
  - Harald von Waldow
  - Moritz Schwarzmeier
output:
  pdf_document:
    citation_package: biblatex
    toc: true
    number_sections: true
bibliography: bibliography.bib
header-includes:
    - \usepackage{pdflscape}
    - \newcommand{\blandscape}{\begin{landscape}}
    - \newcommand{\elandscape}{\end{landscape}}
---

**Abstract**:
In this paper we define the broad notion of what an RSE is and
give a list of foundational competencies that define the RSE profile.
Using that we elaborate on the progression of these skills along different
dimensions and give examples of future specializations.
An Appendix details how existing curricula fit into this framwork.

---

**Keywords**: research software engineering, training, learning, competencies


# Required Generic RSE skills
The role of an RSE lies somewhere on the spectrum between that of a researcher
(the "R") and a software engineer (the "SE") and, therefore, requires
competencies in both fields. RSEs typically apply their knowledge and
experience in larger teams which allows them to cultivate this hybrid nature.
Therefore, we categorise the competencies into software engineering skills,
research skills, and team skills with particular focus on the software and
research cycle and the scientific process. The generic skills are relevant in a
broad setting and form the foundation for specific specialisations.

These skills and competencies come into play in various forms: first of all the
RSEs themselves need to acquire and develop them as their career progresses
(**Career level**). However, some knowledge of software and data processing is
required at all academic levels and for all positions
(**Academic Progression/better title**). The relative importance of the skills
and competencies also depend on the size of the RSE team
(**Project team size**). Finally, different sets of skills are emphasised in
the different RSE specialisations (**RSE specialisations**).

## Software Engineering Skills
There are many software engineering curricula out there, that try to define
which tasks a software engineer should be able to perform. A recent example
highlighting some aspects in more detail than here is [@Landwehr2017].
The software skills outlined here are required to make research software adhere
to the FAIR principles. [@ChueHong2014] defines different levels of research
software reuseability and the extent to which the software engineering skills
need to be applied to reach them.

### Creating documented code building blocks (DOCBB)
The RSE should be able to create building blocks from source code that are
reusable. This ranges from simple libraries of functions up to complex
architectures consisting of multiple software packages. An important part of
reusability is that at least oneself, and ideally others, are able to understand
what a piece of code aims to do and how to use the provided functionality. This
is primarily achieved through a "clean" implementation and enhanced by
documentation. Documentation ranges from commenting code blocks to using
documentation (building) tools.

### Building distributable libraries (LIBS)
The RSE should be able to distribute their code with their domain/language
specific distribution platforms. This almost always encompasses
handling/documenting dependencies with other packages/libraries. It sometimes
requires knowledge of using build systems to enable interoperability with other
systems.

### Understanding the software lifecycle (SWLC)
The traditional software lifecycle defines the stages that form the process of building a piece of software.
This generally involves a creative process where you try to understand what it is that you need to build,
work out how you are going to build it and then implement it.
This is then followed by testing that things work as expected and that they continue to do so into the future.
We emphasize the the lifecycle is not complete here but also includes periods of maintaining a software
and also phasing out a software of its original use.

### Use repositories (SWREPOS)
The RSE should be able to use public platforms to share the artefacts they have
created and invite the public to scrutinise them for public review.

### Legal aspects (LEG)
The RSE should know licenses and their respective domains for data or software.
On an entry level, the competency is mostly about awareness: namely that different
(open source) licenses exist, that those might not be compatible with each other,
and that use of third party software might restrict licensing of the resulting work.

### Software Behaviour Awareness and Analysis (MOD)
We define this as a certain quality of analytical thinking that enables an RSE to
form a mental model of a piece of software in a specific environment.
Using that, an RSE should be able to make predictions about a software's behaviour.
This is a required skill for common tasks like debugging, profiling, designing good
tests, or predicting user interaction.

## The research skills
### Curiosity (NEW)
RSEs gain their reputation from their effectiveness to interact with their
domain peers. Therefore, some curiosity together with a broad overview of the
research field is required. Curiosity is also reflected when an RSE is actively
trying out new tools. Lifelong learning is then no longer just a phrase, but
becomes a motivation to work.

### Understanding the research cycle (RC)
One of the crucial skills of RSEs is their mental proximity to research
and they embrace being part of a larger community which,
despite friendly competition, shares the common goal of gaining knowledge
for its own sake and not just for personal or commercial gain.
Thereby they know, that they are part of a bigger cycle that involves many other parties in and outside of
their domain, and also that their software can be utilized in different stages of the research cycle by different persons.
Like other researchers, RSEs are open to discussions and arguments beyond
their own expertise and appreciate the underlying principles of
good research, like publications, review and reproducibility.

### Finding/discovering software and attribution (SD)
One goal of FAIR software is to avoid unnecessary duplication of work by reusing
existing work instead. To (re-) use software, researchers have to be able to
find it and then to easily evaluate if the software actually suits their needs.
Apart from functionality also licensing, integration with other software,
expected sustainability and expandability have to be part of this evaluation.
Finally, after obtaining/publishing results by modifying and/or using the
software, the original authors need to receive proper attribution.

### Using domain repositories/directories (DOMREP)
Almost all research software is developed within a specific scientific domain.
Some software may be able to cross boundaries, but the majority will have a
home domain, with which it needs to be able to interact. The RSE needs to be
aware of any domain specific software repositories, data sets and catalogues
and the RSE's software needs to be able to interact with the existing
domain-specific data repositories.

### Outside Party interaction (USERS)
Research software is often developed as part of the research process itself,
and like research, it will change in unpredictible ways
hence it often has to be developed very closely to its users, the researchers.
Therefore, roles like developers and users can seldomly be distinguished
as most people represent multiple roles ranging from end-users, up to funders.
However, regardless if this is the case or not: compared to other SE environments,
there is an unusually close interaction between and within different roles in research,
as well as between experts from different domains.
Often this means it is necessary for an RSE to think "outside their comfort zone",
but at the same time to be able to convey their knowledge and experience to experts
of other fields in a way they can understand more easily.
This includes their own domain knowledge in discussions with RSEs (from other domains),
as well as their SE knowledge when talking to domain scientists and also the
exchange of new techniques and algorithms to keep their software up-to-date.

## Team Skills
### Teaching (TEACH)
Working in a group means being able to effectively perform e.g. onboarding, or more formal teaching procedures to their colleagues.
This includes tasks such as consulting and mentoring since these also often aim at educating people.
We deliberately mention, that giving code reviews is also part of this skill, since
Code review can be part of teaching people on improving their skills.

### Project Management (PM)
The RSE should have knowledge about project management. At some institutes, it follows the practices of the local research groups,
but it is useful, if an RSE knows its place in a PM scheme, or can bring in new ideas for improvement.

### Working in a team (TEAM)
There are various facets to working in a team. They range from functioning in a team to leading a team.
It includes following measures that increase team cohesion like performing code reviews.

## RSE Tasks and Responsibilities
These skills, while already numerous are also generic on purpose. They span a
multidimensional space in which the day-to-day tasks and responsibilities of a
RSE can be found. A snapshot of what this means today can be obtained 
from  learners and novice RSEs that we asked during the Paderborn workshop
what they would like to have learnt. Among the top five things mentioned were:

- Testing. This task is a manifestation of the SE competencies of DOCBB and MOD
since a model of the software is required in order to write good tests that
facilitate understanding and documentation. Today this encompasses the
knowledge of testing frameworks and CI/CD practices.
- Contributing to large projects. This is a topic that requires competency in
SWREPOS, LEG, in order to understand the ramifications of sharing, and DOCBB,
since the contributed code has to be understood by others. Interacting with
project members depends on the the TEAM skill. Today this entails the effective
use of collaborative platforms like github/gitlab, honouring a projects Code of
Conduct, and some knowledge of software licenses like the GPL.
- When or why to keep repositories private. This decision requires knowledge in
the RC, to understand when it makes sense to open up or close down a repository.
The USERS, TEAM and sometimes LEG skills are required to make this decision.
Furthermore, knowledge of the practices and contractual regulations of the
RSE's institution are also required.
- Proper Development. This broad topic requires all of the SE skills. Of course
these are the competencies that are the most fluid since they have to adapt at
a high rate to the technological advancements. Additionally proper SE skills
often require knowledge of TEAM, and PM. Today this means effective use of IDEs,
static analysis tools, design patterns, documentation (for oneself and others),
etc.
- Finding a community. This can be interpreted in two different facets. First
we have the aspect of community building for a research project. Since this
deals with software that is supposed to be used in research this requires
knowledge of RC, USERS, and also NEW, in order to effectively interact with
domain scientists. Today, an example is a presence on social media. The other
TEAM-related aspect is the embedding of RSE graduates into the community of
RSEs. We envision our RSE graduates to be a part in a strong network of other
RSEs, tool-related communities and the classical domain communities. This point
is further elaborated in [How do we reach people in different stages of their careers](#how-do-we-reach-people-in-different-stages-of-their-careers).


Beyond that, we feel that today Other important tasks of RSEs are

- Mentoring colleagues.
  This necessitates giving good advice that fits to a projects stage in its lifecycle,
  thereby requiring knowledge of (SWLC), and its context in its research domain, thereby requiring knowledge of (RC).
  Research software often starts out as a tool to answer a personal research
  question and becomes more important when other researchers rely on it.
  Some research software might even be used to deal with critical questions such as weather forecasting or medical diagnosis.
  To formalize the process of giving good advice a classification of software is commonly used [@Wang2012; @Schlauch2018b]
  where research software can move from one class to another during its lifecycle.
  [@Schlauch2018b] classify applications based on their scope and criticality and provide software engineering recommendations.
  The RSE needs to be able to identify the application class they are dealing with and apply the respective RSE practices.

- Enforcing reproducibility. Projects like [@ReproHack] can greatly help in fostering that competency.

# How much do different people need to know?
Now that we have the different competencies, we can explore various dimensions of these competencies,
depending on their circumstances. A strong beneficiary of specialized RSEs can also be newly formed RSE centers at research institutions.

## Career level
At different career levels, differing skills are required. We have set this up according to the following separation often applied within a single project:

- Junior RSE: These are persons that have just started, but generally speaking they should have the skills to contribute to software projects
- Senior RSE: They have gained experience and can set the examples in the software project.
- Principal RSE: Their actual job description varies a lot. These may be RSE team leaders based in a professional services type role, or they may be professors or research group leaders based in a more academic-focused role. They are often the people responsible for bringing in the money that supports new projects and sustains existing projects. Generally speaking, they do not need to to be actively involved in the day-to-day technical tasks but they should be able to guide projects from both a technical and research perspective.

The required skills are distributed according to this table
First Dimension: Career path e.g. Junior RSE -> Senior RSE -> PI scale (1->6) (less -> lot)

\blandscape
\small
\renewcommand*{\arraystretch}{1.4}

|       | Junior | Senior | Principal RSE(brings in funding)  |
| ----  | -------------- | -------------- | ------------------ |
| DOCBB | should be able to write reusable building blocks |same as junior, but the quality should set the standard for the project, while following current best practices | should know the current best practices and point its people to the right resources. |
| LIBS  | should be able to use package distribution platforms      | same as junior, but should set the project standard and follow current best practices. | should ensure that their project is in an up-to-date distribution platform |
| MOD   | should have a basic grasp of their piece of the software in order to use basic tools like a debugger | Should understand the characteristics of large parts of the codebase considering a variety of the metrics | Should understand the big idea of the software project in order to define the task that the software solves  |
| SWLC  | Awareness about the existence of the software lifecycle. | Should know which decisions lead to technical debt. | Should know in which part of the lifecycle their project is and how to steer development/project resources accordingly. |
|SWREPOS| Seamless interaction with the swrepo of their project is a must | Should be well-versed in the intricacies of a swrepo, and probably interact with multiple projects' repo's | Should be able to effectively interact with swrepos and especially the interaction with the connecting projects. |
| LEG   | Awareness about legal intricacies about sharing code | Should be able to give advice on legal issues and resolve the most common issues | same as Senior RSE |
| NEW   | Some curiosity required to fit into research teams | same as junior, but a curiosity to enhance the code base is required | Curiosity to know in which direction to steer the project is required |
| RC    | Awareness about the RC | should know the position of the project in the RC | Should know what is necessary for the project to fit into its position in the RC |
| SD    | Should be aware about tools for SD |   Should be able to find sth. with SD tools    | Should be able to effectively find sth. with SD tools and be able to evaluate and perform the integration of a library into the project. |
| DOMREP| The RSE should be able to interact with the domain repository | same as junior RSE | same as junior, and should know about how it fits into workflows surrounding these domain repositories |
| USERS | The RSE should be able to communicate with non-SE users of the project | same as junior | same as junior, and take feedback into account of the steering |
| TEACH | should be able to perform simple peer-to-peer onboarding tasks | should be able to explain logical components to other RSEs | Should be able to effectively communicate about all large-scale parts of the project. |
| PM    | Awareness about the employed project managemement method | Should be able to use the employed PM method | Should be able to design and adapt the employed PM method. |
| TEAM  | Should be able to work in the team in order to effectively fulfill the given tasks. Should be able to learn from code review. | Should be able to break down tasks into more easily digestable sub-tasks | Should be able to lead the team and set the respective direction. |

\elandscape

## Academic Progression / Career Path? (Help me for better title) 
In the previous section, 
we looked at the competency levels needed for RSE specialists.
However, many of these competencies are important for typical researchers in academia.
Naturally, the 'R' competencies apply 
and research in general is increasingly team based.
Additionally, many researchers in fields from classical examples like 
numerical mathematics or theoretical physics 
to newer disciplines like digital humanities
will spend time in their research on writing and developing software.
Therefore, RSE focused training, e.g. in a Masters programme, 
is also beneficial for students in these fields
resulting in a broader audience. 

This section outlines how the RSE competencies could be reflected at all academic levels. 
It is important to note that this section does not reflect the current state of academic training and research institutions.
Instead, it summarises the discussions with and between workshop participants at different levels of academic progression on what they would have liked to learn at an earlier stage or know before starting their current position.
While individuals already work at implementing some of these changes and teaching these skills it has not yet reached a systemic level.

The text is organised along the academic progression path (Bachelor, Master, PhD, PostDoc, PI/Professor). 
Since each level is based on the previous levels we presume that the skills and competencies at each level also encompass those of the previous levels.
Due to the broad need throughout academic specializations,
the described levels serve as a baseline 
and certain fields will require higher SE skill levels 
as development is a large part of their actual research.

### Bachelor
Students at undergraduate level mostly consume science/knowledge.
During their studies they should also learn about the existence of digital tools and structures.
Undergrad students should be aware that RSEs exist and that software has different quality aspects (DOCBB).
They should be aware of domain specific tools (LIBS, SD) and where to find them (SWREPOS, DOMREP).
At this level it is sufficient to consider software as black boxes (USERS) although some training in data presentation would be very helpful and a good way to find out about programming (MOD, NEW).
They should have an awareness of software licenses and who to ask if they have any questions (LEG).
They will be taught about the research cycle (RC) and that researchers often work in groups (TEAM).
During practicals they will have an opportunity for peer learning (TEACH).

### Master
A student at Master level can participate in science and should therefore be able to use "some" digital structures. 
A master student needs to be aware of relevant tools and data sets for their domain, where to find them and how to use them (LIBS, SWREPOS, DOMREP).
They should be able to process and present their data (MOD).
They need to understand how their research depends on software (SWLC).
Working on their master thesis allows them to understand the research cycle (RC), practice project management (PM) and collaborate with other members of their research group (TEAM).

### PhD
A PhD student performs independent research under guidance. 
They need to know relevant tools and structures. 
They should know where to find information about tools and where to find help using them (DOCBB, SWREPOS). 
They should be able to use the tools (LIBS) and identify and report bugs (MOD). 
They need to be aware that the user's perspective is different from the developer's perspective in order to be able to write bug reports (USERS). 
They might produce new software (MOD, SD) in which case they need to understand how to license their code (LEG). 
PhD students need to be curious to be able to conduct their research. 
In order to be able to explore new tools (NEW) they must be able to evaluate research software (SWLC). 
They need to be able to interact with services (RC) and domain specific repositories (DOMREP). 
They should be able to supervise a student (TEACH).

### PostDoc
PostDocs are independent researchers. 
Their role is similar to that of a PhD student with a deepened focus on their research career.
However, they are proficient users of all relevant tools, that make them active contributors to their domain of research.
They need to be aware of patents (LEG).

### PI/Professor
They are experts in their field and should be able to give proper guidance to their students on which digital tools are currently relevant. 
They should be aware of the skills of an RSE and when they might need one in their group (DOCBB). 
They should encourage their students to use relevant tools (LIBS). 
They need to be able to judge the suitability of the software (SWLC) and follow the interactions between relevant projects (SWREPOS). 
They should be able to advise their students on legal aspects of the software (LEG). 
They should be able to contribute meaningfully to the steering decisions of the software in their field (USERS).
They need to guide students and give full-size lectures (TEACH). 
They need to manage and lead their research group (PM, TEAM).

## Project team Size
Some explanation of the team sizes:

- individual: A single person working on their research software
- Small team(~4 persons) This is a small team, that has decided to work together on something
- Organizations( >10 persons): These are big organizations with clear structures and a bigger degree of specialization.

\blandscape
\small
\renewcommand*{\arraystretch}{1.4}

|       | individual | small team | organization  |
| ----  | ----------- | ----------- | --------------- |
| DOCBB |   you might get away with less satisfactory code, as long as the product is OK | think about your colleagues    | your organization most likely has guides here |
| LIBS  |   you will only be successful if your artefact is usable by others    |  same here   | your organization probably has rules here |
| MOD   | you should precisely know what your entire code is doing where | you should know what your part is doing and have a feeling about the others contributions | You should know what your small part is doing |
| SWLC  | it's you and your software | You should know the Bus factor | The organization takes care of that |
|SWREPOS|   you need academic credit.    |   same here    | your organization probably has rules here |
| LEG   |   you carry the responsibility    |  someone in your group needs to take car of this    | your organization will have specialized people for it |
| NEW   |   You need a motivation to do this alone    |   ?    | Not so much, since other people might do this task |
| RC    | ? | you should maybe talk among your peers where your software fits in | You define your research cycle |
| SD    |   you need to be able to build on other work to be successful    |   same here    | there might be someone in your organization who does this |
| DOMREP|   You're doing science in a domain    |   there should be a person in your team who knows how to do it    | your organization might have specialists for that, but some basic familiarity |
| USERS | at one point you hope to have users | same here | maybe you have specialists for outreach |
| TEACH |   N/A   |   able to peer teach    | teaching to groups |
| PM    |   Not much required  |  able to follow checklist     | Working with PM tools, or use them for organization |
| TEAM  |   N/A    |   should be able to give equal feedback to their colleagues    | should be able to work within their role |

\elandscape

Bonus points may be distributed if managing teams remotely

[BIO Excel framework](https://competency.ebi.ac.uk/framework/bioexcel/3.0/carreer-profiles)

# RSE specializations
What we have defined above are intended to be base skills that an RSE irrespective of domain, place, and time should know about.
But not all RSEs are created equal, they specialize in different areas,
some of which we want to present below. Many of the specializations may overlap,
so the same RSE might for example work on data management and on Open Science.

## HPC-RSE
RSEs with a focus on High Performance Computing (HPC) have specialist knowledge
about programming models that can be used to efficiently undertake large-scale
computations on parallel computing clusters. They may have knowledge of (automatic)
code optimization tools and methods and will understand how to write code that is
optimized for different types of computing platforms, leveraging various efficiency
related features of the target hardware. They are familiar with HPC-specific
package managers and can build dependencies from sources. They also understand the process of
interacting with job scheduling systems that are often used on HPC clusters to
manage the queuing and running of computational tasks. HPC-focused RSEs may be
involved with managing HPC infrastructure at the hardware or software level (or
both) and understand how to calculate the environmental impact of large-scale
computations. Their knowledge of how to run HPC jobs and write successful HPC
access proposals can be vitally important to researchers wanting to make use of
HPC infrastructure.

They may also be familiar with High-Throughput Computing (HTC) and manage
a network of heterogeneous compute resources, typically desktop workstations
equipped with multicore processors and possibly GPU accelerators.
They can apply their node-level performance engineering skills to maximize
utilization of the available resources.
Finally, they typically have expert knowledge in at least one compiled language,
and can assist domain scientists who have excellent command of scripting languages
but only a cursory understanding of compiled languages get up to speed with
compiled software.

## ML-RSE
The development of research software based on machine learning (ML) requires specialized theoretical background and experienced handling of appropriate software in order to produce meaningful results.
This involves knowledge about data analysis and feature engineering, metrics that are involved in ML, ML algorithm selection and cross validation, and knowledge in mathematical optimization methods and statistics.
ML-RSEs analyse and check the suitability of an algorithm if it fulfils the needs of a certain task and they play a main role in deciding and selecting machine learning libraries for a given task.
The increasing usage of ML in numerous scientific areas with social impact, involves an emphasized awareness and consideration of possible manipulative or discriminatory influences.
At the intersection of data science [@SSIDataScience] and Data-focused RSEs, the complex way of solving problems utilizing machine learning calls for this separate specialization.

## Research Infrastructure RSE
This RSE is interested in SysOps and system administration and sets up IT infrastructures for and with researchers.
Therefore, this specialization on the one hand requires a deep knowledge of physical computer and network hardware and
on the other hand knowledge about setup and configuration of particular server software.
Those specialised RSEs know how to acquire, setup and maintain general-purpose as well as domain specific infrastructure,
e.g. setup of virtual machines on hypervisors or the planning and setup of compute server clusters for GPU based machine learning.
As an interface between the researchers and the infrastructure, they take care of user management, access permissions, and configuration of required services, for example.

## Web-Development RSE
This RSE is skilled in web applications, front- and/or backend, and/or building 
and using APIs, for example for research data portals or big research projects.
Ideally, this RSE should also have knowledge about (web) accessibility to allow a broad
range of researchers or even the public to use the resulting applications.
Therefore a deep knowledge of web skills is a required skill for this RSE.

## Legal-RSE
With the prevalence of software, we foresee the need for RSEs that specialize in legal questions around software.
They are the go-to person if people have a question about licensing, mixing and matching of software as well as patenting or copyright.
The publication of research software also requires knowledge about particular laws or regulatory frameworks concerning data protection, like the GDPR within the EU [@GDPR].
Familiarity with legal aspects of cybersecurity and export control in science and research (see [@ExportControl] for Germany) complete the competencies of those RSEs.

## Data-focused RSE
RSEs working at the flourishing intersection between data science and RSE. 
They are skilled in cleaning data and/or running data analyses and can help researchers
in setting up their analysis pipeline and/or research data management (RDM) solutions.
When the field requires research on sensitive data or information, e.g. patient information in medicine, 
this RSE should have knowledge about secure transfer methods and/or ways to anonymize the data.
As part of RDM, this RSE profile is able to support all stages of the research data lifecycle[@Nieva2020], with synchronous data management processes. 
Those processes implement established best practices for planning and documenting of data acquisition in a data management plan (DMP) as well as for management,
storage, and preservation of data, and publication and sharing of data in repositories according to the FAIR principles [@FAIR].

## OpenScience RSE
Open Science and FAIRness of Data and Software are increasingly important topics in research, as exemplified by the demand of an increasing amount of research funding agencies requiring openness.
Open Science RSEs can help researchers navigate the technical questions that come up 
when practicing Open Science, such as "How do I make my code presentable?", 
"What do I need to consider when it comes to licensing?", or 
"How can I use version control / automation for my project?".

## Project/Community manager RSEs
When research software projects become larger, they need someone who manages
processes and people. Building a community around a research project is an
important building block in building sustainable software [@Segal2009], so these RSEs play
an important role, even if they do not necessarily touch much of the code themselves.

## Teaching RSEs
RSEs who focus on teaching the next generation of researchers and/or RSEs play
a vital role in improving the quality research software.

## ${DOMAIN}-RSE
While software is the lingua franca of all RSEs there will be RSEs that have specialized in the initricacies of one particular research domain,
 such as medical RSEs, digital humanities RSEs or physics RSEs.

## Optional RSE competencies -> Maintenance RSEs
Oftentimes, a significant amount of effort in (research) software development needs to be spent on maintenance to ensure that software remains useful for researchers now and in the future.
The research environment is constantly changing and this can also apply to the software requirements.
If software is not properly maintained, it becomes increasingly difficult to install and use. 
At some point, the software is no longer available and cannot be used to reproduce results.
While ensuring maintenance and sustainability of research software is of huge importance to the communities that build and use it,
a particular challenge is that it is often very difficult to obtain ongoing research funding for software maintenance tasks.
As a result, when a project that developed or extended a piece of software finishes, support for the software fades as team members move on to other research,
academic or RSE roles, or become busy with other funded work.
While this is not a core concern of this paper, we wanted to highlight this important issue that is frequently faced when working with software in the research community.
With regard to which additional competency is required,
these are people having experience with ancient software stacks that are not anymore part of the general curricula (think of COBOL and FORTRAN).

FIXME: I think it would be nice if we could move each of these optional competencies to a different specialization.

# Reaching out to potential RSEs
Many current RSEs have found their way to being an RSE during their doctoral studies.
This transition usually happens slowly. You start programming a tool, and someone else likes it, it becomes known that you have programming skills and suddenly you are the RSE of the group that everyone would like to have in their projects.
If you enjoy this role, you need to be aware that there is a RSE career path as well as that specialized training materials exist.
Beyond that, for an RSE it is important to be a part of a network with other RSEs, irrespective of the career level.
A perfect first step for forming this network is topic-related conferences, workshops or meetups.
Beyond that, there is the broader RSE community organized at the local and regional level with chapters or local/regional communities, at the national level with societies and the international RSE society.
Each of them offers possibilities for connecting within or beyond an individual institution and is a great way to find like-minded people to grow a wider network and thereby facilitate the sharing of information on interesting events or help each other out.
This available layered network can greatly benefit the RSE in finding help with issues outside of their own comfort zone
and provides a welcoming, social safety net providing a home for the RSE. Since we feel providing aspiring RSEs this net
is of utmost importance we envision compulsory events introducing that to young RSEs.
Qualification badges are another venue, that RSEs to find people with the same technical interest.
Structuring and institutionalizing the education and structures for the add-on courses that are also open to others in academia,
will be topics of a follow-up paper.

# Conclusion and Outlook
This paper started from a community workshop at deRSE23 in Paderborn
where people working in RSE related fields got together to figure out 
structures and ideas of educating newcomers to this field.
One outcome of this diverse gathering is that RSEs from far away fields gather around similar concepts.
In this publication we have tried to formalize them. We have formulated a set of values that
guide our actions in society and manifestly makes RSEs part of the community of values of scientists
but at the same time, being Software Engineers, we have to take responsibility for our tools.
We continue with core competencies that have on purpose been formulated 
abstractly without referencing any particular information processing device.
As expected, we draw equally upon notions from software engineering and research,
but find that we likewise require teamwork capabilities.
We continue with detailing these competencies in various dimensions, and find that
a different amount is required in different positions and scientific domains.
Nevertheless, they are required and hence the values and competencies form a common denominator
that unifies RSEs and enables them to identify with this domain.
These competencies at the intersection of research and software engineering 
coupled with a firm believe in team processes makes RSEs sought after on the job market
and their values make them responsible members of a digital society.
This yields a qualification profile which makes
an education based on them highly attractive to young people and the institutions that provide
this education will be the topic of a follow-up paper.

# Appendix

## An applied example curriculum
## An example of a possible career path
- We can follow Kim, who has been the protagonist of the original deRSE Paper.

## HPC skills and certification

As an area that generally requires a range of advanced skills,
High Performance Computing (HPC) is one field where there is ongoing work
to identify relevant sets of skills for HPC practitioners and potential paths
to develop these skills. The HPC Certification Forum [@HPCCFCompetencies] has
developed a competence standard for HPC that defines a range of skills and
how they are related in the context of a skill tree [@Kunkel2020a; @Kunkel2020b].
This competence standard is currently being built upon by the CASTIEL 2 [@CASTIEL2] project
in collaboration with initiatives funded by the European High Performance Computing
Joint Undertaking (EuroHPC JU) to create a framework for HPC certification [@EuroHPCJU2023].

Also looking at pathways and how different skills are related,
the UNIVERSE-HPC project [@UNIVERSEHPC], funded under the UK's ExCALIBUR
research programme [@EXCALIBUR], is looking to understand and develop
training pathways to support the development of specialist skills in the HPC
and exascale domains. The project is gathering open source training materials
to develop curricula that support the training pathways that are underpinned
by high-quality training materials.

## Bioinformatics skills and certification

Bioinformatics is another field that actively works on developing skill trees.
The Bioinformatics Core Competencies [@Mulder2018; @Welch2016; @Welch2014],
the BioExcel competency framework [@Matser2016],
the PerMedCoE competency framework [@Lloret-Llinares2021],
the Research Data Management and Data Stewardship competence framework [@Demchenko2021]
and the ELIXIR Data Stewardship Competency Framework for Life Sciences [@Scholtens2019]
are examples of grassroot efforts aiming at defining the set of skills
of various bioinformatics specialties,
one of them as a taxonomy [@Mulder2018].
These frameworks eventually converged into the EMBL-EBI Competency Hub
[@CompetencyHub; @Lloret-Llinares2022],
where typical RSE and bioinformatician profiles at different levels
of seniority can be queried
(e.g. [Junior RSE](https://competency.ebi.ac.uk/framework/bioexcel/3.0/profile/view/10115/alex-2),
[Senior Computational Chemist](https://competency.ebi.ac.uk/framework/bioexcel/3.0/profile/view/10121/kim-0))
and compared against one another
(e.g. [Junior vs. Senior RSE](https://competency.ebi.ac.uk/framework/bioexcel/3.0/profiles/compare/10115/10117)).

Competencies can be divided into more fine-grained building blocks:
knowledge, skills and abilities (KSAs). They can be organized in a taxonomy,
and are also transferable, i.e. a KSA can be a pre-requisite to multiple competencies.
The Mastery Rubric for Bioinformatics [@Tractenberg2019] and the ELIXIR
Data Stewardship Competency Framework for Life Sciences [@Scholtens2019]
are examples of KSA frameworks for bioinformatics curricula.

The Curriculum Task Force of the International Society for Computational
Biology (ISCB) curates a database of degrees and certificates
in bioinformatics [@BioinformaticsCertification; @Mulder2018].
The database includes Bachelor and Master's degree programs and specializations,
Ph.D. programs, and certificates from graduate schools.