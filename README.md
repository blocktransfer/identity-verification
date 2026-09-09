# Identity Verification

An open identity-verification to support client onboarding through SEP-12 and explore decentralized identity-data infrastructure shared across transfer agents.

## Status

Work in progress.

## Purpose

The goal is to develop an open platform for collecting and reviewing the identity information needed during investor onboarding, with a longer-term direction toward distributed, community-operated infrastructure. Publishing the implementation will allow others to inspect how the platform works and contribute improvements.

The project supports the identity-verification process described in [BlockTransfer’s AML policy](https://www.blocktransfer.com/compliance/user/aml-policy.html). That policy describes the broader operational process; this repository tracks the software being developed to support it.

## Decentralization direction

The [TAD3-protocol issue](https://github.com/blocktransfer/TAD3-protocol/issues/11#issue-5190005279) completes a SEP-12 server with exploring a uniform DRS Database. It describes a separate registration-system project as a proving ground for distributed, Storj-like community peers, encryption at rest, and potential issuer and transfer-agent access through class-based controls.

This project shares that direction: explore how identity information could be held across community-operated peers and made available to authorized issuers and transfer agents. Decentralizing storage is intended to preserve the privacy of identity records, not make them public.

Peer operation, encryption, key management, and access controls remain design questions. The issue’s suggestion of homomorphic encryption is an avenue for investigation, not an implemented capability or a settled design.

That bit is in flux re [JW Agenda#24](https://github.com/JFWooten4/agenda/issues/24) per the NMS CAT DB precedent.

## Stellar integration

SEP-12 defines a standard API for exchanging customer KYC information between clients and services. It is the intended integration standard for this project.

[Protocol specification](https://github.com/stellar/stellar-protocol/blob/master/ecosystem/sep-0012.md)

## Initial development priorities

- Define the onboarding workflow and required identity information.
- Design the SEP-12 integration and customer review process.
- Explore distributed storage and issuer and transfer-agent access for a uniform DRS Database.
- Document access controls, data retention, and deletion behavior.
- Add an implementation, tests, and local setup instructions.

These are proposed development priorities, not completed capabilities.

## Privacy

See [BlockTransfer’s privacy policy](https://www.blocktransfer.com/compliance/user/privacy-policy.html) for information about how BlockTransfer collects, uses, and shares personal information, and how to contact us about privacy requests.

## Contributing

Early contributions can help clarify requirements, evaluate implementation approaches, and improve the documentation. Open an issue to discuss substantial changes before beginning implementation.

See [Inspirations](Inspirations.md) for projects collected as references. Their inclusion does not imply an integration or dependency.

Use synthetic identity information in examples, fixtures, and public discussions. Do not submit real identity documents or personal information to this repository.
