# Changelog

All notable changes to the VDA-MD Framework are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [4.1.0] — 2026-04-28

Documentation accuracy corrections. No architectural or capability changes from V4.0.

### Changed
- **Section 8.1 — credential signing description.** Previous text described signing as "HMAC-SHA256, server-side secret." Corrected to Ed25519Signature2020 via `@digitalbazaar/ed25519-signature-2020` (asymmetric key pair, no shared secret, conformant with W3C VC Data Model v1.1). The previous wording was a documentation error; the implementation has always used Ed25519.
- **Section 8.1 — credential TTL and rotation cycle.** Previous text conflated TTL ("23 hours after issuance") with rotation ("Automatic rotation cycle"). Corrected: credentials carry a 24-hour TTL; rotation runs every 23 hours so credentials rotate before expiry.
- **Section 13 numbering.** Subsections previously labelled 12.1 through 12.4 renumbered as 13.1 through 13.4 to match the parent section.
- **Scope terminology.** Replaced mixed uses of "POC" and "functioning platform" with "functioning proof-of-concept platform" throughout Sections 12.3 and 14.
- **Document classification.** Updated from "Confidential" to "Public — Creative Commons Attribution 4.0" to reflect publication intent.

### Added
- **Section 8.3 — transport boundary statement.** New sentence clarifying that the credential is transmitted as a base64url-encoded VC JSON payload in the Bearer header, that this is a non-standard transport chosen for internal platform-managed agent use, and that cross-party VC exchange scenarios would use a Verifiable Presentation envelope (out of scope for the current deployment).
- **Appendix A — glossary entries.** New entries for `Ed25519Signature2020` and `Verifiable Presentation (VP)`. Updated `Verifiable Credential (VC)` entry to include signing suite and TTL/rotation detail.
- **Appendix B — W3C VC standards reference.** Rewritten to cite Data Model v1.1 explicitly, name the Ed25519Signature2020 signing suite, and document the base64url bearer transport scope.
- **Appendix C — Live Platform Demonstration.** New section describing the functioning proof-of-concept platform (citizenM hotels on the Apaleo PMS).
- **Appendix D — Changelog.** This changelog.

### Moved
- **Live demo URL.** Previously on the cover page; relocated to Appendix C with a fuller description of what the demonstration exercises. The GitHub repository URL now appears on the cover and in header metadata.

### Unchanged
- Core architecture (Sections 2-7)
- C2MD methodology (Section 4)
- Customer journey model (Sections 5-6)
- A2A Protocol specification (Section 9)
- Onboarding Agent workflow (Section 10)
- Witness Agent event taxonomy (Section 11)
- GDPR / EU AI Act compliance mapping (Section 12)
- Competitive positioning (Section 15)
- Implementation roadmap (Section 16)

## [4.0.0] — 2026-04 (prior release)

Introduced four new capability layers:
- Cryptographic agent identity via W3C Verifiable Credentials
- A2A Protocol interoperability for external agent integration
- Self-governing Onboarding Agent with a 7-phase admission workflow
- Witness Agent governance expansion with categorised events and 6-hour integrity checks

See the V4.0 whitepaper (archived) for full detail.

[4.1.0]: https://github.com/mikerawsonnz/vda-md-framework/releases/tag/v4.1.0
[4.0.0]: https://github.com/mikerawsonnz/vda-md-framework/releases/tag/v4.0.0
