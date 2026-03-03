# NeuroScript — NSF Funding Alignment Analysis

## What NeuroScript Is (for framing purposes)

NeuroScript is a **neural architecture composition language** — a domain-specific language (DSL) written in Rust that compiles to PyTorch. Its core contributions span: compile-time shape algebra and type safety for tensor operations, a composable neuron-as-first-class-unit abstraction, a package manager with cryptographic signing, and an open-source ecosystem with registry aspirations. Future targets include ONNX and JAX backends.

The research surface area touches: **programming language design**, **compiler construction**, **formal methods** (shape inference, type systems), **software engineering** (composability, reuse, package ecosystems), and **AI/ML infrastructure** (making neural architecture development more declarative and less error-prone).

---

## Tier 1 — Strong Alignment

### 1. PESOSE — Pathways to Enable Secure Open-Source Ecosystems
- **Why it fits:** PESOSE's description *literally names "languages"* as an in-scope open-source product type. NeuroScript is an open-source language with a package registry, cryptographic signing, and ecosystem ambitions. The three proposal types map cleanly: (1) scope/plan an OSE, (2) establish/expand a sustainable OSE, (3) improve safety/security/privacy of an existing OSE. The signing/verification infrastructure already in NeuroScript speaks directly to type 3.
- **Status:** Cleared, due **2026-09-01**
- **Fit strength:** Exceptional. This is the most natural home.
- **URL:** https://www.nsf.gov/funding/opportunities/pesose-pathways-enable-secure-open-source-ecosystems/nsf26-506

### 2. SHF — Software and Hardware Foundations
- **Why it fits:** SHF explicitly funds "programming languages research, from foundations to design to implementation" including "design and implementation of domain-specific languages," "compilers and runtime systems," "abstract interpretation, program analysis and optimization." NeuroScript's shape algebra, compile-time validation, and dead-branch elimination are textbook SHF territory. SHF also mentions "formal methods for the specification, modeling, development, and verification of software and hardware systems" and "development of new formal techniques for emerging areas such as artificial intelligence."
- **Status:** Cleared, accepts proposals via Future CoRe solicitation (nsf25-543), due **2026-09-10**
- **Fit strength:** Strong. The language/compiler/formal-methods angle is core SHF.
- **URL:** https://www.nsf.gov/funding/opportunities/shf-software-hardware-foundations/pd25-7798

### 3. MFAI — Mathematical Foundations of Artificial Intelligence
- **Why it fits:** MFAI targets "mathematically grounded design and analysis principles for the current and next generations of AI systems." NeuroScript's shape algebra is a mathematical framework for guaranteeing neural architecture correctness. The program specifically calls for "establishing a fundamental mathematical understanding of the factors determining the capabilities and limitations of current and emerging generations of AI systems" — a shape-typed composition language is one way to formalize what architectures are *expressible* and *valid*.
- **Status:** Cleared, due **2026-10-09**
- **Fit strength:** Strong, but would need to foreground the mathematical contribution (shape algebra, type theory for tensors) over the engineering/tooling.
- **URL:** https://www.nsf.gov/funding/opportunities/mfai-mathematical-foundations-artificial-intelligence/nsf24-569

---

## Tier 2 — Moderate Alignment (with framing)

### 4. Advancing AI Agent Ecosystems through PESOSE (DCL)
- **Why it fits:** This Dear Colleague Letter (posted 2026-02-20 — *four days ago*) specifically encourages proposals about AI agent ecosystems through the PESOSE program. If NeuroScript positions itself as infrastructure enabling composable, verifiable neural components for AI agents, this is timely.
- **Caveat:** DCLs signal interest but aren't standalone solicitations. Would be submitted through PESOSE.
- **URL:** https://www.nsf.gov/funding/opportunities/dcl-advancing-artificial-intelligence-ai-agent-ecosystems

### 5. RI — Robust Intelligence
- **Why it fits:** RI covers "architectures for intelligence" and "computational neuroscience: theory and analysis of computational processes in the nervous system, including approaches to RI problem areas grounded in neural computation." NeuroScript's neuron-as-abstraction philosophy and its compilation of declarative architecture specs into executable PyTorch models touches this.
- **Caveat:** RI warns that "projects that simply apply existing RI techniques to particular domains" don't belong. You'd need to frame NeuroScript as *enabling new research* in architecture search, composability theory, or formal guarantees for neural systems — not just as a tool.
- **Status:** Cleared, via Future CoRe solicitation, due **2026-09-10**
- **URL:** https://www.nsf.gov/funding/opportunities/ri-robust-intelligence/103514

### 6. AIMing — AI, Formal Methods, and Mathematical Reasoning
- **Why it fits:** AIMing supports "research at the interface of innovative computational and AI technologies and new strategies/technologies in mathematical reasoning." NeuroScript's compile-time shape checking is a formal verification problem applied to neural architecture design. If you can frame it as advancing formal methods *for* AI systems (type-theoretic guarantees that architectures are dimensionally consistent), there's alignment.
- **Status:** Cleared
- **URL:** https://www.nsf.gov/funding/opportunities/aiming-artificial-intelligence-formal-methods-mathematical/nsf24-554

### 7. Future CoRe — CISE Future Computing Research (umbrella)
- **Why it fits:** This is the umbrella solicitation containing SHF, RI, HCC, CPS, NeTS, CSR, etc. Budget up to $1M over 4 years. Typical $150K–$250K/year. If the work cross-cuts multiple sub-programs (e.g., SHF + RI), submitting to Future CoRe allows the proposal to be routed appropriately.
- **Status:** Cleared, due **2026-09-10**
- **URL:** https://www.nsf.gov/funding/opportunities/future-core-computer-information-science-engineering-future-computing/nsf25-543

---

## Tier 3 — Tangential / Stretch

### 8. EDSE — Engineering Design and Systems Engineering
- Mentions "data science and artificial intelligence in design" but is fundamentally about engineering artifacts at the physical/systems level. NeuroScript would be a stretch unless framed as "design methodology for neural systems."

### 9. Science of Learning and Augmented Intelligence
- Interesting if NeuroScript were framed as an educational tool for understanding neural architecture composition, but the program's focus is cognitive/behavioral/social science of learning, not programming language design.

### 10. SCH — Smart Health and Biomedical Research in the Era of AI
- Only relevant if NeuroScript were specifically applied to biomedical neural architectures. The tool-agnostic nature of NeuroScript doesn't give it a natural home here.

### 11. Expeditions in Computing
- $15M over 7 years. Transformative, decade-ahead vision. NeuroScript alone isn't at this scale, but could be *part of* a larger Expedition around "verified AI infrastructure" or "composable intelligence."

### 12. EPCN — Energy, Power, Control, and Networks
- Mentions neural networks and neuromorphic engineering but is focused on energy/power/control systems. Wrong domain.

---

## Programs With No Meaningful Alignment

The following appeared in the CSV but have negligible relevance to NeuroScript: CAIG (geosciences), National AI Research Institutes (waiting for new publication), NSF-Italy DCL, Biology/AI intersection DCL, Plant Genome Research, NQNI (quantum/nano), CICI (cybersecurity), IDSS (data infrastructure), CyberAI SFS (scholarships), CCI (chemistry centers), PRFB (postdoctoral biology fellowships), TCUP (tribal colleges), DMREF (materials), PCL Test Bed (autonomous labs), CREST-RISE (MSI capacity building), eMB (math biology), CER (computing education), RTG (math training groups), FIRE (wildland fire science), PoLS (physics of living systems), DARE (disability engineering), Fluid Dynamics, Thermal Transport, Biosensing, CCSS (circuits/sensing), RFE (formation of engineers), MSI (manufacturing systems), CMFP (chemistry), FRR (robotics), M3X (human-machine interaction), RITEL (ed-tech), ExLENT (workforce), FDT-BioTech (digital twins), FM (future manufacturing), CPS (cyber-physical), SaTC 2.0 (cybersecurity), HCC (human-centered computing), and various DCLs.

---

## Critical Caveat: Eligibility

Most NSF programs require proposals from **institutions of higher education** (universities) or **non-profit research organizations**. If you're applying as an independent developer or a for-profit entity, your eligibility is sharply limited. Common paths around this:

- **Academic collaboration:** Partner with a university PI who leads the proposal; you contribute as senior personnel or via a subaward.
- **SBIR/STTR:** If NeuroScript has commercial potential, NSF's Small Business Innovation Research program funds early-stage R&D at small businesses. This wasn't in the CSV but is worth investigating separately.
- **Non-profit formation:** Some open-source projects form 501(c)(3) organizations to become eligible for federal grants.

This eligibility question isn't a minor detail — it determines whether any of the above is actionable for you personally.

---

## Recommended Next Steps

1. **Clarify your institutional affiliation** — this determines which programs you can actually apply to.
2. **PESOSE is the clearest shot** if you have or can establish an eligible organizational structure. The language, the package registry, the signing infrastructure — it's like they wrote the solicitation for projects like NeuroScript.
3. **SHF via Future CoRe** is the strongest *research* angle if you partner with an academic PL/compilers group.
4. **Read the Advancing AI Agent Ecosystems DCL carefully** — it's brand new and may signal where NSF is directing reviewer attention within PESOSE.
