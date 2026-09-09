# Identity Verification

An open identity-verification project initiated by BlockTransfer, intended to support client onboarding through Stellar’s SEP-12 KYC API and explore decentralized identity-data infrastructure shared across transfer agents.

## Status

Work in progress. This repository currently contains project documentation and a license. It does not yet include an application, a working SEP-12 service, or deployment instructions.

## Purpose

The goal is to develop an open platform for collecting and reviewing the identity information needed during investor onboarding, with a longer-term direction toward distributed, community-operated infrastructure. Publishing the implementation will allow others to inspect how the platform works and contribute improvements.

The project is intended to support the identity-verification process described in [BlockTransfer’s AML policy](https://www.blocktransfer.com/compliance/user/aml-policy.html). That policy describes the broader operational process; this repository tracks the software being developed to support it.

## Decentralization direction

The third paragraph of TAD3 protocol issue #11 connects completing a SEP-12 server with exploring a uniform DRS Database. It describes a separate registration-system project as a proving ground for distributed, Storj-like community peers, encryption at rest, and potential issuer and transfer-agent access through class-based controls.

https://github.com/blocktransfer/TAD3-protocol/issues/11#issue-5190005279

This project shares that direction: explore how identity information could be held across community-operated peers and made available to authorized issuers and transfer agents. Decentralizing storage is intended to preserve the privacy of identity records, not make them public.

Peer operation, encryption, key management, and access controls remain design questions. The issue’s suggestion of homomorphic encryption is an avenue for investigation, not an implemented capability or a settled design.

## Stellar integration

SEP-12 defines a standard API for exchanging customer KYC information between clients and services. It is the intended integration standard for this project. SEP-12 support has not yet been implemented here.

Protocol specification:

https://github.com/stellar/stellar-protocol/blob/master/ecosystem/sep-0012.md

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

## License

GNU Affero General Public License v3.0. See [LICENSE](LICENSE) for the full terms.
