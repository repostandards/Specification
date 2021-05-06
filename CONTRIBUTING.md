# Contributing to the Repository Specficiation

Thank you for taking the time to contribute to a standard from the Repository Standards Consortium! We are an open-source standards body for novel implementations of APT (such as for jailbroken iOS devices). These guidelines help us organize standards such that anyone, no matter their background, can contribute and support open standards.A

## Key Ideas

When proposing any changes to a specification, we have three core tenets we strive to uphold:

- **Developer Friendliness:** The specification should put as little burden on repositority and package manager developers as possible. Standards will be implemented by multiple different parties and should be:
   - Unambiguous
   - Simple
   - Open

- **Backwards Compatibility:** Don't break stuff. Changes should try to maintain compatibility with previous iterations of both previous standard versions and historical specifications.

- **Thoughfulness:** Don't propose random stuff. Proposals should be crafted with care, solve a problem in the current specification(s), and beneift multiple parties.

## Repo Structure

This specification is split up into three sections: [*Active*](Active/), [*Deprecated*](Deprecated/), and [*Discontinued*](Discontinued/). These folders contain specification features that are currently in use, deprecated and being removed on their specified date, and features that no longer exist.

In each folder is a Markdown file containing the following content that explains the specification. Please keep to this general structure:

```md
# Feature Name

---

* Authors: Author 1, Author 2

*After review, add these fields as necessary*

* Approvers: Approver 1, Approver 2
* Implementation Date: **N/A**
* Replaces Proposal Feature: **Feature**
* Replaces Proposal Deprecation Date: **N/A**

---

## Proposal
Describe your solution here. Be sure to include as much detail as possible and explain any older features that this would be replacing/deprecating.

## Viable Alternatives
Discuss any alternatives to your solution that you may have considered here. Be sure to describe why the approach proposed above is the best option compared to alternatives.
```