<h1 align="center">Razieh Moradi</h1>

<p align="center">
  <b>Researcher · AI and LLM Security</b><br>
  Cyber Science Lab &nbsp;·&nbsp
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/razieh-moradi-b23614170/"><img src="https://img.shields.io/badge/LinkedIn-Razieh%20Moradi-0A66C2?style=flat-square" alt="LinkedIn"></a>
  <a href="https://scholar.google.com/citations?user=aznI2l0AAAAJ"><img src="https://img.shields.io/badge/Google%20Scholar-Publications-4285F4?style=flat-square" alt="Google Scholar"></a>
  <a href="mailto:moradr1@mcmaster.ca"><img src="https://img.shields.io/badge/Email-moradr1%40mcmaster.ca-D14836?style=flat-square" alt="Email"></a>
  <img src="https://img.shields.io/badge/Based%20in-Toronto%2C%20Canada-111111?style=flat-square" alt="Toronto">
</p>

---

### About

I study how large language models fail, and how to measure that failure honestly.

I am a researcher at the Cyber Science Lab at the University of Guelph, where I have worked since September 2025 with Dr. Fattane Zarrinkalam, Dr. Ali Dehghantanha, and Dr. Havva Alizadeh Noughabi. My work sits where probability theory, adversarial machine learning, and security meet, and most of it comes down to one question: when a defense reports that it worked, what exactly did it prevent?

My route here was not the usual one. I hold two master's degrees, one in Systems and Technology from McMaster University and one in Industrial Engineering by thesis, and before research I spent eight years coordinating enterprise systems delivery for the National Iranian Oil Company, a multi year ERP implementation with Arthur D. Little as implementation partner. That work left me with a systems engineer's instinct for how complex systems actually break once real people and real incentives are attached to them. I now point that instinct at language models.

### Research

**Multi turn jailbreak attacks and defense evaluation**
Built a local red teaming and evaluation pipeline on garak, PyRIT, and llama.cpp that runs adaptive multi turn attacks against six published defenses, including SmoothLLM, Self Reminder, Goal Prioritization, Llama Guard, PARDEN, and Intention Analysis, across four open model families. Produced and analyzed a human scored corpus of 36,000 defended conversation rounds, scoring each round for current harm and forward looking residual risk rather than a binary jailbreak label, with a benign over refusal gate for utility. Defenses are compared with paired bootstrap and sign flip permutation tests under Holm correction, verified by a blinded expert audit, through a React annotation console I built for multi expert scoring.

**RAG security and knowledge poisoning**
Showed that the internal representations of cross encoder rerankers carry signals separating poisoned passages from clean ones, and used those signals to detect knowledge poisoning attacks on retrieval augmented generation pipelines. Built poisoned retrieval corpora on HotpotQA, MS MARCO, and Natural Questions for robustness testing.

**Topological backdoor detection**
A controlled study of whether persistent homology features of layer activations detect backdoor inputs better than plain distance statistics, using class conditional controls and paired comparisons of the same images with and without the trigger. Retrained clean and backdoored ResNet18 models on CIFAR10, reaching about 94.5 percent clean accuracy with 99.4 percent attack success on the backdoored model, and am now designing a topological detector evaluated under both heavy and very low contamination.

**Escalation forecasting**
Trajectory level safety risk forecasting on the scored multi turn corpus, so that a dangerous conversation trajectory is flagged before harm occurs. A first step toward classifiers that detect escalation in progress and an adaptive defense controller.

**Self healing knowledge constrained AI systems**
A longer research program in three phases: knowledge graph and code behaviour guided fault localization for separating malicious from benign prompts, a reinforcement learning defense that enforces knowledge graph constrained policies while preserving utility and factuality, and teacher student distillation to carry those capabilities into lightweight models for resource constrained deployment.

### Publications

**Defending RAG Against Knowledge Poisoning Using Cross-Encoder Activation Signals**
R. Moradi, H. Alizadeh Noughabi, F. Zarrinkalam, A. Dehghantanha.
Canadian AI 2026, 39th Canadian Conference on Artificial Intelligence, oral presentation.
Proceedings of Machine Learning Research, vol. 318, 2026. [Paper](https://proceedings.mlr.press/v318/moradi26a.html)

Further manuscripts in progress on multi turn jailbreak evaluation and topological backdoor detection.

### Service

- Program Committee, AutonomousCyber 2026 workshop at ESORICS 2026
- Reviewer, ICLR 2027 · ECIR 2027 · IEEE Internet of Things Journal, 2026 · CEEA-ACEG 2025
- Organizer, SECURE-AGRO workshop at PST 2026, Ottawa, on behalf of the Cyber Science Lab
- Author of the accepted workshop proposal for IEEE CCECE 2027, now confirmed on the conference program

### Selected engineering work

**LunaNet-DX, electric vehicle charging load forecasting** · Burlington Hydro Inc.
Identified electric vehicle ownership across a dataset of more than 68,000 households, then designed a custom attention based architecture for forecasting charging loads, with interactive dashboards supporting utility infrastructure planning.

**Pneumonia detection by teacher student knowledge distillation**
A lightweight student CNN detecting pneumonia from chest radiographs, distilled from a larger teacher model. Reached 92.56 percent recall and 90.36 AUC-ROC, outperforming a fine tuned ResNet-50.

**Fine tuning large language models under GPU constraints**
Fine tuned GPT-2 XL, DeepSeek R1-Qwen, LLaMA-3, Mistral-7B, and Gemma-3-4B on a dialogue corpus using LoRA and 4 bit quantization, then evaluated the results with an LLM as judge protocol.

**Hybrid RAG virtual teaching assistant** · McMaster University
A retrieval augmented generation and knowledge graph system for personalized learning and question answering in engineering education.

**IoT medication reminder and dispensing device** · McMaster University
A working hardware prototype that reminds users to take medication and dispenses it on schedule, donated to McMaster's medical school, where it remains in use.

### Toolbox

**Machine learning** Python · PyTorch · Hugging Face Transformers · scikit&nbsp;learn · NumPy · pandas · MATLAB
**Large language models** fine tuning, LoRA and 4 bit quantization, RAG pipelines, knowledge graphs, reinforcement learning, LLM as judge evaluation
**LLM security** garak · PyRIT · llama.cpp · adversarial ML, threat modelling, prompt injection and jailbreak analysis, data and knowledge poisoning, backdoor detection
**Natural language processing** spaCy · NLTK · Gensim · tokenizers
**Computer vision** OpenCV · torchvision · PIL · Albumentations · CNN classification, semantic segmentation, object detection, transformer based vision models
**Evaluation and statistics** paired bootstrap, permutation tests, Holm correction, inter rater agreement, topological data analysis and persistent homology, multivariate statistical methods
**Mathematics and operations research** probability, stochastic modelling, statistical inference, optimization, integer programming, queuing theory, fuzzy analytic network process
**Cloud and infrastructure** Google Cloud Vertex AI · AWS SageMaker · Docker · CUDA on local GPU workstations
**Enterprise systems** SAP, full cycle ERP implementation, fit gap analysis, user acceptance testing, business intelligence reporting

### Education

| Degree | Institution | Years |
|---|---|---|
| MEng, Systems Technology, Smart Systems and AI stream | McMaster University | 2024 to 2026 |
| MSc, Industrial Engineering, by thesis | University of Science and Culture, Tehran | 2014 to 2017 |
| BSc, Industrial Engineering, System Analysis | Islamic Azad University, Tehran | 2012 |

Graduate cumulative average of 11.57 on the 12 point scale at McMaster. Master's thesis: a multi objective programming model using the fuzzy analytic network process to optimize supplier and carrier selection in order allocation.

### Teaching

Teaching assistant in Statistical Methods and Integer Variable Programming, and in Advanced Statistical Methods, Computer Programming, and Multivariate Statistical Methods. I have mentored junior colleagues throughout my career, and informally supported international women students in McMaster's engineering program through the Machine Learning and Cloud Computing courses.

### Certifications

- Google Cloud Professional Machine Learning Engineer
- AWS Certified AI Practitioner

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Rosemoradi&show_icons=true&hide_border=true&theme=default" height="150" alt="GitHub stats">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Rosemoradi&layout=compact&hide_border=true&theme=default" height="150" alt="Top languages">
</p>

<p align="center"><i>Open to research collaboration on LLM security, adversarial evaluation, and trustworthy AI.</i></p>
