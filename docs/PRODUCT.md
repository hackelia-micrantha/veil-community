# Product direction and use cases

Veil's central distinction is between **changing what people see** and **controlling what someone can recover**. These are separate requirements with separate security properties.

## What exists

The existing artistic image workflow applies a Voronoi-style transformation to produce a visibly altered image. It is useful as a creative treatment or altered preview. It is **not** designed to prove that subjects, locations, or other sensitive attributes can no longer be inferred.

No supported public key-controlled recovery, confidential text steganography, or automatic sensitive-object classification is declared by this repository.

## What is being explored

### 1. Reversible image sharing

**Scenario:** An illustrator or publisher wants an altered preview for a public discussion, while a separately authorized recipient needs access to the exact original file.

**Target behavior:** Produce a useful transformed visual representation and independently authenticated encrypted recovery material. A recipient with the appropriate key could restore the original bytes; wrong keys and modified carriers must fail safely.

**Open questions:** How large can the carrier become? What happens after resizing, metadata removal, recompression, cropping, or platform re-encoding? Is the encrypted recovery material actually bound to the intended visible image? Is a self-contained image preferable to a companion container? These are research and qualification questions, not support guarantees.

### 2. Abstract encrypted text

**Scenario:** A writer wants to publish an abstract or metaphorical message that represents another text, recoverable by someone holding a separate key.

**Target behavior:** Convert original text to authenticated ciphertext, encode it as a readable carrier, and reproduce the exact original text on successful verification. A readable carrier alone must not be mistaken for confidentiality.

**Open questions:** Capacity, naturalness, deterministic decoding, edits and typography, Unicode, size expansion, cost, and robustness. Language-model fluency does not imply accurate recovery or cryptographic security.

### 3. Selective visual transformation

**Scenario:** A creator wants to choose areas of an image for stronger or weaker visible alteration.

**Target behavior:** Potential opt-in semantic assistance alongside manual controls.

**Boundary:** A detection model can miss faces, text, reflections, background context, or other sensitive cues. AI-assisted selection would not itself constitute proven anonymization or safe permanent redaction.

## What Veil is not promising

- No protection against recognizing a person or scene solely because an image looks abstract.
- No key recovery, escrow, DRM, or confidentiality promise from the artistic image output.
- No recovery guarantee after arbitrary file edits, social-media processing, or lossy re-encoding.
- No claim that generated text is undetectable steganography, naturally authored, or resilient to paraphrase.
- No production availability, pricing, platform support, or SLA for the experimental capabilities described above.

## Customer feedback

Specific real-world requirements are more actionable than general feature requests. When opening a public issue, describe the desired outcome, file types and sizes, target platforms, transformations the carrier must survive, confidentiality expectations, and what would count as success. **Use synthetic, non-sensitive examples only.**

See [Community participation](COMMUNITY.md) and the [research overview](RESEARCH.md).
