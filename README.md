# Veil Community

**Image obfuscation today. Research into key-controlled, reversible media tomorrow.**

Veil explores ways to transform images and text for creative presentation and selective disclosure. Its existing artistic image workflow makes photographs visibly different using a Voronoi-style treatment. Research is exploring whether an encrypted original can eventually travel with a transformed image—or be represented through abstract text—and be restored only by someone holding the necessary key.

This is Veil's **public product, research, and community interface**. The implementation, unpublished engineering work, and release decisions remain outside this repository. Public discussion or a prototype does not imply that a feature is available, audited, or fit to protect sensitive data.

## Capabilities and status

| Area | Current status | What this means |
| --- | --- | --- |
| Artistic image obfuscation | Implemented in Veil's private project | Produces a visibly altered, lossy image. It is **not** a guarantee of anonymity or irreversible removal of sensitive information. |
| Reversible image protection | Experimental; not a supported public release | Browser-local prototypes exercise a separate key and encrypted recovery of original image bytes. Cross-platform, security, and release acceptance remain outstanding. |
| Recovery data inside an ordinary viewable image | Research | Investigating whether a self-contained altered image can carry enough authenticated recovery data without a companion archive. No supported format or durability guarantee. |
| Text analysis and reversible text transformations | Experimental research | Exploratory interfaces/codecs are not encryption or an independently supported text product. |
| Encrypted abstract text | Research | Investigating whether a readable, abstract message can represent encrypted text and allow exact authenticated restoration. Not available as a released feature. |
| AI-assisted region selection | Proposed | Exploring opt-in, selective image treatments; no claim of a production-ready detector or privacy classifier. |
| Hosted API and commercial tiers | Discovery | Free, voluntary supporter/beerware, and paid service concepts are being evaluated; no pricing, quotas, SLA, or paid access promise is made here. |

**Availability:** This repository currently publishes documentation and community guidance only. It does not distribute a verified public demo, installable release, or supported API endpoint. The artistic image capability exists in Veil's private implementation; public access should not be inferred from its implemented status. See [Community participation](docs/COMMUNITY.md) to share a use case or request availability updates.

**Important:** Visual distortion is not the same as redaction, anonymization, or confidentiality. Exact restoration requires more than recognizable visual similarity. Published encryption, privacy, and recovery claims will require separately qualified evidence.

## Explore

- [Product and use cases](docs/PRODUCT.md) — the practical problems and boundaries Veil is investigating.
- [Research directions and reading](docs/RESEARCH.md) — research questions, selected external publications, and evaluation criteria.
- [Community participation](docs/COMMUNITY.md) — how to suggest a use case, contribute a reference, or report a reproducible product problem.
- [Private security reporting](SECURITY.md) — use the GitHub private report option if enabled, or the published Micrantha security contact; never post vulnerability details in public issues.
- [Micrantha contribution guidelines](https://github.com/hackelia-micrantha/.github/blob/main/CONTRIBUTING.md) — shared code of contribution and review practice.

## Who this is for

**Prospective users and teams:** Describe an actual workflow: public image previews, controlled sharing, educational or creative imagery, or text representations that require a separately held key.

**Researchers:** Bring papers, reproducible evidence, threat models, and failure cases involving reversible media, information hiding, coding theory, or semantic text carriers.

**Contributors:** Help clarify documentation, accessibility, interoperability needs, UX expectations, and platform failure modes without needing access to private implementation.

## Repository boundary

This repository is **not** the core source tree, a release/download channel, a cryptographic specification, an API compatibility contract, or a mirror of internal planning. It contains no product credentials, private algorithms, customer data, private test fixtures, or deployment instructions.

A public suggestion does not become an accepted roadmap item until reviewed by the project maintainers. Security-sensitive reports follow the private channel above.

## License and rights

**The existing public-content license is [CC0 1.0 Universal](LICENSE), not CC BY 4.0.** CC0 allows reuse without an attribution requirement and its dedication is intended to be irrevocable. Material made available under CC0 here is subject to the rights its contributors actually hold. Third-party publications remain governed by their own licenses and copyrights. **This does not license Veil's private implementation, patents, trademarks, branding, or future product releases.** A community contribution does not imply acceptance into the product.

Maintained by [Micrantha](https://github.com/hackelia-micrantha).
