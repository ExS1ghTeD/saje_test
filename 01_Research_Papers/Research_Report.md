# Research Papers for the Proposed Face Biometric Security System

> **Mock literature review:** The paper details below are illustrative research-paper summaries prepared to demonstrate the expected structure for Chapter 2. Verify the bibliographic details, results, datasets, and citations against the original publications before submitting the research proposal.

## 2.1 Literature Review Overview

Face biometric authentication identifies or verifies a person using facial characteristics. The literature shows a progression from handcrafted image features and statistical classifiers toward deep convolutional neural networks, embedding-based recognition, and privacy-aware edge systems.

The proposed research focuses on a face biometric security system that should be accurate, resistant to presentation attacks, and practical to deploy. The selected papers therefore cover four related concerns:

- face representation and recognition accuracy;
- performance under changes in lighting, pose, and facial expression;
- liveness detection and protection against spoofing; and
- privacy, fairness, and resource constraints in real-world deployment.

## 2.2 Summary of Important Research Papers

### Paper 1: DeepFace

| Item | Research-paper information |
|---|---|
| **Paper Title** | *DeepFace: Closing the Gap to Human-Level Performance in Face Verification* |
| **Author(s)** | Yaniv Taigman, Ming Yang, Marc'Aurelio Ranzato, and Lior Wolf |
| **Year** | 2014 |
| **Research Problem** | The study investigated how to improve face verification accuracy when images contain differences in pose, illumination, expression, and image quality. |
| **Method / Technique** | A deep neural network was trained to produce discriminative facial representations. The approach used a 3D face-alignment step followed by a deep convolutional neural network and face verification using the similarity between learned representations. |
| **Dataset / Tools** | A large-scale face dataset collected from online images and the Labeled Faces in the Wild (LFW) benchmark. |
| **Main Findings** | The alignment and learned representation substantially improved verification performance and achieved results close to human-level performance on the reported benchmark. |
| **Limitation** | The approach required a large training set and considerable computational resources. Its performance may also decrease when faces are heavily occluded, captured at extreme angles, or recorded with low-quality cameras. |
| **Relevance to Proposed Research** | This paper supports the use of face alignment and learned feature representations as the recognition foundation. It also shows why a security system must test more than clear, front-facing images. |

### Paper 2: FaceNet

| Item | Research-paper information |
|---|---|
| **Paper Title** | *FaceNet: A Unified Embedding for Face Recognition and Clustering* |
| **Author(s)** | Florian Schroff, Dmitry Kalenichenko, and James Philbin |
| **Year** | 2015 |
| **Research Problem** | The research addressed the need for a face-recognition system that can represent identity efficiently while supporting verification, identification, and clustering. |
| **Method / Technique** | A deep convolutional network learned a compact Euclidean embedding using triplet loss. Images of the same person were pushed closer together in the embedding space, while images of different people were separated. |
| **Dataset / Tools** | Large-scale internal face collections and the LFW and YouTube Faces benchmarks. Training used deep-learning hardware and a triplet-mining strategy. |
| **Main Findings** | The embedding could be used for several face-recognition tasks with a simple distance threshold. The method reported strong verification and clustering performance while using a compact representation. |
| **Limitation** | Training triplets effectively is difficult and computationally expensive. The correct threshold can vary with the operating environment, camera quality, and the security level required. |
| **Relevance to Proposed Research** | The proposed system can use an embedding-and-distance architecture instead of storing raw face images for every comparison. The paper also provides a basis for selecting and evaluating a verification threshold. |

### Paper 3: ArcFace

| Item | Research-paper information |
|---|---|
| **Paper Title** | *ArcFace: Additive Angular Margin Loss for Deep Face Recognition* |
| **Author(s)** | Jiankang Deng, Jia Guo, Niandong Xue, and Stefanos Zafeiriou |
| **Year** | 2019 |
| **Research Problem** | The study investigated how to make identities more separable in a deep face-recognition feature space and improve recognition under difficult image conditions. |
| **Method / Technique** | Additive angular margin loss was introduced to increase the angular separation between classes. The method normalised features and classifier weights so that identity discrimination could be learned on a hypersphere. |
| **Dataset / Tools** | Training and evaluation were conducted using large-scale face datasets and standard benchmarks such as LFW, CFP-FP, AgeDB, and MegaFace. |
| **Main Findings** | The angular-margin objective produced highly discriminative face embeddings and achieved strong results across multiple face-recognition benchmarks. |
| **Limitation** | The approach depends on large, diverse, and correctly labelled training data. Demographic imbalance, noisy labels, and domain differences between training and deployment data can still produce unequal error rates. |
| **Relevance to Proposed Research** | This paper supports using a modern margin-based embedding model for the recognition stage. It also highlights the need to report performance separately across different conditions and user groups rather than relying on one overall accuracy value. |

### Paper 4: Face Anti-Spoofing with Depth and Motion Cues

| Item | Research-paper information |
|---|---|
| **Paper Title** | *Learning Deep Models for Face Anti-Spoofing with Depth and Motion Cues* |
| **Author(s)** | Rui Shao, Xiangyuan Lan, and Pong C. Yuen |
| **Year** | 2019 |
| **Research Problem** | The research addressed presentation attacks in which an attacker presents a photograph, replayed video, or mask to a face-recognition camera. |
| **Method / Technique** | A deep anti-spoofing model learned complementary spatial, depth, and temporal information. Motion and depth cues were used to distinguish a live three-dimensional face from a flat or replayed presentation. |
| **Dataset / Tools** | Face anti-spoofing benchmarks such as CASIA-FASD and Replay-Attack, together with RGB video input and model-training software. |
| **Main Findings** | Combining appearance with depth or motion cues was more reliable than using a single still-image classifier for several common presentation attacks. |
| **Limitation** | The model may not generalise to unseen attack materials, new cameras, or different lighting conditions. Additional sensors can also increase system cost and reduce ease of deployment. |
| **Relevance to Proposed Research** | This paper establishes that recognition alone is insufficient for a secure biometric system. The proposed design should include a liveness or anti-spoofing stage and test attacks that were not included during training. |

### Paper 5: Face Anti-Spoofing in the Wild

| Item | Research-paper information |
|---|---|
| **Paper Title** | *Face Anti-Spoofing in the Wild: How to Generate and Adapt to Unknown Attacks* |
| **Author(s)** | Yousef Atoum, Yaojie Liu, Amit Joshi, and Xiaoming Liu |
| **Year** | 2017 |
| **Research Problem** | The study examined why anti-spoofing models trained in controlled environments often fail when exposed to unknown attacks and uncontrolled real-world conditions. |
| **Method / Technique** | A deep model combined facial appearance information with depth-related cues. The work also considered domain variation and the challenge of adapting a detector to attacks that were not present in the training data. |
| **Dataset / Tools** | Public face anti-spoofing datasets, RGB video frames, face detection, and deep-learning tools. |
| **Main Findings** | Depth-aware and domain-aware representations improved the detection of several spoofing conditions compared with relying only on colour or texture information. |
| **Limitation** | No anti-spoofing method can guarantee detection of every future attack. Performance remains sensitive to the quality of the camera and to differences between the training and deployment environments. |
| **Relevance to Proposed Research** | The findings support an evaluation plan that includes cross-dataset or unseen-attack testing. This makes the proposed security claims more realistic than reporting accuracy on one familiar dataset. |

### Paper 6: Fairness and Demographic Effects in Face Recognition

| Item | Research-paper information |
|---|---|
| **Paper Title** | *Gender Shades: Intersectional Accuracy Disparities in Commercial Gender Classification* |
| **Author(s)** | Joy Buolamwini and Timnit Gebru |
| **Year** | 2018 |
| **Research Problem** | The paper investigated whether commercial facial-analysis systems perform equally across gender and skin-tone groups. |
| **Method / Technique** | The researchers created a benchmark with balanced representation and measured classification error across intersectional demographic groups. |
| **Dataset / Tools** | The Pilot Parliaments Benchmark (PPB) and commercial gender-classification systems. |
| **Main Findings** | The reported systems showed substantially different error rates across demographic groups, with the highest errors affecting darker-skinned women in the tested task. |
| **Limitation** | The benchmark focused on gender classification rather than face verification or authentication. Results may also change as commercial systems and datasets are updated. |
| **Relevance to Proposed Research** | The paper supports fairness testing as part of system evaluation. The proposed research should report false acceptance and false rejection rates by relevant demographic and environmental conditions where the dataset permits. |

### Paper 7: Privacy-Preserving Face Recognition

| Item | Research-paper information |
|---|---|
| **Paper Title** | *DeepPrivacy: A Generative Adversarial Network for Face Anonymization* |
| **Author(s)** | Mats L. B. Sørensen, Mads L. B. Sørensen, and colleagues |
| **Year** | 2020 |
| **Research Problem** | The research considered how to protect facial identity in images while preserving useful visual information for analysis and system development. |
| **Method / Technique** | A generative adversarial network generated synthetic replacement faces conditioned on non-identifying information such as body pose, segmentation, and scene context. |
| **Dataset / Tools** | Face datasets containing people in varied scenes, image segmentation, and generative-adversarial-network training tools. |
| **Main Findings** | Synthetic face replacement can reduce direct identity exposure while retaining much of the surrounding image structure and pose information. |
| **Limitation** | Anonymisation is not the same as full privacy protection. Generated images can contain artefacts, and biometric identity may still be inferred from information outside the replaced face. |
| **Relevance to Proposed Research** | The paper supports a privacy-by-design discussion. The proposed system should minimise raw-image storage, protect templates, define retention rules, and explain how biometric data will be secured. |

## 2.3 Cross-Paper Comparison

| Research concern | Evidence from the literature | Design implication for the proposal |
|---|---|---|
| Recognition accuracy | DeepFace, FaceNet, and ArcFace show the value of alignment and discriminative deep embeddings. | Use a face detector/alignment stage and compare embeddings using a calibrated threshold. |
| Environmental variation | Pose, lighting, expression, camera quality, and occlusion affect recognition results. | Evaluate the system using more than clear, front-facing images. |
| Presentation attacks | Anti-spoofing studies show that photographs and replayed videos can bypass recognition-only systems. | Add liveness detection and include unseen-attack testing. |
| Generalisation | Results on a controlled dataset may not transfer to a new camera or environment. | Separate training, validation, and test data and document the deployment conditions. |
| Fairness | Error rates may differ across demographic groups. | Report subgroup results and identify data-collection limitations. |
| Privacy | Face images and templates are sensitive biometric information. | Prefer protected templates, limited retention, access control, and explicit user consent. |

## 2.4 Research Gap

The reviewed studies provide strong techniques for face representation and anti-spoofing, but they often evaluate one component in isolation or rely on large controlled datasets. There is a practical gap in combining recognition, liveness detection, threshold calibration, privacy protection, and fairness evaluation in one lightweight system suitable for a constrained deployment environment.

The proposed research addresses this gap by designing and evaluating an integrated face biometric security system. The evaluation will consider both recognition performance and security performance, including false acceptance rate, false rejection rate, equal error rate, liveness detection performance, processing time, and behaviour under changes in lighting, pose, and presentation attack type.

## 2.5 Proposed Evaluation Measures

| Measure | Purpose |
|---|---|
| Accuracy | General measure of correct predictions; should not be used alone for security claims. |
| False Acceptance Rate (FAR) | Measures how often an unauthorised person is incorrectly accepted. |
| False Rejection Rate (FRR) | Measures how often an authorised person is incorrectly rejected. |
| Equal Error Rate (EER) | Indicates the threshold at which FAR and FRR are equal. |
| Attack Presentation Classification Error Rate (APCER) | Measures how often spoof presentations are classified as genuine. |
| Bona Fide Presentation Classification Error Rate (BPCER) | Measures how often genuine presentations are classified as attacks. |
| Inference time | Measures whether the system is practical for near-real-time authentication. |
| Subgroup performance | Compares performance across relevant demographic and environmental conditions. |

## 2.6 Chapter Summary

The literature indicates that deep face embeddings can provide strong recognition performance, but recognition accuracy alone does not establish biometric security. A complete system must also address presentation attacks, domain variation, unequal performance, and the privacy risks of storing facial data. These findings guide the proposed research toward an integrated, measurable, and privacy-aware face biometric security system.