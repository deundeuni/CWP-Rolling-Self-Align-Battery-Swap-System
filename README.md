> **Bilingual Disclosure Notice:** This document is a bilingual disclosure of the same content in KR/EN. v2.0 2026-08-23 (Korean: [README.ko.md](README.ko.md))

# CWP Rotary Self-Aligning Battery Swap System v2 - Heavy & Small Platform

* **Date:** 2026-08-23
* **Author:** deundeuni
* **License:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
* **Purpose:** Open-source hardware specification and Prior Art registration
* **Keywords:** EV battery swap, CWP, self-alignment, V-groove guide, battery swap, rolling rail

---

## 0. Designer's Note

The core concept, parameters, and modular system (Type A/B/C and Type S) are originally conceived and defined by the human designer, deundeuni.

* **Designer (deundeuni):** Conceived the V-groove + height-adjustable caster mechanism, the modular system architecture, and defined all core parameters.
* **AI Tooling:** Meta AI (draft/visualization), Gemini (formatting) — Used strictly as assistive tools under the designer's direction.

---

## 1. Essence - Structure is essence, not appearance

The essence lies in the 3-tier combination mechanism of standard machine elements, not visual representations.

* **Transport:** Rolling rail sliding transfer
* **Alignment Format:** V-groove guide in the 25°~50° range (preferably 30°~45°) combined with height-adjustable casters for mechanical manual self-alignment (Passive Self-Align)
* **Modular Format:** Maintains the same rail standard; frame modules are swapped according to the environment.

---

## 2. Type A / B / C - Heavy Platform

**Environment-Adaptive Types**

| Type | Environment | Core Format |
| :--- | :--- | :--- |
| **Type A** | Flat indoor | Fixed basic rail |
| **Type B (Core)** | **Outdoor unpaved field** | **V-groove self-align + height-adjustable caster** |
| **Type C** | Heavy equipment site | Reinforced H-beam steel frame |

**Technical Specifications (Heavy)**

> **[Non-Limiting Declaration]** All dimensions, angles, and materials in this document are One Embodiment for understanding and can be modified within the range implementing the same function (rolling transfer + V-groove self-align).

* **Main Frame:** 20x20mm to 40x40mm standard aluminum profile or equivalent H-beam (Embodiment: 20x20, 4040)
* **Alignment Guide:** V-groove 25°~50° range (preferably 30°~45°) (Embodiment: 30°)
* **Drive:** Sealed ball bearing roller and low-friction bearing
* **Tolerance Absorption:** ±3mm~±10mm floating constraint (Embodiment: ±5mm)

---

## 3. Type S - Small Platform

**Definition & Mechanism**
Applies the same self-alignment principle as the Heavy platform, light-weighted for small battery specifications.

* **Structure:** 20x20mm class aluminum profile rail + sliding carriage
* **Format:** Mini V-groove 25°~50° range (Embodiment: 30°) + 20mm~50mm class low-profile caster (Embodiment: 25mm, ±5mm self-align)
* **Features:** Weight 1.0kg~3.0kg range (Embodiment: 1.8kg) / Length 250mm~400mm range (Embodiment: 320mm) / Low-profile 70mm~120mm range (Embodiment: 95mm) / Tool-less latch
* **Specification:** (Embodiment: 320x120x95mm / 1.8kg, modifiable within scope)
* **Electrical:** 12V~48V range (Embodiment: 24V 5Ah) / XT30 or equivalent connector / Operating temp -20°C~60°C
* **Application:** E-Scooter, Power Tools, Small AGV, etc.

---

## 4. AI Visualization Disclaimer

> **Note:** Mechanism concept designed by deundeuni. Images are AI-generated conceptual visualizations (Meta AI) for explanatory purposes only, not copied from any product or patent.

---

## 5. Prior Art Declaration and License

This idea is shared as public Prior Art. Including the numerical ranges and variations described above, anyone can freely reference, expand, and implement it commercially.

* **License:** CC BY 4.0 / deundeuni
* **Proof:** GitHub commit history timestamp
