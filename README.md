> **Bilingual Disclosure Notice:** This is a bilingual disclosure - same content in KR/EN, v2.2 2026-09-13 (Korean version: [README.ko.md](README.ko.md))  
> **Original Authority Notice:** This English version was drafted and translated with the assistance of AI tools, so phrasing and expressions may not be perfectly smooth or fully precise. The authoritative original for all legal, technical, and engineering interpretations belongs exclusively to the Korean document (`README.ko.md`). (PHILOSOPHY.ko.md is authoritative original)

# CWP Rotary Self-Aligning Battery Swap System v2.2 - Heavy & Small Platform (Battery Application Embodiment of a Universal Heavy Payload & Small Module Fail-Safe Mechanical Alignment Platform)

* **Date:** 2026-09-13 (first draft 2026-08-20, v2.0 2026-08-23, v2.1 2026-09-06, v2.2 2026-09-13)
* **Author:** deundeuni (System Architect / Natural Person Inventor)
* **License:** CERN-OHL-S v2 (Hardware/CAD/Schematics) | CC BY-SA 4.0 (Documentation/Diagrams)
* **Purpose:** Defensive Publication / Prior Art - To prevent exclusive patenting and mitigate infringement risks
* **Keywords:** CWP, CWP-Rolling-Self-Align, EV battery swap, self-alignment, V-groove guide, Passive Self-Align, Rolling Rail, Type A, Type B, Type C, Type S, Battery Swap, Height Adjustable Caster, Low Impact Docking, Prior Art, CWP-Entry, CWP-Battery-Swap, CWP-Clamping, universal heavy payload alignment, Heavy Payload Alignment Platform, Off-Grid Self-Align, open-field heavy module precision alignment

---

## 0. Designer's Philosophical Declaration (Designer's Independent Conception & Prior Art Disclosure)

1. **Architectural Conception and Originality of Technology Combination:**  
   This system originated from the **designer's (deundeuni) independent philosophy and problem-solving framework**: aiming to achieve secure docking and coupling via mechanical passive self-alignment (Passive Self-Align) without relying on expensive dedicated servo equipment, even under harsh field conditions such as unpaved outdoor terrain, power outages, and trapped passengers. The architectural decision-making authority—conceiving the 3-tier mechanical combination of 'V-groove guide + height-adjustable caster + sliding rolling rail' and establishing the modular system framework (Types A/B/C and Type S) along with parametric numerical ranges—belongs solely to the natural person designer.

2. **Limitation on Software Utility Usage:**  
   Software and AI tools utilized in drafting this document are limited strictly to **Passive Execution Utilities** that executed simple formatting, contextual refinement, and conceptual visualization outputs based on the technology combinations, design directions, and numerical parameters already defined by the designer. All design intent, structural combination rights, and prior art disclosure authority for this infrastructure belong entirely to the natural person designer.

---

## 1. Essence & Application Scope

### 1.1 Mechanism Essence - Structure is essence, not appearance
The technical essence of this system lies in the 3-tier combination mechanism of standard machine elements, rather than visual representations or specific payloads.

* **Transport:** Rolling rail sliding transfer structure supporting low-friction linear motion.
* **Alignment Format:** Modular structure combining a V-groove guide in the 25°~50° range (preferably 30°~45°) with height-adjustable casters to facilitate mechanical passive self-alignment (Passive Self-Align).
* **Modular Format:** Framework structured to swap frame modules according to environmental and operational requirements while maintaining a standardized rail specification.

### 1.2 Application Scope
This structure is not limited to EV battery swapping, but is universally applicable to the absorption of physical dimensional errors and precision mechanical coupling of heavy modular housing, disaster shelters, agricultural machinery modules, logistics pallets (over 500kg), and small module payloads in open-field and unpaved terrain. It encompasses all domains requiring payload attachment/detachment and alignment, including EV, ESS, logistics robots (AGV/AMR), drones, marine, aerospace, and construction/agricultural heavy equipment modules.

---

## 2. Type A / B / C - Heavy Platform

### 2.1 Environment-Adaptive Type Classification

* **Type A (Flat Indoor):** Fixed basic rail structure aiming for high-precision alignment.
* **Type B (Outdoor Unpaved Field - Core):** V-groove self-alignment guide combined with height-adjustable casters to flexibly absorb ground unevenness and sand/dirt clearance errors.
* **Type C (Heavy Equipment Site):** Reinforced H-beam steel frame structure supporting high-load operations.

### 2.2 Technical Specifications (Heavy)

* **[Non-Limitation Declaration]** All dimensions, angles, and materials in this document represent One Embodiment provided for explanatory purposes. Modified values, material substitutions, and variant applications implementing equivalent functions (rolling transfer + V-groove self-alignment) fall within the scope of this prior art.

* **Main Frame:** 20x20mm to 40x40mm standard aluminum profile or equivalent H-beam (Embodiment: 20x20, 4040)
* **Alignment Guide:** V-groove 25°~50° range (preferably 30°~45°) (Embodiment: 30°)
* **Drive:** Sealed ball bearing roller and low-friction bearing structure
* **Tolerance Absorption:** ±3mm~±10mm floating constraint range (Embodiment: ±5mm)

---

## 3. Type S - Small Platform

A lightweight module format applying the same mechanical self-alignment principle as the Heavy platform, adapted for smaller battery and small module specifications.

* **Transport Structure:** 20x20mm class aluminum profile rail combined with a sliding carriage.
* **Alignment Format:** Mini V-groove 25°~50° range (Embodiment: 30°) combined with 20mm~50mm class low-profile casters (Embodiment: 25mm, supporting ±5mm self-alignment tolerance absorption).
* **Mechanical Specifications:** Weight range 1.0kg~3.0kg (Embodiment: 1.8kg) / Length range 250mm~400mm (Embodiment: 320mm) / Low-profile height range 70mm~120mm (Embodiment: 95mm) / Tool-less latch engagement.
* **Detailed Specification:** (Embodiment: 320 x 120 x 95 mm / 1.8 kg, modifiable within scope)
* **Electrical Specifications:** Voltage range 12V~48V (Embodiment: 24V 5Ah) / XT30 or equivalent connector / Operating temperature -20°C to 60°C.
* **Target Applications:** Electric scooters, power tools, small logistics robots (AGVs/AMRs), drone landing skids, small sensor modules, and related domains.

---

## 3.5 CWP 3-Hardware Mechanisms & Survival Architecture (CWP 3-Hardware & System Integration)

This mechanical self-alignment structure (Type B/S) does not function in isolation; it operates organically in combination with the three core CWP hardware mechanisms and upper survival architectures to form a zero-downtime survival-oriented swapping station and precision docking infrastructure.

* **Entry Guidance & Primary Alignment (`CWP-Entry`):** Reusing car wash V-rail and ground guide groove infrastructure and line laser guides to mitigate vehicle entry errors and guide the vehicle into the servicing zone.
* **Mechanical Secondary Alignment (`CWP-Rolling-Self-Align-Battery-Swap-System` - This Technology):** Interfacing with V-groove and caster manual/self-alignment mechanisms (Types A/B/C/S) to physically absorb entry tolerance errors (e.g., ±5mm or more) and guide the pack into the precise docking zone. (Applicable to battery packs and universal heavy modules over 500kg)
* **Differential Speed Low-Impact Docking (`CWP-Battery-Swap`):** Utilizing N/(N+1) differential gear ratios (e.g., 60T/61T) and a rotary stage to slow down relative engagement speed to extremely low levels (e.g., ~0.016rpm level) aiming for cushioned docking.
* **Electromagnetic Clamping & Secure Latching (`CWP-Clamping-Battery-Swap-System`):** Interfacing with universal EPM magnetic clamping modules, dual locking pins, and 3-layer cushion structures to achieve unpowered permanent magnetic holding and emergency release capability.
* **Physical Emergency Detachment & Release (`0.1ms HW Intercept` / `LAST-LIGHT` Integration):** Upon emergency events such as power outages or fire, a Hardware Intercept signal releases chains, pneumatics, and EPM clamps, supporting unpowered mechanical detachment and emergency escape.
* **Computational Control Survival (`chiplet-apu-multi-system-survival-architecture`):** Interfacing with distributed control (CCS) and multi-chiplet control architecture to ensure alignment and swapping control logic continues operating even if a control chiplet fails.

---

## 4. Limitation, Disclaimer of Warranties & Liability

This document is a technical concept disclosure for defensive publication and is provided strictly "AS-IS" without warranty of any kind.

1. **Disclaimer of Warranties:** No warranty of any kind, express or implied, is given regarding fitness for a particular purpose, merchantability, safety, or feasibility of commercialization.
2. **Limitation of Liability:** The author (deundeuni) shall not be liable for any direct, indirect, incidental, special, or consequential damages, accidents, or losses resulting from the use, implementation, or application of this document.
3. **Non-Infringement Disclaimer:** No warranty is provided that this document or implementations based on it do not infringe third-party patents, trademarks, copyrights, or other intellectual property rights. Freedom-to-operate investigation is the sole responsibility of the implementer.
4. **Compliance & Safety Responsibility:** Compliance with national regulations, electrical/fire/safety standards, certification acquisition, and safety verification remains fully the responsibility of the implementer.

---

## 5. Figures & AI Visualization Disclaimer

* **Note (AI Visualization Disclaimer):** The mechanism concept in this specification was independently conceived by the author (deundeuni). Attached figures or conceptual drawings are visual examples generated using generic generative AI visualization tools for explanatory purposes only and are not copied from any existing product or registered patent of others.
* **Note on Drawings:** All dimensions, angles, and quantities in these drawings are non-limiting illustrative examples. Only functional structures (V-groove self-alignment, rolling rail, caster combination) constitute the core of this disclosure.

---

## 6. Licensing & Commercial Usage Guidelines

```text
CERN Open Hardware Licence Version 2 - Strongly Reciprocal (CERN-OHL-S v2)
Copyright (c) 2026 deundeuni

This hardware design is licensed under CERN-OHL-S v2.
You may manufacture and distribute it, even commercially,
but if you distribute products based on it, you must also
make the modified design files available under the same license.

Full text: [https://ohwr.org/cern_ohl_s_v2.pdf](https://ohwr.org/cern_ohl_s_v2.pdf)

Documentation and figures: CC BY-SA 4.0
[https://creativecommons.org/licenses/by-sa/4.0/](https://creativecommons.org/licenses/by-sa/4.0/)
```

* **Commercial Usage Guidelines:** Both commercial manufacturing and sales are permitted. You only need to make modified design files of the CWP portion available under the same license; you are not required to disclose other proprietary secrets of your company.

---

## 7. Practical Protection

* **Authoritative Original Principle:** The legal and technical interpretations of this specification strictly prioritize the Korean original document (`README.ko.md`), while English and other translations function solely for secondary reference.
* **Broad Scope Inclusion:** Rail specifications, V-groove angles, tolerance absorption figures, and caster methods described herein are illustrative examples for broad prior art coverage and apply generically as upper concepts.
* **Separation of Commercialization Content:** This white paper original contains strictly Pure Open Source and prior art disclosures, while proprietary revenue models and business execution details are managed separately as standalone technical documents.

---

## 8. Sources & Records

* **Ecosystem Repositories & Academic Identifiers**
  * Universal Survival Architecture & APU Controller (`chiplet-apu-multi-system-survival-architecture`) — GitHub: `deundeuni / chiplet-apu-multi-system-survival-architecture` | CERN Zenodo DOI: `10.5281/zenodo.22374987` (https://doi.org/10.5281/zenodo.22374987)
  * Disaster Evacuation & Auxiliary Infrastructure (`LAST-LIGHT`) — GitHub: `deundeuni / LAST-LIGHT` | CERN Zenodo DOI: `10.5281/zenodo.22373189` (https://doi.org/10.5281/zenodo.22373189)
  * CWP Rolling Self-Align (`CWP-Rolling-Self-Align-Battery-Swap-System`) — CERN Zenodo DOI: `10.5281/zenodo.22373704` (https://doi.org/10.5281/zenodo.22373704)
  * CWP Battery Swap Docking (`CWP-Battery-Swap`) — CERN Zenodo DOI: `10.5281/zenodo.22373538` (https://doi.org/10.5281/zenodo.22373538)
  * CWP Electromagnetic Clamping (`CWP-Clamping-Battery-Swap-System`) — CERN Zenodo DOI: `10.5281/zenodo.22373722` (https://doi.org/10.5281/zenodo.22373722)
  * CWP Entry Guidance & Alignment (`CWP-Entry`) — GitHub: `deundeuni / CWP-Entry`
  * Canonical Gateway & Main Repository (`soma-moa`) — GitHub: `deundeuni / soma-moa` | Gateway Domain: `somamoa.ai.kr`

* **Legal Statutes & Precedents**
  * Korean Patent Act Article 103 — Prior Use Rights (Non-exclusive License by Prior Use)
  * 35 U.S.C. §273 — Defense to Infringement Based on Prior Commercial Use
