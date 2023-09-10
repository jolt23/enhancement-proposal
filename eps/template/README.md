# EP-0000: Enhancement Process

<!-- toc -->
- [Status](#status)
  - [Jira](#jira)
- [Proposal Checklist](#proposal-checklist)
- [Summary](#summary)
- [Motivation](#motivation)
  - [Business Case](#business-case)
  - [Goals](#goals)
  - [Non-Goals](#non-goals)
- [Proposal](#proposal)
  - [Architecture](#architecture)
  - [User Stories](#user-stories)
    - [Story 1](#story-1)
    - [Story 2](#story-2)
  - [Notes/Constraints/Caveats (Optional)](#notesconstraintscaveats-optional)
  - [Risks and Mitigations](#risks-and-mitigations)
- [Design Details](#design-details)
  - [Test Plan](#test-plan)
    - [Prerequisite testing updates](#prerequisite-testing-updates)
    - [Unit tests](#unit-tests)
    - [Integration tests](#integration-tests)
    - [e2e tests](#e2e-tests)
  - [Upgrade / Downgrade Strategy](#upgrade--downgrade-strategy)
- [Production Readiness Review Questionnaire](#production-readiness-review-questionnaire)
  - [Rollout, Upgrade and Rollback Planning](#rollout-upgrade-and-rollback-planning)
  - [Monitoring Requirements](#monitoring-requirements)
  - [Dependencies](#dependencies)
  - [Scalability](#scalability)
  - [Troubleshooting](#troubleshooting)
- [Implementation History](#implementation-history)
- [Drawbacks](#drawbacks)
- [Alternatives](#alternatives)
- [Infrastructure Needed (Optional)](#infrastructure-needed-optional)
<!-- /toc -->

## Status

<!--
Update the EP status based on the latest state of the proposal.
- `provisional`
- `implementable`
- `implemented`
- `staged`
- `deferred`
- `rejected`
- `withdrawn`
- `replaced`
- `completed`
-->

**status here**

### Jira

<!--
List of Jira Epics tracking design and implementation.
-->
- Jira Epic or Story Link

## Proposal Checklist

<!--
The following checklist of items are required to be completed before this
proposal is marked as complete.
-->

- [ ] Business Case? How does the use case fit within the current landscape of the app?
- [ ] What is the timeline for release?
- [ ] Architectural diagrams created and completed?
- [ ] Location of enhancement, will this cloud, ship side or both?
- [ ] Identification of hyper-visor solution, is this a VM or containerized solution?
- [ ] Identification of sizing footprint of VM or container?
- [ ] Will firewalls, DNS, and SSLs will be needed?
- [ ] Has profiling or performance test been executed?
- [ ] How will this solution be monitored? Do current monitoring solutions fit?
- [ ] What team will own the solution?
- [ ] What automation is being leveraged?

<!--
**Note:** The checklist above is not meant to be completed before the proposal
is complete. However this checklist is part of the production readiness and
must be completed before deployment to production and completion of proposal.
-->

## Summary

<!--
In this section you should be able to create a good description of what the change
is and generally how this change impacts systems and processes. Write the summary
from the perspective of someone who does not have any understanding and will be
using this enhancement as a user. Identify any high level plans or release
timelines required for this EP.

Think about the deployment footprint will this be a cloud, ship or deployment
across both. Identify if major dependencies and any requirements needed to get
started.

The length of a summary is up to the creator of the EP, however something to
short would not provide a good understanding something to large would take away
from the template.
-->

## Motivation

<!--
This section is about identifying the need for the enhancement. Is this a
Revenue generating change? Is this a cost saving enhancement? Are we trying to
reduce technical debt?
-->

### Business Case

<!--
What is the Business Case for the enhancement? Here describe the business unit
that will be benefiting form this requirement and how it will generate revenue
or optimize cost. The goal is to understand the importance of technically
enhancements to the way that business revenue or cost happens. This also allows
to understand timeline and other factors to the enhancement requirement.

The Business Case should describe and explain how this enhancement will impact
a guest or crew member.
-->

### Goals

<!--
List the specific goals of the EP. What is it trying to achieve? How will we
know that this has succeeded?
-->

### Non-Goals

<!--
What is out of scope for this EP? Listing non-goals helps to focus discussion
and make progress.
-->

## Proposal

<!--
This is where we get down to the specifics of what the proposal actually is.
This should have enough detail that reviewers can understand exactly what
you're proposing, but should not include implementation details.
-->

### Architecture

<!--
Provide a list of architecture Diagrams that provide a description of the following:
- [ ] Ship and Cloud Connectivity and Integration
- [ ] Component Composition and Target Deployment Hypervisor
- [ ] External thirdparty Integrations
- [ ] User or Client interaction with components
- [ ] Stateful or Database requirements
-->

### User Stories

<!--
Detail the things that people will be able to do if this EP is implemented.
Include as much detail as possible so that people can understand the "how" of
the system. The goal here is to make this feel real for users without getting
bogged down.
-->

#### Story 1

<!--
High-level template TBD
-->

#### Story 2

<!--
High-level template TBD
-->

### Notes/Constraints/Caveats (Optional)

<!--
What are the caveats to the proposal?
What are some important details that didn't come across above?
Go in to as much detail as necessary here.
This might be a good place to talk about core concepts and how they relate.
-->

### Risks and Mitigations

<!--
What are the risks of this proposal, and how do we mitigate? Think broadly.
For example, consider both security and how this will impact the system.

Has security reviewed this enhancement? Does security need to do a scan? Is
this dependent on a new technology or vendor?

Does this impact UX or UI, if so do we have a plan to retrain operators or
guests who consume the UI.
-->

## Design Details

<!--
This section should contain enough information that the specifics of your
change are understandable. This may include API specs (though not always
required) or even code snippets. If there's any ambiguity about HOW your
proposal will be implemented, this is the place to discuss them.
-->

### Test Plan

<!--
How is this enhancement going to be tested? Are Unit Tests possible, will
Postman scripts be used to test the functionality. What type of integrations
need to be tested pre and post deployments.

A test plan should also describe any testing differences between cloud and
ship if these exist.
-->

#### Prerequisite testing

<!--
Based on reviewers feedback describe what additional tests need to be added prior
implementing this enhancement to ensure the enhancements have also solid foundations.

Do we have the required testing tools? Do we need data for tests or data can be
generated?
-->

#### Unit tests

<!--
TBD
-->

- `<package>`: `<date>` - `<test coverage>`

#### Integration tests

<!--
TBD
-->

- <test>: <link to test coverage>

#### e2e tests

<!--
TBD
-->

- <test>: <link to test coverage>

### Upgrade / Downgrade Strategy

<!--
How is this technology upgraded? Is this to be upgraded in place or can be
replaced? Is new infrastructure required during upgrades? What type of sate is
required to be maintained during an upgrade.

Does this enhancement allow for us to downgrade to a previous version?

Identify what would be the plan for ongoing upgrades and downgrades to the
enhancement.
-->

## Production Readiness Review Questionnaire

<!--
The production readiness review is required for all enhancements to to rolled
out to any production environment.

The production readiness review questionnaire is not subject to on the below
questions, reviewers are welcome to add additional questions that would be
required.
-->1

### Rollout, Upgrade and Rollback Planning

<!--
TBD
-->

#### How can a rollout or rollback fail? Can it impact already running workloads?

<!--
Think of fail fast and always assume integrations are not guaranteed to work.
Identify not only internal failures to the enhancement but what other parts of
the stack can cause a failure.

If a failure does happen what type of impact are we going to expect? Can this
impact workflows that are not using the enhancement.
-->

#### What specific metrics should inform a rollback?

<!--
What signals should users be paying attention to when the feature is young
that might indicate a serious problem?
-->

#### Were upgrade and rollback tested? Was the upgrade->downgrade->upgrade path tested?

<!--
Describe manual testing that was done and the outcomes.
Longer term, we may want to require automated upgrade/rollback tests, but we
are missing a bunch of machinery and tooling and can't do that now.
-->

### Monitoring Requirements

<!--
What dashboards need to be created in Grafana for this enhancement? What alerts
and what Prometheus probes are required to pull metrics? Can CPU and Memory
usage by monitored? Does this tool require throughput and volume monitoring for
network connections and requests?

Can the following stack provide monitoring
Grafana/Prometheus/AppDynamics/Splunk?

Should logging errors be notified as alerts? If so to what team and what errors
should be configured for notification.
-->

#### What are the reasonable SLOs (Service Level Objectives) for the enhancement?

<!--
This is your opportunity to define what "normal" quality of service looks like
for a feature.

It's impossible to provide comprehensive guidance, but at the very
high level (needs more precise definitions) those may be things like:
  - per-day percentage of API calls finishing with 5XX errors <= 1%
  - 99% percentile over day of absolute value from (job creation time minus expected
    job creation time) for cron job <= 10%
  - 99.9% of /health requests per day finish with 200 code

These goals will help you determine what you need to measure (SLIs) in the next
question.
-->

#### What are the SLIs (Service Level Indicators) an operator can use to determine the health of the service?

<!--
Pick one more of these and delete the rest.
-->

- [ ] Metrics
  - Metric name:
  - [Optional] Aggregation method:
  - Components exposing the metric:
- [ ] Other (treat as last resort)
  - Details:

#### Are there any missing metrics that would be useful to have to improve observability of this feature?

<!--
Describe the metrics themselves and the reasons why they weren't added (e.g., cost,
implementation difficulties, etc.).
-->

### Dependencies

<!--
This section must be completed when targeting beta to a release.
-->

#### Does this feature depend on any specific services running in the cluster?

<!--
What are the dependent systems required for this enhancement. Think not only of
services running on Kubernetes but any thirdparty or external service which is
required for the health of the enhancement.

Are the dependencies runtime, deployment time or build time? Are dependencies
specific to the location, would dependencies change based on cloud or ship?
-->

### Scalability

<!--
How will this scale? Will the enhancement scale horizontally or vertically? Is
the scale fixed to a certain amount of requests or users?

Is scalability automated or does it need to be monitored? What are the metrics
that need to be identified to understand if scaling is required?
-->

#### Can enabling / using this feature result in resource exhaustion of resources (PIDs, sockets, inodes, etc.)?

<!--
What resources is the enhancement consuming? CPU, Memory, Storage? Is this a
container or a VM? What would be the impact to other workloads if any resources
are exhausted?

Does the system have the ability to limit the resource consumption if so what
are those gates?

Network is also a resource. If traffic is expected to go across cloud and ship
identified the volume of movement. Also identify any inter system volume that
would cause network resource consumption such as bandwidth.
-->

### Troubleshooting

<!--
The Troubleshooting section currently serves the `Playbook` role. We may consider
splitting it into a dedicated `Playbook` document (potentially with some monitoring
details). For now, we leave it here.
-->

#### What are other known failure modes?

<!--
For each of them, fill in the following information by copying the below template:
  - [Failure mode brief description]
    - Detection: How can it be detected via metrics? Stated another way:
      how can an operator troubleshoot without logging into a master or worker node?
    - Mitigations: What can be done to stop the bleeding, especially for already
      running user workloads?
    - Diagnostics: What are the useful log messages and their required logging
      levels that could help debug the issue?
      Not required until feature graduated to beta.
    - Testing: Are there any tests for failure mode? If not, describe why.
-->

#### What steps should be taken if SLOs are not being met to determine the problem?

<!--
For any SLO defined what is the playbook that is required to be executed when
it is breached? Are SLI's notifying of these breaches and can the playbooks be
automated?
-->

## Implementation History

<!--
Major milestones in the lifecycle of a DEP should be tracked in this section.
Major milestones might include:
- the `Summary` and `Motivation` sections being merged, signaling SIG acceptance
- the `Proposal` section being merged, signaling agreement on a proposed design
- the date implementation started
- the first Kubernetes release where an initial version of the DEP was available
- the version of Kubernetes where the DEP graduated to general availability
- when the DEP was retired or superseded
-->

## Drawbacks

<!--
Why should this DEP _not_ be implemented?
-->

## Alternatives

<!--
What other approaches did you consider, and why did you rule them out? These do
not need to be as detailed as the proposal, but should include enough
information to express the idea and why it was not acceptable.
-->

## Infrastructure Needed (Optional)

<!--
Is new infrastructure needed for this enhancement or can this run on current
system? What type of infrastructure is needed, additional resources for
containers, new VM's? Are the VM's Linux or Windows? Does this enhancement
required dedicated CPU and Memory in large quantities?

Can this be deployed to existing Cloud (AWS)?
-->
