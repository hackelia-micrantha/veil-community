# Research directions

Veil studies reversibility, visual transformation, and information carrying capacity. The research is exploratory; these references do **not** imply implementation, endorsement of a particular algorithm, security approval, or reproduction of the authors' results.

## Questions we want evidence for

| Area | Research question | Evidence needed |
| --- | --- | --- |
| Exact recovery | Can an altered artifact support restoration of the original encoded file bytes, not just visually similar pixels? | Byte-for-byte round trips, tampering rejection, explicit failure cases |
| Carrier capacity | How much authenticated recovery material can a viewable image or readable text actually carry? | End-to-end payload/size comparisons including metadata and cryptographic overhead |
| Robustness | Which normal user operations preserve recovery? | Format and platform compatibility matrix; crop, resize, recompression, Unicode and edit tests |
| Confidentiality | What does possession of the carrier reveal without the key? | Separately reviewed cryptographic and leakage analyses; no claims based only on appearance |
| Human usability | Is the result understandable, accessible, and easy to share correctly? | Realistic user tasks, clear key handling, manual accessibility review |
| AI-assisted encoding | Do model-derived choices improve capacity or presentation enough to justify their cost? | Reproducible comparisons, bounded compute, failure and privacy analysis |

## Selected external reading

These publications are **independent research**, not Veil specifications or claims of successful product integration.

### Image information hiding

- [FlexMark: Adaptive Watermarking Method for Images (ACM MMSys 2024)](https://www.cs.sfu.ca/~mhefeeda/Papers/mmsys24_flexmark.pdf) — prompts questions about adaptive image regions and watermark capacity. Watermark detection is not equivalent to encrypted full-file recovery.
- [Learning Robust Image Watermarking with Lossless Cover Recovery (ICCV 2025)](https://openaccess.thecvf.com/content/ICCV2025/html/Chen_Learning_Robust_Image_Watermarking_with_Lossless_Cover_Recovery_ICCV_2025_paper.html) — connects reversibility with robustness. Recovering a visual cover is not automatically the same as recovering every original encoded-file byte.
- [We Can Hide More Bits: The Unused Watermarking Capacity in Theory and in Practice (2025)](https://arxiv.org/abs/2510.12812) — explores capacity trade-offs; reported bit accuracy or theoretical capacity does not establish authenticated recovery of a complete encrypted file.

### Linguistic information hiding

- [STEAD: Robust Provably Secure Linguistic Steganography with Diffusion Language Model (NeurIPS 2025)](https://proceedings.neurips.cc/paper_files/paper/2025/hash/3d03800841fa1bb2f43ef1750aafcce4-Abstract-Conference.html) — addresses text-carrier robustness under specific model and edit assumptions. Its security properties should not be confused with Veil's confidentiality or exact-message recovery requirements.

## How to evaluate a paper

A useful contribution identifies the precise research claim, tested conditions and limitations, relevant threat model, and what an independent experiment could disprove. Distinguish **bit accuracy** from **whole-message success**, **pixel fidelity** from **original-file identity**, and **formal security under a model** from real-world deployment security.

For a new paper, use a public issue with its DOI/publisher URL, a short summary in your own words, the specific Veil use case, and a testable question. Do not copy paywalled papers, copyrighted figures, internal research notes, or unpublished implementation details.

See [Product direction](PRODUCT.md) and [Community participation](COMMUNITY.md).
