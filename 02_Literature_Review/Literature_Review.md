# 5. Literature Review Supporting Materials

## 5.0 Scope and Consistency with the Research Proposal

This supporting report is based on the supplied systematic literature review paper, *Vulnerability Analysis of Operational Security (OPSEC) in Military Contexts (2018–2026)*. It supports a proposed study of military OPSEC vulnerabilities in modern cyber-physical and information-warfare environments.

The literature is organised around three connected domains:

1. **Human factors:** social engineering, digital behaviour, social media, geolocation leakage, and open-source intelligence (OSINT).
2. **Process security:** Command, Control, Communication and Intelligence (C3I) systems, supply-chain security, firmware, credentials, and cyber-threat-intelligence sharing.
3. **Operational and technical risk:** IoBT, UAVs, GPS spoofing, AI-enabled attacks, Zero Trust Architecture (ZTA), deception, and mission assurance.

> **Source note:** The supplied PDF reports 140 records identified, 75 records assessed for eligibility, and 20 studies included in the final review. The detailed comparison below is a representative sample of 15 sources reported in the paper. Bibliographic details and numerical claims should be checked against the original publications before final submission.

## 5.1 Review Questions

The literature review supports the following research questions:

- **RQ1:** What are the key vulnerabilities affecting modern military OPSEC?
- **RQ2:** How have emerging technologies such as AI, IoBT, UAVs, and OSINT affected OPSEC?
- **RQ3:** What mitigation strategies are proposed in current literature?
- **RQ4:** What research gaps limit the development of resilient military OPSEC?

## 5.2 Literature Search and Selection Summary

### Information Sources

The source review searched Google Scholar and IEEE Xplore. Google Scholar provided broad coverage of journal articles, conference papers, and technical reports, while IEEE Xplore provided focused coverage of cybersecurity, engineering, defence systems, and emerging technologies.

### Search Period and Search Strings

The review covered publications from 2018 to 2026. The reported Boolean search strings were:

```text
("Operational Security" OR "OPSEC") AND ("Military" OR "Defense")
AND ("Human Factors" OR "Process Security")

("Supply Chain 4.0" OR "C3I") AND ("Cybersecurity" OR "Vulnerability Analysis")

("Zero Trust Architecture" OR "ZTA") AND ("Military UAV" OR "IoBT")

("Open-Source Intelligence" OR "OSINT") AND "Military Operational Security"
```

### Search and Screening Results

| Database | Records identified | After screening | Final included |
|---|---:|---:|---:|
| Google Scholar | 80 | 45 | 12 |
| IEEE Xplore | 60 | 30 | 8 |
| **Total** | **140** | **75** | **20** |

### Inclusion and Exclusion Criteria

| Inclusion criteria | Exclusion criteria |
|---|---|
| Published between 2018 and 2026 | Published before 2018 |
| Peer-reviewed journal articles and conference papers | Blogs, opinion articles, or other non-scholarly sources |
| Official government or defence reports where relevant | Studies focused only on civilian enterprise security |
| Military or defence application | No military or defence relevance |
| Written in English | Non-English publications |
| Relevant to OPSEC, cybersecurity, human factors, military systems, or countermeasures | Duplicate or irrelevant records |

### Data Extraction and Quality Assessment

The source review extracted information about vulnerabilities, technologies, mitigation strategies, study methods, and OPSEC relevance. The reported quality assessment considered:

- computational feasibility;
- adversarial robustness;
- relevance to military OPSEC;
- practical applicability to C3I, UAV, IoBT, and logistics environments; and
- whether the proposed method was evaluated empirically rather than only conceptually.

## 5.3 Literature Review Analysis Table

The following table consolidates the representative studies identified in the supplied PDF. The focus, method, finding, and limitation columns support comparison for Chapter 2.

| Reference | Focus/theme | Method or technique | Main finding | Limitation or critical observation |
|---|---|---|---|---|
| Ahmad et al. (2023) | Process security; C3I | Taxonomy and survey of vulnerabilities, attacks, and countermeasures | Identifies 13 vulnerability types and 19 attack vectors in C3I systems; reports that 61% of reviewed research lacks rigorous evaluation. | Taxonomy-based analysis may not fully represent live battlefield conditions; the review highlights an evaluation gap rather than solving it. |
| Nowakowski (2025) | Human factors | Six-phase human-hacking framework using MICE and RASCLS concepts | Explains how adversaries use psychological triggers and staged social engineering to exploit personnel. | Framework effectiveness requires validation with military populations and realistic exercises. |
| Takpah and Oriakhi (2025) | Process security; Supply Chain 4.0 | Systematic literature review and simulation-based hybrid cybersecurity framework | Highlights supply-chain poisoning risks in interconnected military logistics. | Simulation results may not capture classified supplier relationships, legacy systems, or active adversarial pressure. |
| Dimitrov and Iliev (2025) | Human factors; geolocation | Case-study analysis of personal smart devices and location data | Shows that fitness and mobile-device data can expose routines, personnel, and military locations. | Case evidence is context-dependent and does not provide a universal risk model for all military bases. |
| Alquwayzani and Albuali (2024) | Operational risk; UAV and IoBT | Systematic literature review of Zero Trust Architecture | Presents ZTA as a strong security approach for distributed military UAV and IoBT systems. | ZTA implementation can be difficult on low-power devices and may introduce latency, policy, and interoperability challenges. |
| Staněk et al. (2025) | Process security; explainable AI | Review of XAI methods including SHAP and LIME | Finds that current XAI methods can be computationally heavy for low-latency combat environments. | The review does not establish which lightweight explanation method is most suitable for each tactical platform. |
| Parmadi and Ramli (2026) | Operational risk; CTI | Hybrid model using STIX 3.0 metadata for military-civilian CTI sharing | Proposes classification-aware information sharing to reduce separation between military and civilian cyber-threat intelligence. | Legal, classification, privacy, and trust barriers may prevent full cross-domain implementation. |
| Danciu (2023) | Human factors; social media | Qualitative analysis | Identifies social media as both an operational communication tool and an OPSEC risk; education is described as a cost-effective countermeasure. | Education alone cannot prevent technical compromise, insider threats, or automated OSINT analysis. |
| Tschimben et al. (2023) | Operational risk; deception | Nonnegative Matrix Factorization (NMF) for digital decoys | Uses digital decoys to obfuscate troop movements and confuse adversarial analysis. | Deception must be carefully controlled because false signals can confuse friendly decision-makers or expose the deception. |
| Malerud and Fridheim (2018) | Operational risk; mission planning | Bow-tie model and gap analysis | Identifies vulnerabilities in mission-critical capability assumptions and signposts that should trigger plan revision. | The 2018 study predates several current AI, IoBT, and supply-chain conditions. |
| Beninger et al. (2024) | Process security; firmware supply chain | AI-driven Software Bill of Materials (SBOM), referred to as ERS0 | Proposes automated detection of firmware vulnerabilities across large numbers of variant packages. | AI-generated findings require validation, reliable component data, and protection against manipulated supplier information. |
| Rurak and Goniewicz (2024) | Operational risk; air-base security | Risk analysis and multi-layered surveillance using drones and biometrics | Proposes integrated surveillance and biometric controls to address internal and perimeter threats. | Surveillance and biometrics introduce privacy, false-alarm, governance, and operational-dependency risks. |
| Avrahami et al. (2025) | Human factors; OSINT | Literature review of proactive OSINT-based cybersecurity | Reports that OSINT can provide a large proportion of actionable intelligence and supports AI-assisted filtering. | OSINT volume, source reliability, misinformation, and analyst bias can reduce confidence in automated conclusions. |
| Tuli et al. (2025) | Operational risk; navigation | Hybrid quantum machine learning for GPS-spoofing detection | Reports 88% accuracy for detecting GPS spoofing in military mission scenarios. | The reported accuracy needs independent replication and comparison with lightweight classical models on operational hardware. |
| Maathuis (2025) | Operational risk; military decision-making | Ontology design and automated reasoning | Models unintended adverse effects, or blowback, to support structured military reasoning. | Ontology completeness and the reliability of automated reasoning remain difficult to establish in complex conflicts. |

## 5.4 Comparison of Existing Techniques

| Technique | Primary threat addressed | Strengths | Weaknesses | Suitability for proposed research |
|---|---|---|---|---|
| Security awareness and Human Firewall training | Social engineering, unsafe digital behaviour, social-media exposure | Low cost, scalable, addresses the human attack surface | Behaviour is difficult to measure; training can decay without reinforcement | Include as a human-control layer and evaluate knowledge or behaviour change. |
| OSINT monitoring and AI-assisted filtering | Publicly visible routines, geolocation, behavioural patterns, misinformation | Enables early warning and large-scale data processing | False positives, source unreliability, privacy concerns, adversarial manipulation | Use for risk discovery with analyst review rather than fully autonomous decisions. |
| Zero Trust Architecture | Credential abuse, lateral movement, distributed IoBT and UAV compromise | Continuous verification, least privilege, micro-segmentation | Complex deployment, latency, policy overhead, limited-resource devices | Use as the main architectural mitigation for distributed military systems. |
| AI/XAI anomaly detection | Unknown attacks, abnormal network or device behaviour | Can identify patterns not captured by fixed rules; explanations may support analyst trust | Training-data bias, adversarial examples, computational cost, explanation quality | Compare lightweight detection and explanation methods under resource limits. |
| AI-driven SBOM and firmware analysis | Supply-chain poisoning and vulnerable components | Improves component visibility and automates large-scale checking | Depends on accurate SBOMs and trustworthy suppliers; false positives require review | Use to support secure-by-design supply-chain risk management. |
| Digital decoys and deception | OSINT exploitation, movement tracking, adversary intelligence collection | Can waste adversary resources and conceal real activity | Risk of confusing friendly forces; requires careful coordination | Evaluate as a supplementary OPSEC control, not a replacement for protection. |
| CTI sharing with STIX metadata | Fragmented military and civilian threat intelligence | Standardised information can improve correlation and response | Classification, legal, privacy, and trust barriers | Investigate a controlled information-sharing model and its governance requirements. |
| GPS-spoofing detection | Navigation disruption of UAVs and military missions | Directly addresses an operationally important attack | Accuracy may not generalise; quantum models may not be practical on edge devices | Benchmark proposed detection against classical baselines and resource constraints. |

## 5.5 Summary of Methods and Algorithms

### Human and Behavioural Methods

- **MICE:** Money, Ideology, Coercion, and Ego; a framework for understanding possible insider or social-engineering motivations.
- **RASCLS:** A set of psychological influence triggers used to structure human-hacking analysis.
- **Human Firewall:** A defence approach combining awareness, digital hygiene, behavioural monitoring, and psychological resilience.
- **Qualitative case analysis:** Used to examine social-media exposure and real-world geolocation risks.

### Technical and Architectural Methods

- **Zero Trust Architecture:** Never trust by default; continuously verify users, devices, services, and access requests.
- **Micro-segmentation:** Divides a distributed network into smaller controlled security zones to reduce lateral movement.
- **AI/XAI anomaly detection:** Identifies deviations from expected behaviour and uses explanation techniques such as SHAP or LIME to assist analysts.
- **SBOM and AI firmware analysis:** Records software and firmware components and checks them for known or inferred vulnerabilities.
- **STIX 3.0 metadata:** Supports structured cyber-threat-intelligence exchange and classification-aware sharing.
- **Nonnegative Matrix Factorization:** Used to model patterns and create digital decoys for operational deception.
- **Hybrid quantum machine learning:** Applied in the source paper to GPS-spoofing detection; requires comparison with classical alternatives.
- **Ontology-based reasoning:** Represents entities, relationships, actions, and unintended consequences for automated analysis.

## 5.6 Relevant Datasets, Data Sources, and Tools

The supplied PDF does not provide a single named public dataset for the full review. Instead, it describes a systematic review of scholarly literature and several application-specific evidence sources. The following data sources are therefore relevant to the proposed methodology.

| Data source or tool | Intended use | Important consideration |
|---|---|---|
| Google Scholar | Broad literature discovery | Results require duplicate removal and quality screening. |
| IEEE Xplore | Engineering, cybersecurity, and defence literature | Search results may favour technical publications and may omit relevant policy research. |
| Peer-reviewed papers and official reports | Evidence for OPSEC vulnerabilities and countermeasures | Publication quality and military relevance must be assessed consistently. |
| Public OSINT and social-media data | Study of geolocation leakage, routines, and adversarial information discovery | Use only lawful, ethical, anonymised data; do not expose real operational information. |
| C3I and IoBT network traces | Detection of abnormal behaviour, credential misuse, or lateral movement | Real military data is normally classified; synthetic or de-identified traces may be required. |
| UAV telemetry and GPS signals | Evaluation of spoofing detection | Test with controlled simulation and safe laboratory conditions. |
| SBOM and firmware package records | Supply-chain and component-vulnerability analysis | Validate component provenance and protect supplier information. |
| STIX 3.0 threat-intelligence records | Structured CTI exchange and correlation | Apply classification, access-control, and data-minimisation rules. |
| Simulated digital-decoy scenarios | Evaluation of deception and movement obfuscation | Measure both adversary confusion and friendly-force decision quality. |

### Data Limitations

Military datasets are difficult to obtain because of classification, privacy, safety, and operational-security restrictions. Consequently, the proposed research should clearly distinguish between real operational evidence, public OSINT, synthetic data, simulation, and expert assessment. Results from simulated or civilian datasets should not automatically be presented as proof of battlefield effectiveness.

## 5.7 Evaluation Metrics Identified from Previous Research

| Metric | Purpose | Application in the proposed study |
|---|---|---|
| Detection accuracy | Measures correct classification of attacks and benign activity | Report for GPS spoofing, anomaly detection, or malware classification, together with class distribution. |
| Precision | Measures how many detected alerts are true threats | Important because excessive false alarms can overload military analysts. |
| Recall or detection rate | Measures how many actual threats are detected | Important for high-consequence attacks such as spoofing, supply-chain compromise, and credential abuse. |
| False-positive rate | Measures benign events incorrectly flagged as threats | Indicates operational burden and possible alert fatigue. |
| False-negative rate | Measures missed threats | Critical for OPSEC because an undetected compromise may expose missions or personnel. |
| F1-score | Balances precision and recall | Useful for imbalanced attack datasets. |
| Detection latency | Time from threat occurrence to alert | Essential for real-time or low-latency tactical environments. |
| Computational cost | CPU, memory, storage, and energy required | Determines whether AI/XAI, encryption, or monitoring can run on tactical sensors. |
| Communication overhead | Additional bandwidth and message volume | Important for distributed IoBT, UAV, and CTI-sharing systems. |
| Robustness to adversarial change | Performance against unseen attacks, altered inputs, or evasion | Addresses the generalisation gap identified in the literature. |
| Coverage of vulnerabilities and attack vectors | Breadth of threats represented | Supports comparison with the C3I vulnerability taxonomy. |
| Human-training improvement | Change in knowledge, behaviour, reporting, or phishing resistance | Evaluates the Human Firewall intervention. |
| Analyst workload and explanation usefulness | Whether alerts and XAI outputs support decisions | Prevents technically accurate systems from becoming operationally unusable. |
| Mission assurance | Ability to preserve essential functions during compromise | Links cybersecurity performance to military operational outcomes. |

## 5.8 Research Gap Analysis

### Gap 1: Lack of Military-Specific AI Benchmarks

Many XAI and autonomous threat-detection studies use civilian datasets or generic benchmarks. These datasets do not represent classified information, battlefield deception, mission urgency, tactical communications, or military-specific attack behaviour. A military OPSEC study therefore needs a transparent benchmark design that records data source, threat type, classification level, and operational context.

### Gap 2: Lightweight Security for Tactical Sensors

Encryption, intrusion detection, XAI, and continuous monitoring may be too computationally expensive for low-power and low-memory IoBT sensors. Future work should compare lightweight algorithms using processing time, memory, energy, bandwidth, and detection performance rather than accuracy alone.

### Gap 3: Fragmented Military-Civilian CTI Sharing

STIX-based CTI exchange may improve national cyber defence, but classification rules, privacy law, ownership, trust, and organisational boundaries limit information sharing. The research gap is not only technical; it also includes governance, access control, and information-release policies.

### Gap 4: Weak Real-World Evaluation

The source paper reports that a substantial proportion of existing work relies on hypothetical scenarios or simplified simulations. The literature review also reports that 61% of research in the C3I review lacks rigorous evaluation and identifies approximately 36% of reviewed academic studies as lacking rigorous real-world testing. These figures should be verified against the original reviews, but they consistently indicate an empirical-evaluation problem.

### Gap 5: Fragmented Treatment of Human, Process, and Technical Risk

Existing studies commonly focus on one layer: human behaviour, network architecture, supply chain, navigation, or AI detection. Fewer studies evaluate how these layers interact. For example, a secure technical control can be defeated by social engineering, while a trained operator can still be exposed by insecure firmware or GPS spoofing. An integrated OPSEC framework is therefore needed.

## 5.9 Proposed Methodology Supported by the Literature

Based on the reviewed evidence, the proposed research should use a mixed and layered methodology:

1. **Systematic evidence review:** Follow PRISMA 2020 principles and document databases, search strings, screening, eligibility, and final inclusion.
2. **Vulnerability taxonomy:** Classify findings into human factors, process security, and operational/technical risk.
3. **Threat modelling:** Map assets, threat actors, attack vectors, vulnerabilities, impacts, and controls using a structured risk model.
4. **Scenario-based evaluation:** Develop controlled scenarios for social engineering, OSINT/geolocation exposure, C3I compromise, supply-chain poisoning, GPS spoofing, and IoBT lateral movement.
5. **Technical benchmarking:** Compare detection or mitigation methods using accuracy, false negatives, latency, resource cost, and robustness to unseen attacks.
6. **Human-factor assessment:** Evaluate awareness, digital hygiene, reporting behaviour, and resistance to social-engineering techniques.
7. **Architecture analysis:** Assess ZTA, micro-segmentation, SBOM, CTI sharing, and deception as complementary layers rather than isolated solutions.
8. **Critical synthesis:** Compare effectiveness, limitations, feasibility, governance requirements, and mission impact.

This approach follows the central finding of the source paper: resilient OPSEC requires coordinated human, technical, process, and strategic controls.

## 5.10 Proposed Conceptual Framework

```text
Threat environment
	|
	+--> Human threats: social engineering, insider risk, social media, geolocation
	|
	+--> Process threats: C3I configuration, credentials, supply chain, firmware
	|
	+--> Technical threats: IoBT compromise, UAV hijacking, GPS spoofing, APTs
	|
	v
OPSEC risk assessment
	|
	+--> Human Firewall and awareness controls
	+--> Zero Trust and micro-segmentation
	+--> AI/XAI monitoring and anomaly detection
	+--> SBOM and secure-by-design supply chain
	+--> CTI sharing and structured threat intelligence
	+--> Digital deception and signature management
	|
	v
Evaluation
	|
	+--> Detection and mitigation effectiveness
	+--> Latency, resource use, and communication overhead
	+--> Adversarial robustness and unseen-attack performance
	+--> Human behaviour and analyst workload
	+--> Mission assurance and governance feasibility
```

## 5.11 Synthesis of Findings

The reviewed literature demonstrates a cybersecurity paradox: technologies that improve military awareness and coordination can also increase the attack surface available to adversaries. C3I, UAVs, IoBT, social media, AI, and connected logistics improve capability but expose information, devices, processes, and personnel to exploitation.

Three themes recur across the studies:

- **Human exposure is persistent.** Personnel behaviour, social-media activity, personal devices, psychological manipulation, and geolocation data can reveal sensitive information without a direct network intrusion.
- **Perimeter security is insufficient.** Distributed UAV and IoBT systems require continuous verification, least privilege, segmentation, and monitoring because devices and communication channels cannot be assumed trustworthy.
- **Security controls must be evaluated in context.** A highly accurate model may be unsuitable if it is too slow, consumes too much energy, produces too many false alerts, or cannot operate with classified data.

The strongest direction for the proposed research is therefore a layered OPSEC model that combines Human Firewall practices, Zero Trust, secure supply-chain controls, AI-assisted monitoring, structured CTI, and controlled deception. No individual technique is sufficient for the full range of human, process, and technical vulnerabilities.

## 5.12 References Supporting the Proposed Methodology

Ahmad, H., Dharmadasa, I., Ullah, F., & Babar, M. A. (2023). A review on C3I systems' security: Vulnerabilities, attacks, and countermeasures. *ACM Computing Surveys, 55*(9), 1–38. https://doi.org/10.1145/3558001

Alquwayzani, A. A., & Albuali, A. A. (2024). A systematic literature review of zero trust architecture for military UAV security systems. *IEEE Access, 12*, 1–32. https://doi.org/10.1109/ACCESS.2024.3503587

Avrahami, Z., Zwilling, M., & Hajaj, C. (2025). Leveraging OSINT for advanced proactive cybersecurity: Strategies and solutions. *IEEE Access, 13*, 1–25. https://doi.org/10.1109/ACCESS.2025.3603868

Beninger, M., Ding, S. H. H., Charland, P., & Fung, B. C. M. (2024). ERS0: Enhancing military cybersecurity with AI-driven SBOM for firmware vulnerability detection and asset management. In *Proceedings of the 16th International Conference on Cyber Conflict (CyCon)*. NATO CCDCOE Publications.

Briggs, G. (2023). Russia's misinformation campaign during wartime: The threat to deploy nuclear weapons against Ukraine and her allies. *Journal of Information Warfare, 22*(1), 32–43.

Correnti, J., Lospinoso, J., Weigand, M., & Kramer, K. (2019). Hidden vulnerabilities: Operational technology cybersecurity shortfalls. In *Proceedings of the Ground Vehicle Systems Engineering and Technology Symposium (GVSETS)*.

Danciu, D. (2023). Social media and the security of military operations. *Studia Securitatis, 2*, 242–249.

Dimitrov, D. S., & Iliev, I. Y. (2025). The risk of personal smart devices in the operational security for military bases, personnel and missions. In *Proceedings of the 16th International Scientific and Practical Conference: Environment. Technology. Resources* (Vol. 2, pp. 99–106). https://doi.org/10.17770/etr2025vol2.8616

Maathuis, C. (2025). *Towards modelling military disadvantage in military operations* (University research paper).

Malerud, S., & Fridheim, H. (2018). Security risk and vulnerability analysis in military operational planning: The why's and how's. In *Safety and Reliability – Safe Societies in a Changing World* (pp. 414–418). Taylor & Francis Group.

Moinuddin, S. M. (2025). Conceptualising information warfare: A strategic imperative for the Bangladesh armed forces. *National Defence College E-Journal, 5*(1), 149–172. https://ndcjournal.ndc.gov.bd/ndcj

Nowakowski, W. (2025). Social engineering analysis framework: A comprehensive playbook for human hacking. *IEEE Access, 13*, 1–20. https://doi.org/10.1109/ACCESS.2025.3532999

Ormrod, A., Ormrod, D., & Slay, J. (2023). Cyber offensive operations in hybrid warfare: Observations from the Russo-Ukrainian conflict. *Journal of Information Warfare, 22*(1), 61–75.

Parmadi, B. D., & Ramli, K. (2026). Beyond silos – Unifying military and civilian cyber threat intelligence for national security. *International Journal on Perceptive and Cognitive Computing, 12*(1), 34–46. https://doi.org/10.31436/ijpcc.v12i1.575

Rurak, A., & Goniewicz, K. (2024). Enhancing security measures for military air bases – Integrating advanced technologies and operational strategies. *National Security Studies, 34*, 57–75. https://doi.org/10.37055/sbn/191446

Staněk, D., Klaban, I., & Coufalíková, A. (2025). *Explainable artificial intelligence: State of the art and beyond* (University research paper).

Takpah, N. E. A., & Oriakhi, V. N. (2025). Cybersecurity challenges and technological integration in military supply chain 4.0. *Journal of Information Security, 16*(1), 131–148. https://doi.org/10.4236/jis.2025.161007

Tschimben, S., Bates, I., Khairnar, R., Crosby, J., Curry, J. H., & Gremban, K. D. (2023). Military decoys for the digital age. In *2023 IEEE Military Communications Conference (MILCOM)* (pp. 761–766).

Tuli, E. A., Golam, M., Somrat, M. M. H., Khafagy, R., & Kim, D. S. (2025). Hybrid quantum machine learning for detecting GPS spoofing attacks in military mission. *ICT Convergence Research Center Paper*, 1–6.

## 5.13 Chapter 2 Alignment Checklist

| Chapter 2 requirement | Covered in this report |
|---|---|
| Background and relevance | Sections 5.0 and 5.11 |
| Search strategy and information sources | Section 5.2 |
| Inclusion and exclusion criteria | Section 5.2 |
| Literature analysis table | Section 5.3 |
| Comparison of existing techniques | Section 5.4 |
| Summary of methods and algorithms | Section 5.5 |
| Relevant datasets and tools | Section 5.6 |
| Evaluation metrics | Section 5.7 |
| Research gap analysis | Section 5.8 |
| Proposed methodology support | Sections 5.9 and 5.10 |
| References | Section 5.12 |