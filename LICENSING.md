# Licensing

The VDA-MD framework — methodology, specifications, and reference documentation
in this repository — is published under the
[Creative Commons Attribution 4.0 International License (CC-BY-4.0)](LICENSE).

You are free to use, adapt, build on, and commercialise the framework, including
in proprietary products, with attribution.

## What is and isn't covered by CC-BY-4.0

**Covered (free to use with attribution):**

- The VDA-MD methodology and whitepaper
- The Customer Journey Model and the Universal Horizontal Value Streams
- File-type conventions: `AGENTS.md`, `SOP.md`, `SKILL.md`, `EXCEPTION.md`
- Exception management patterns and YAML-encoded RACI structures
- The POC design, success criteria, and boundary test scenarios
- Glossary, standards anchors, and prior-art statements
- Anything else in this repository at the tagged release version

**Not covered by this licence:**

- The C2MD runtime (private, commercial — see below)
- The A2A Witness enforcement runtime (private, commercial)
- Industry-specific implementation packages (hospitality, financial services, etc.)
- Advisory engagements applying the framework to a specific organisation
- The "VDA-MD" and "C2MD" wordmarks, when used in a way that implies
  endorsement or official partnership

If you implement the framework in your own product, you do not need permission
or a separate agreement — attribution per CC-BY-4.0 is sufficient.

## Attribution

Recommended attribution line:

> Built using the VDA-MD framework by Mike Rawson —
> https://github.com/mikerawsonnz/vda-md-framework (CC-BY-4.0)

If you publish a derivative methodology, please make clear which parts are
your own contribution versus the underlying VDA-MD layer.

## Reference version

This repository is the canonical source. Production implementations should pin
to a tagged release rather than `main`, and should record the commit hash they
implemented against. The current stable release is **v4.1**.

## Commercial extensions

The methodology being free does not mean the runtime is free. The following are
proprietary and available through commercial agreement only:

**C2MD — the runtime that turns VDA-MD specifications into governed behaviour.**
Cloud Run service generating EU AI Act-aligned compliance bundles with
W3C Verifiable Credential signing, multi-IdP token validation, and
A2A JSON-RPC 2.0 integration. Available as a paid product at
[c2md.getvda.ai](https://c2md.getvda.ai).

**Industry implementation packages.** Reference implementations, mappings to
sector-specific standards, and pre-built file sets for hospitality, financial
services, and other verticals — built and maintained as commercial deliverables.

**Advisory engagements.** Direct work applying VDA-MD to a specific
organisation, including governance review, framework extension design,
implementation guidance, and review of derivative methodologies.

For any of the above, contact **mike@getvda.ai**.

## Trademarks

"VDA-MD" and "C2MD" are used as descriptors of this open framework and the
associated commercial runtime, respectively. Nominative use ("compatible with
VDA-MD," "uses C2MD") is fine. Use that implies official endorsement,
partnership, or certification ("VDA-MD Certified," "Official C2MD Partner")
requires written permission.

## Security disclosures

Security issues affecting either the framework documentation or commercial
runtime should be reported to **security@getvda.ai**.

---

*Maintained by Mike Rawson. Questions about commercial engagement:
mike@getvda.ai.*
