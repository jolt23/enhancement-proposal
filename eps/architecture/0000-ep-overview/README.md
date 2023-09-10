# Enhancement Proposal Process

## Table of Contents

<!-- toc -->
- [Summary](#summary)
- [Motivation](#motivation)
  - [Business Case](#business-case)
- [Proposal](#proposal)
  - [Reference-Level Explanation](#reference-level-explanation)
    - [What Type of Work Should Be Tracked by a DEP](#what-type-of-work-should-be-tracked-by-a-DEP)
    - [EP Template](#EP-template)
    - [EP Workflow](#EP-workflow)
    - [Git and GitHub Implementation](#git-and-github-implementation)
    - [EP Author Role](#EP-author-role)
    - [EP Editor Role](#EP-editor-role)
    - [KPI's](#kpi's)
    - [Prior Art](#prior-art)
- [Drawbacks](#drawbacks)
- [Alternatives](#alternatives)
  - [Confluence](#confluene)
  - [OneDrive Documents](#onedrive-documents)
- [Unresolved Questions](#unresolved-questions)
<!-- /toc -->

## Summary

The Enhancement Proposal Process or EP is meant to be a way to bring
forth enhancements to the system, in a meaningful well though manner that
facilitates quick implementation across teams.

The EP process can help align multiple sig leaders to accomplish a single
enhancement. The process is also focused around brining in reviewers early on
in the design process and making them part of the solution.

It is also my expectation that the EP process will force the organization to
properly assemble into sig like organization with members owning each. A sig
owner is not meant to be a member of the team but instead a core contributor
which could be through implementation or ideation.

## Motivation

Many of us have been talking about having a proper way to collect and propose
changes across our system. In this attempt I am trying to take the
knowledge I have gained from having these conversation and turn it into a
process. One idea that came to me was the success that the Kubernetes community
has in making changes and how this is accomplished. There is a lot more to k8s
enhancements than KEPs but I thought it could be a create way of bringing in a
successful process and adopt it for our engineering needs.

Additionally many of our changes require enhancements across the stack and are
rarely limited to one team. One enhancement may lead to additional
instructors or services that need to be created to support its lifecycle. This
process is meant to open this process up and include the required folks early
on in the process.

### Business Case

The main business driver for this process is efficiency and audibility. As our
stack expands it becomes more difficult to make changes or we build more
technical debt with out properly informing owners. The purpose of this is to
improve this deficiency.

- Reduce number of meetings and leverage pull requests for review and approval
- Identify business initiatives that modify our stack and document why
- Find gaps and holes that need to be identified for solutions to be successful
- Create tangible successful criterions for enhancements.

The above should lead to dollar savings to the stack or allow to better track
cost of running business. Finally, this should lead to reduction in replication
of work and help sharing enhancements along with respective documentation with
others.

## Proposal

### Reference-Level Explanation

#### What work to track with a EP

Any effort of substantial change should have a EP created. That means this is
opinionated in nature. However, the first action in a EP is to discuss the
change within a given sig, after that discussion it should be clear if a EP is
required or not. However here are some actions that if we had to do all over
again would require EP.

- Adding Redis Cluster to K8s Platform
- GitHub as the Platform SCM
- GraphQL as the API Gateway

Examples above might be platform heavy, however in reality any core changes to
API should be tracked by a EP.

#### EP Template

**Please see: [EP Template](/eps/template/README.md).**

#### ep Workflow

A ep has the following states:

- `provisional`: The ep has been proposed and is actively being defined.
  This is the starting state while the ep is being fleshed out and actively defined and discussed.
  The owning SIG has accepted that this work must be done.
- `implementable`: The approvers have approved this ep for implementation.
- `implemented`: The ep has been implemented and is no longer actively changed.
- `staged`: The ep has been eployed to staging environments and has passed testing plan.
- `deferred`: The ep is proposed but not actively being worked on.
- `rejected`: The approvers and authors have decided that this ep is not moving forward. Exit state.
- `withdrawn`: The authors have withdrawn the ep. Exit state.
- `replaced`: The ep has been replaced by a new ep. Exit state.
- `completed`: The ep has been rolled out through production. Exit state.

#### Git and GitHub Implementation

Each ep is to be placed inside the corresponding sig which will own the
enhancement. Ownership of an enhancement will be shared between the Author of
the ep and the sig owners approving the ep.

The naming of a ep should be `draft-yyyy-mm-dd-name.md`, once the ep has
received a number it can be moved to a directory named `NNNN-name`, and renamed
to `README.md`. Each ep should be the main `README.md` file with in the
directory. It is possible to have additional files within the ep file as
supporting documents however this should be limited and should not take away
from the template.

ep should always be owned by a sig, even if cross sig approval is required a
single sig should own responsibility of tracking the enhancement.

### EP Author Role

I am a ep author what do I do?

The ep author is the person who initiates the creation of the ep and updates
it frequently based on feedback from reviewers. The author is not meant to
simply take direction on changes but should provide arguments for their
opinions and work with approval owners to come to a concensus.

The ep author is also responsible for moving the ep across its lifecycle
and to get to an end state. This state does not have to be `completed` it can
be any of the exit states.

While this seems like a lot of responsibility it is more of a facilitator role.
As a author creation of the enhancement idea or proposal is important but work
different sig owners to come to a complete solution. The expectation of this
process is to provide a strong foundation but work with cross teams to
accomplish the enhancement. This can be leaning on others for implementation
details or api reference or helping with process.

### KEP Editor Role

Taking a cue from the [Python PEP process][], we define the role of a KEP
editor. The job of an KEP editor is likely very similar to the
[PEP editor responsibilities][] and will hopefully provide another opportunity
for people who do not write code daily to contribute to Kubernetes.

In keeping with the PEP editors, who:

> Read the PEP to check if it is ready: sound and complete. The ideas must make
> technical sense, even if they don't seem likely to be accepted.
> The title should accurately describe the content.
> Edit the PEP for language (spelling, grammar, sentence structure, etc.), markup
> (for reST PEPs), code style (examples should match PEP 8 & 7)

KEP editors should generally not pass judgement on a KEP beyond editorial
corrections.
KEP editors can also help inform authors about the process and otherwise help
things move smoothly.

[Python PEP process]: https://www.python.org/dev/peps/pep-0001/
[PEP editor responsibilities]: https://www.python.org/dev/peps/pep-0001/#pep-editor-responsibilities-workflow


#### KPI's

To track the success of our process the following metrics will be tracked:

- number of eps created in a PI
- number of eps completed in a PI
- average number of changes per ep

#### Prior Art

The ep process is purposely stolen from the [Kubernetes ep process][]
Process. Which was stolen from [Rust RFC process][] :)

[Kubernetes ep process]: https://github.com/kubernetes/enhancements
[Rust RFC process]: https://github.com/rust-lang/rfcs

## Drawbacks

Teams could see a process like this feel difficult and long to complete. To
mitigate this the process of a ep is meant to be evolutionary. So while you
don't have to complete all the items, it provides a mechanism to put together
thoughts and ideas.

This process would require adoption from all teams to be successful. While this
can work within one team it maybe to much overhead.

## Alternatives

### Confluence

Confluence is great and has been a good part of our ability to document and
collaborate and work together. Today teams are already organized into spaces
and best practices on process and governance are laid out. However it is
difficult to have a review process with confluent.

The above layout could be created as a template in Confluence and we could add
a new section to an existing or new space and work through these requirements.
One benefit that confluence would produce is easily made these documents
available to product and other teams outside of engineering.

Additionally we are moving away from Bitbucket server and are trying to
identify how to keep documentation close to our source code.

In conclusion, confluence could be a good destination for a process like this
one however it does loose the ability for enhancements to have dedicated
reviewers and have an engineering first approval process.

### OneDrive Documents

Additionally we could use OneDrive or another mechanism to share documents. In
This scenario we could create a template document and have a process to review
any newly created proposal. However, similar to the Confluence alternative this
might become difficult to track down reviewers and understand responsibility.

The document perspective does bring however a better way to use images and
other graphical improvements to the process. This could be beneficial to add
color and more understanding to concepts. Additionally sharing documents could
be as easy as exporting and sending through an email or slack.

Overall managing a large number of files with in a OneDrive directory might
become difficult and this might be harder of a solution to manage than using
Confluence.

## Unresolved Questions

- How reviewers and approvers are assigned to a ep?
- How to automate ep process to track changes? What needs to built into this repository to manage it?
- Should we track metadata information about ep like eps do?
- How should architecture diagrams be linked and tracked?
- How to deploy ep's into an internal documentation hosting product?
- How to automate the table of contents for each markdown?
