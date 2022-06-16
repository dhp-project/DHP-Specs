# Specification Governance
## Draft 01

# Authors

1. Ravi Prakash : ravi@becknfoundation.org

# Latest Version
Draft 01

# Previous Versions
None

# Scope

This document intends to establish processes and guidelines which build a transparent, open mechanism for deciding how to manage contributions to the DHP specification. The DHP Working Group will initially follow these processes when merging changes from external contributors or from the DHP Working Group itself. This guideline document will be adjusted as practicality dictates.

This document is intended for the following audience.

1. Anyone who wants to understand how contributions are reviewed and merged by the DHP Working Group


# Prerequisites

1. Readers must have a working knowledge of git
2. Readers should also know how open-source repositories are managed on Github.
3. Readers must have knowledge and understanding of DHP specification

# Context

DHP exists as a set of public repositories on Github at https://github.com/dhp-project. These repositories contain specification documents, reference implementations, tools and utilities. Like all version controlled open-source repositories, there are processes that must be adopted to manage changes to the files present in these repositories. The most common way a change is proposed to the specification is via an Issue linked to that repository which ultimately gets converted to a Pull Request linked to that Issue. These pull requests must then be reviewed by the maintainers of the repository and subsequently merged with the main / master branch of that repository. 


# Abstract 

The evolution of DHP specification is always use-case driven. The DHP Working Group can specify support for hypothetical use cases as they see fit, but the specifications should be backed by realistic scenarios. Management of contributions towards an open-source specification like DHP are governed by well defined policies and processes. These processes will evolve just like the specification does, based on use cases. Given beckn is designed to be a global protocol, maintainers and committers must be aware any change committed to the specification has a global impact on implementation. Therefore, the governance model of DHP specification is based on strict and unambiguous design principles described in this document.  Anyone reviewing pull requests must apply these principles on each suggested change and decide if a change is deemed worthy of inclusion into the specification. The methodologies, guidelines and processes of conducting working group meetings to review contributions made to the specification is described in this document.


# Terminology

1. **Git:** A decentralized version control software
2. **Github:** An online platform for managing shared repositories via git
3. **Pull Request:** A request to merge a change to an existing version of the repository
4. **DHP Working Group:** Current maintainer and governing authority of the DHP specification


# Expected Outcomes after reading this document

After reading this document, the reader should be able to

1. Understand how to review and merge changes to the specification

# Introduction

DHP is maintained via an open community-driven governance model. The community comprises multiple businesses and organizations that actively contribute to the specification to fuel their digital acceleration. This collaboration across domains, technologies and expertises will bring in new ideas which need to be part of the protocol. Hence there is a need for a standardised process for making relevant changes to the specification as well and for a retrospective understanding of the specification. The governance model for DHP has been created using some of the best practices of globally recognized governance models.

Evolution of DHP specification is guided by the **DHP Working Group**. This working group contains members that bring their API expertise, industry knowledge, incorporate feedback from the community, and expand the group of committers as and when appropriate. All development activity on the future specification will be performed as features on a draft branch and merged into this branch. Upon release of the future specification, this branch will be merged to master.

The DHP Working Group holds weekly web conferences to review open pull requests and discuss open issues related to the evolving specification. Participation in weekly calls and scheduled working sessions is open to the community. 

This governance model is inspired from the [DHP Governance Model](https://github.com/beckn/protocol-specifications/blob/master/GOVERNANCE.md).


# The DHP Credo

The DHP community is an open community. So, no registrations. No memberships. No partnerships. Just a minimal footprint of an open and equally accessible DHP that anyone can use. Multiple businesses and organizations have started using DHP to fuel their digital acceleration. The credo of being an open protocol creates a level-playing field for any market player, small or large.


## Motivation

To make the internet small-business friendly. be a force multiplier with minimal footprint.

## Guiding Lights

Open specs, equal access. retain agency of small businesses. non-rivalrous, non-exclusive networks

## Community Driven

Increase value for all participants. be a network weaver in your own way. be a contributor of specs and best practices

DHP is an open health and wellness protocol with an generic core, which is enabling governments and market players to reimagine building seamless digital experiences and networks in the field of health and wellness. This is very similar to how HTTP, while being a simple and open protocol has fueled seamless interaction between multiple systems and led to an explosive growth in internet adoption.

## Open Community Contributions

The DHP Specification has been accepting community contributions to the specification since Feb 2022.

# Design Principles

To allow open contributions from the community, a governance model is required to apply some basic design principles while reviewing or proposing changes to the specification. They are:

## Interoperability via Abstraction:
Any feature included in the specification must be sufficiently abstracted so as to allow it to be consumed across a global range of use cases. That means no feature should be linked to a specific domain, region or use case. 

## Optimal ignorance:
Before including any feature in the specification, reviewers should ask the following questions: a) _Do we need it?_ And, b) _Do we need it now?_ If the answer to both these questions is “Yes” then this criteria will have been met.

## Privacy and Security
Any feature being included in the specification must be tested for any security or privacy vulnerabilities. Free text fields, loosely-typed fields and any fields that may be used to implicitly capture Personally Identifiable Information should not be accepted.

## Scalability

Any feature being included in the specification must be tested for scalability. String fields with unlimited size; arrays with unlimited size etc, must be discouraged. Any feature that is included must work at scale.

## Reusability
Any new feature must be checked if it can reuse components from the existing schema before inclusion into the specification.

## Unification over Standardization
Not all features across the globe can be standardized. Standard values vary with domain, region and adoption. In case multiple standards are being adopted for a single feature, it is recommended that both the standards are included in the feature instead of proposing a new standard. For example, if a Location schema is defined using gps and address, then the feature should include both gps and address instead of choosing one over the other. Standardization should occur as a natural consequence of market adoption rather than a forced adoption. 

There will be exceptions to the above principles. The objective of the DHP Working Group is to address such exceptions and define the most logical way forward to include such exceptions. 

# Need for Governance

Since the core specification is essentially abstracted, the implementers of the specification must use instances of the core specification for various domains, regions and scope. Moreover, the DHP specification is built by applying policies on the core specification. Hence, there is a need for a strong and inclusive governance model that adheres to the basic design principles while simultaneously being inclusive in its approach to evolution as opposed to a foundation-controlled evolution.


# Areas That Require Governance

There are many independently governable specification elements in the DHP. These elements are called areas. Each area will have multiple working groups under it. The following are the areas currently identified :


* **API** : Core API and schema definitions
* **Taxonomy** : Domain-specific repositories for organization of taxonomies and taxonomy element definitions
* **Certification** : Certification and compliance rules and specifications
* **Architecture** : High level architecture definition and definitions of the various components in the network
* **Network Security** : Network security protocols and best practices
* **Policy** : Governance structures, licences and copyrights
* **Missions** : Specific implementation related working groups


# Working Groups (WG)

A Working Group is a collection of people who collaborate on, and are responsible for managing evolution of the DHP specification. 

## Working Group Structure

Each WG has the following structure

1. Administrators
2. Community Managers
3. Core Committers
4. Implementation Specialists
5. Technical Writers

### Administrator

Each WG will have one Administrator (Admin). The Admin will be responsible for declaring a rough consensus on any decision the group has to make. Having full consensus is preferred but not required. During a decision process if the Admin decides that the issues brought forward have been discussed enough and the group has made an informed decision, the Admin can declare that there is rough consensus to go ahead with the decision. For assets (github repository, document collections, group email id etc) coming under each WG, the Admin will have access to modify it.

### Community Manager


### Core Committers

Each WG will have at least one committer. The purpose of the committer is to review PRs against WG guidelines and design principles and post comments on Github regarding the status of the PR. 



# Managing Specification Evolution

The specification will evolve over time. Changes may be made when any of the following criteria are met:

1. **Clarity**. The current "way" something is done doesn't make sense, is complicated, or not clear.
2. **Consistency**. A portion of the specification is not consistent with the rest, or with the industry standard terminology.
3. **Necessary functionality**. We are missing functionality because of a certain design of the specification.
4. **Forward-looking Designs**. As usage of APIs evolves to new protocols, formats, and patterns, we should always consider what the next important functionality should be.
5. **Impact**. A change will have an impact on a large number of use cases. We should not be forced to accommodate every use case. Maintainers should strive to make the common and important use cases both well supported and common in the definition of the OAI Spec. We cannot be edge-case driven.

# Specification Review Guidelines

While reviewing each change in the specification committers should always consider the following in addition to the design principles:

1. **Migration Impact**: Is this a construct that has a smooth implementation path from the latest specification? If so, how complicated is it to migrate implementations to the proposed change? Secondly, how large of a cohort is affected due to this change
2. **Tooling**: Contributors should strive to support code generation, software interfaces, spec generation techniques, as well as other utilities. Some features may be impossible to support in different frameworks/languages. These should be documented and considered during the change approval process.
3. **Visualization**: Can the specification change be graphically visualized somehow in a UI or other interface 

Spec changes should be approved by a majority of the committers. Approval can be given by commenting on the issue itself, for example, "Approved by @DHP Working Groupadmin" however at least one formal GitHub-based flow approval must be given. After the voting criteria is met, the WG Admin can merge or assign a member to merge the PR. No change should be approved until there is documentation for it, supplied in an accompanying PR.

# Feature Evolution

All new features have a life cycle starting from a proposal to a required standard. All new features to the specification must start with a status as “proposed”. Upon review, the DHP Working Group will decide to move forward with a discussion on the change and then move it to a “draft” status. If the feature is considered to become part of the specification, it will be moved to the “recommended” status. And if the feature is widely accepted and adopted by the ecosystem, then it will be moved to a “required” status after which it will become part of the core specification.


All proposals to the specification are submitted as namespaced properties as mentioned in CONTRIBUTIONS.md. The working group has the responsibility of reviewing these proposals and classify them accordingly as draft, recommended, required or not-recommended features. Once classified, the WGs must rename the namespace with the appropriate feature stage component after review.  


## Proposal

A proposal is a request to update the specification to support a specific use case or to resolve a bug in the specification. These proposals can be in the form of github discussions, issues or markdown files submitted as PRs into the protocol-specifications/docs/proposals folder. They are unstructured and typically contain informal language. 


## Protocol Drafts

Protocol drafts are formal documents created by the core committers that have been drafted from one or more proposals. They must necessarily contain the name of the proposer in the Authors and must contain links to all external references and uploaded to the protocol-specifications/docs/proposals folder as an RFC. 

## Recommended Standard
These are formal documents that have been selected from the protocol drafts and have been included into the specification. They are found in the protocol-specifications/docs/protocol-standards/recommended folder. These are recommendations made by the DHP Working Group for implementers. They are not mandatory to be implemented but it is a good idea to implement DHP according to these specifications. 


## Required Standard
These are formal documents that have been selected from the protocol drafts and have been included into the specification. They are found in the protocol-specifications/docs/protocol-standards/required folder. They are mandatory to be implemented by all implementers. 

### Not Recommended
These are proposals and protocol-drafts that have been rejected by the DHP Working Group and are not recommended to be implenented by DHP implementers. 


# Working Group Weekly Meetings

To review change requests to the specification, The DHP Working Group conducts weekly calls. All meeting recordings and decks can be accessed [here](https://github.com/dhp-project/DHP-Specs/discussions?discussions_q=label%3Ameeting)

# Change Tracking and Management

**GitHub** is the medium of record for all spec designs, use cases, and so on.

All the specification documents are present on the official DHP Github account [here](https://github.com/dhp-project/DHP-Specs).


## Sources of Truth

1. The **protocol-specifications** repository is the source of truth for the core transaction API specification. 


## Branch Structure

At any given time, there should be _at most_ 4 working branches. The branches would exist if implementation has started on them. For example, assume a current version of **0.9.2** in the protocol-specifications repository. 

1. **master** - Current stable version. No PRs should be accepted directly to modify the specification. PRs against supporting files can be accepted.
2. **draft** - The working draft branch the specification. 

The main branch shall remain the current, released DHP specification. The will describe and link the working branch(es) on the default README.md on main.

Examples of how something is described _currently_ vs. the proposed solution should accompany any change proposal.

Use labels for the workflow of specification changes. Examples of labels are _proposed_, _draft-*_, _recommended_, _required_-, _not-recommended_, _review_ (candidate for upcoming WG meeting), _rejected_, and _needs-approval_. These labels must be assigned by WG members. Style is lowercase with dashes in place of spaces.

An issue will be opened for each feature change. Embedded in the issue, or ideally linked in a file via pull-request (PR), a document about use cases should be supplied with the change.

A PR will be used to describe the _proposed_ solution and linked to the original issue.

Not all committers will contribute to every single proposed change. There may be many open proposals at once, and multiple efforts may happen in parallel.

When the work branch is ready and approved, the branch will be merged to main.


## Reviewing Pull Requests

Any Pull Request must have an associated Issue. If an Issue is not present, the reviewer must post a comment on the PR comment section asking the contributor to Raise an Issue and link the PR to it. If an Issue is not raised within 24 hours, the PR should be considered as rejected and must be closed by the reviewer with the comment _“Closing this due to unlinked Issue”_


## Managing Conflicts

If a Pull Request causes a merge conflict, the reviewer should respond with a comment “Merge conflicts present, kindly resolve and re-submit PR”. If the merge conflict is not resolved within 24 hours, the PR should be considered as rejected and must be closed by the reviewer with the comment “_Closing this due to unresolved merge conflicts_”


# Release Process

A release requires a vote on the release notes by DHP Working Group members within the voting period. Major or minor release voting periods will be announced by the DHP Working Group admin in the Slack channel and noted on the calendar at least 6 days in advance. During this time, DHP Working Group members who have not yet voted must note their approval on the GitHub pull request for the release notes. Patch releases must happen at the first DHP Working Group meeting of a calendar month. The admin is responsible for coordinating the actual merge to main with marketing support, if any.

* Patch-level releases require majority approval by WG members. (Max voting period 3 days)
* Minor: requires approval by 66% of WG members. (Max voting period 7 days)
* Major: requires approval by 66% of WG members. (Max voting period 14 days)

The above policies apply to the DHP Working Group. However, a WG Admin may override the majority percentage and voting period depending on the area and size of the group.

# Transparency

The process should be as transparent as possible. Sometimes there will be discussions that use customer names, sensitive use cases, and so on. These must be anonymized, discussed in a private repository, or conducted offline. General discussions should happen on the GitHub issues for this project.


# Participation

While governance of the specification is the role of the DHP Working Group, the evolution of the specification happens through the participation of members of the developer community at large. Any person willing to contribute to the effort is welcome, and contributions may include filing or participating in issues, creating pull requests, or helping others with such activities.
