# Contributing

This document describes the Intercognitive Foundation's default collaboration process for open standards work.

Individual repositories may add more specific contribution rules. When they do, follow the repository-local guidance first.

## Repository Roles

The Intercognitive GitHub organization should separate current reality from aspiration:

- `profile/README.md` describes what the Foundation is and where builders should start today.
- `CONTRIBUTING.md` describes how contributors should propose and discuss standards.
- Canonical implementations should stay in their originating repositories unless Intercognitive explicitly maintains a reference implementation.

## Intercognitive Open Standard Proposals

Standards are proposed as **IOSPs: Intercognitive Open Standard Proposals**.

An IOSP is a public, versioned proposal for a protocol, interface, data format, conformance requirement, or shared infrastructure standard for physical AI and machine networks.

An IOSP is not an Intercognitive Open Standard. It becomes a standard only after review and acceptance.

## Maturity Stages

Intercognitive standards move through visible maturity stages:

```text
Idea -> Draft IOSP -> Candidate IOSP -> Accepted IOS -> Recommended IOS -> Deprecated
```

| Stage | Meaning |
| --- | --- |
| **Idea** | A problem, opportunity, or interoperability gap has been raised, but no formal proposal exists. |
| **Draft IOSP** | A written proposal exists and is open for discussion. |
| **Candidate IOSP** | The design is stable enough for implementation trials and conformance work. |
| **Accepted IOS** | The Foundation recognizes the proposal as an Intercognitive Open Standard. |
| **Recommended IOS** | The standard has multiple implementations, conformance evidence, and real-world adoption. |
| **Deprecated** | The standard is obsolete, superseded, or no longer recommended for new work. |

## How Standards Are Proposed

Start with an issue or discussion before opening a proposal pull request. The goal is to make the problem clear before polishing the solution.

A new IOSP should have a champion: a person or member organization responsible for shepherding the proposal through discussion, revision, and implementation feedback.

Each proposal should include:

- Title and short summary
- Champion and interested implementers
- Problem statement
- Scope and non-goals
- Terminology
- Proposed protocol, API, data model, or conformance requirement
- Security, privacy, and safety considerations
- Interoperability requirements
- Backward compatibility and migration notes, if relevant
- Reference implementations or known implementation plans
- Conformance tests, validation tools, or test vectors, if available
- Open questions

When a dedicated standards repository exists, proposal files should use stable names such as:

```text
iosp/0001-universal-machine-time.md
iosp/0002-machine-identity.md
```

## How Standards Are Accepted

Intercognitive uses the principle of **rough consensus and running code**.

Consensus does not require unanimous approval. It does require visible discussion, serious objections being addressed, and no unresolved blocking concerns from the maintainers responsible for the standard area.

An IOSP can become an **Accepted IOS** when it has:

- A clear, reviewable specification
- Public discussion and revision history
- Rough consensus among participating members and maintainers
- Security, privacy, and safety considerations documented
- At least one working implementation or credible implementation trial
- A maintainer or working group willing to steward the standard

An Accepted IOS can become a **Recommended IOS** when it has:

- Two or more independent implementations, preferably from different organizations
- Conformance tests, validators, test vectors, or equivalent verification artifacts
- Evidence from a real-world deployment, pilot, or integration
- A versioned release of the specification
- Clear guidance for implementers

## Canonical Implementations

Intercognitive should not fork member repositories only for discoverability.

Instead:

- Use Intercognitive repositories for standards, registries, conformance tools, and true reference implementations.
- Link to canonical implementation repositories owned by member organizations.
- Fork only when Intercognitive is actively maintaining a variant, reference implementation, integration branch, or archival mirror with a clear purpose.

Examples of canonical ecosystem repositories:

- [`aukilabs/auki-sdk`](https://github.com/aukilabs/auki-sdk)
- [`peaqnetwork/Universal-Machine-Time-UMT`](https://github.com/peaqnetwork/Universal-Machine-Time-UMT)

## Pull Requests

Pull requests should be focused and reviewable.

For documentation and standards work:

- Explain why the change is needed.
- Link related issues or discussions.
- Keep terminology consistent with existing Intercognitive language.
- Update the README when contributor-facing entry points change.
- Prefer small, coherent changes over broad rewrites.

Commit messages should be clear and follow Conventional Commits where practical, such as:

```text
docs: add IOSP contribution process
docs: clarify canonical implementation policy
```

## AI Agents and Automation

AI agents may help draft, edit, and review Intercognitive materials, but should not resolve governance ambiguity on their own.

When in doubt:

- Surface the ambiguity.
- Propose the issue, question, or follow-up task.
- Ask before creating issues, changing process, moving project-board cards, or asserting a standard has advanced maturity stage.

Standards work depends on trust. Process changes should be explicit, reviewed, and easy for humans to audit.
