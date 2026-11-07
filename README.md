# Profile

Software Engineer and AI/ML Engineer with 7+ years of industry experience building secure, scalable backend systems for large-scale financial services and developing AI-driven solutions for digital banking and eKYC.

I previously worked on mobile banking platforms serving 9M+ users, with hands-on experience in core banking features including card-to-card transfers, card balance inquiry, bill payment by card, mobile top-up, internet package purchase, card-based payment flows, and account services.

I am currently working as an AI/ML Engineer in the Digital Banking Platform team, focusing on face verification, eKYC, computer vision, model benchmarking, and AI components for digital banking systems.

My background combines Java backend engineering, microservices, system design, AI research, computer vision, and deep learning. I am especially interested in building intelligent, reliable, and production-ready systems for FinTech, healthcare technology, and AI-driven digital products.

---

## Research Interests

* Medical Image Analysis and Multimodal Neuroimaging
* Generative AI and Latent Diffusion Models
* Deep Learning and Computer Vision
* Image Segmentation and Spatial Representation Learning
* Statistical Model Evaluation and Reliable AI
* Clinical Applications of Machine Learning
  
---

## Education

**M.Sc. in Artificial Intelligence**  
_[Yazd University](https://yazd.ac.ir/en), Yazd, Iran_ | 2016 – 2019

* **Thesis:** _Brain Tumor Segmentation Using Convolutional Neural Networks in MR Images_
  * Developed a 2D CNN based on a modified U-Net architecture
  * Dataset: BRATS 2018 Challenge
  * Achieved Dice scores: 0.887 for whole tumor, 0.806 for tumor core, and 0.781 for enhancing tumor
  * Ranked under the name “AfN” on the [BRATS 2018 Leaderboard](https://www.cbica.upenn.edu/BraTS18/lboardValidation.html)

**B.Sc. in Computer Engineering**  
_[Isfahan University of Technology](https://english.iut.ac.ir), Isfahan, Iran_ | 2009 – 2014

* **Thesis:** Enhancing Snort Intrusion Detection System with Anomaly Detection

---

## Professional Experience

### AI/ML Engineer  
_Digital Banking Platform, TID Development Co._ | May 2026 – Present

* Working as an AI/ML Engineer in the Digital Banking Platform team, focusing on AI-driven solutions for digital banking and identity verification.
* Developing and evaluating computer-vision and deep-learning components for video-based electronic Know Your Customer (eKYC) workflows.
* Building benchmark frameworks to evaluate face verification models based on accuracy, FAR, FRR, EER, TAR@FAR, FPS, model size, and deployment readiness.
* Working on face verification, head-pose analysis, challenge-response validation, and passive liveness detection.
* Built an LFW-based face-verification evaluation pipeline to examine similarity distributions and thresholds across assurance levels, with reproducible CSV/JSON/NPZ outputs.
* Implementing Python-based inference services with FastAPI, OpenCV, and ONNX Runtime, with attention to configuration, testing, and operational readiness.
* Collaborating with engineering and product teams on integration into digital banking services.

### Software Developer  
_Mobile Banking Platform, TID Development Co._ | May 2020 – Apr 2026

* Developed and maintained secure Java and Spring Boot REST services for a mobile banking platform serving more than 9 million users.
* Worked on core mobile banking features including:
  * Card-to-card money transfer
  * Card balance inquiry
  * Bill payment using bank cards
  * Mobile top-up purchase
  * Internet package purchase
  * Card-based payment flows
  * Account-related services and account information flows
* Designed and maintained RESTful backend APIs using Java and Spring Boot.
* Contributed to high-throughput financial services handling 600+ TPS in core banking scenarios.
* Participated in the design and optimization of backend services for reliability, performance, and scalability.
* Worked with microservices, Oracle, SQL Server, Redis, RabbitMQ, Docker, Jenkins, Prometheus, and Grafana.
* Integrated monitoring and observability tools to support real-time diagnostics and operational visibility.
* Improved deployment and delivery workflows using CI/CD practices.
* Collaborated with product, mobile, backend, QA, and infrastructure teams to deliver production banking features.

### .NET Developer  
_TID Development Co._ | May 2019 – Apr 2020

* Contributed to backend systems in the financial-services domain.
* Worked on enterprise systems including Anti-Money Laundering and Facilities Management systems.
* Developed and maintained backend services using C# and .NET technologies.
* Collaborated with banking-domain teams to support business-critical internal systems.

### .NET Developer  
_Kasra Co._ | 2018 – 2019

* Developed financial and administrative backend systems.
* Worked on enterprise software solutions using C# and .NET.
* Participated in backend development, database integration, and business logic implementation.

### C# Developer  
_Behko Co._ | 2014 – 2016

* Delivered customized software solutions for enterprise operations.
* Developed and maintained C# applications for business process improvement.
* Worked on software design, implementation, debugging, and support.
  
---

## Selected Projects

### Diffusion-Derived Latent Deviation Mapping — BraTS 2024

**Independent research | Sep 2026 – Present**
**Topics:** Multimodal Brain MRI · 3D Latent Diffusion · DDIM · Spatial Analysis · Statistical Evaluation
Developed a reproducible 3D latent-diffusion pipeline to investigate whether diffusion-derived latent deviation features carry spatial information associated with brain tumor pathology, without using segmentation masks during feature generation.
* Used **BraTS 2024 Adult Glioma Post-Treatment v2** (1,350 cases; fixed 1,080/270 train/development-validation split).
* Implemented train-derived latent normalization, deterministic DDIM reconstruction, whole-volume sliding-window inference, exact latent-to-voxel correspondence, and support-aware aggregation.
* Performed case-level statistical analysis using bootstrap confidence intervals, Wilcoxon tests, and Holm correction.
* Observed **median Whole Tumor AUROC 0.614 [0.606, 0.621]; 252/270 cases (93.3%)** had higher median deviation in tumor-containing latent cells than in clean background.
* Interpreted findings as a modest but consistent spatial association, not evidence of established diagnostic or segmentation performance.

**Code:** [brain-tumor-normative-diffusion](https://github.com/AfsanehNarimani/brain-tumor-normative-diffusion)

### Face Verification Benchmark for eKYC

Built a Python-based benchmark framework for evaluating face verification models in an eKYC-like scenario.

The goal was to compare multiple face recognition models and select a suitable candidate for an eKYC MVP based on accuracy, security, runtime performance, model size, and deployment readiness.

**Models evaluated:**

* ArcFace
* MobileFaceNet
* GhostFaceNet
* EdgeFace
* FaceNet
* AdaFace

**Evaluation metrics:**

* Accuracy
* FAR — False Accept Rate
* FRR — False Reject Rate
* EER — Equal Error Rate
* TAR@FAR
* FPS
* Model size
* Weighted decision score

**Result:**

EdgeFace was selected as the initial candidate for the eKYC MVP due to its balance between accuracy, security metrics, small model size, and CPU-friendly deployment.

**Technical stack:**

* Python
* ONNX Runtime
* InsightFace
* OpenCV
* NumPy
* Pandas
* Pytest
* Ruff
* Black
* Excel report generation

---

### Mobile Banking Backend Services

Worked on backend services for a production mobile banking platform used by millions of users.

Main areas included:

* Card services
* Account services
* Payment flows
* Financial transaction APIs
* High-throughput backend services
* Monitoring and operational diagnostics
* Microservice-based backend architecture

Key features included:

* Card-to-card transfer
* Card balance inquiry
* Bill payment by card
* Mobile recharge / top-up purchase
* Internet package purchase
* Account information services
* Secure REST API development

This experience strengthened my skills in financial-service backend engineering, scalable system design, API reliability, monitoring, and production-grade software development.

---

### Brain Tumor Segmentation Using CNNs

Implemented deep learning models for automated brain tumor segmentation in MRI images as part of my M.Sc. thesis.

* Developed a modified U-Net architecture
* Trained and evaluated on the BRATS 2018 dataset
* Focused on segmentation of whole tumor, tumor core, and enhancing tumor regions
* Results were benchmarked on the BRATS 2018 leaderboard under the name “AfN”

This project strengthened my background in medical image analysis, deep learning, and computational oncology.

---

## Research Experience

### Research Assistant  
[NeurAITex — NeurAI Tech Medical Innovation](https://www.linkedin.com/company/neuraitex/about/) | 2025 – Present

* Conducting research on AI-driven medical imaging and deep learning applications in neurology and neurosurgery
* Exploring MRI analysis and computer vision techniques for improving diagnostic accuracy and surgical outcomes
* Collaborating with engineering and medical students in a multidisciplinary research environment at the University of Tehran
* Contributing to the design of intelligent algorithms and AI-powered healthcare systems

---

## Entrepreneurial & Innovation Interests

* Engineering solutions for healthcare technology
* AI-driven product development and commercialization
* FinTech innovation and digital transformation
* Digital banking and intelligent financial services
* eKYC, identity verification, and applied computer vision
* Venture creation and lean startup methodologies

---

## Technical Skills

* **Research / ML:** Medical image analysis, multimodal brain MRI, image segmentation, latent diffusion, model evaluation, bootstrap-based evaluation
* **AI/ML Frameworks:** PyTorch, TensorFlow, Keras, scikit-learn, OpenCV, ONNX Runtime, NumPy, Pandas, FastAPI
* **Programming:** Python, Java, C++, C, C#, MATLAB
* **Backend Engineering:** Java, Spring Boot, REST APIs, Microservices, API Design
* **Databases:** Oracle, SQL Server, Redis
* **Infrastructure & Observability::** Docker, Jenkins, CI/CD, Prometheus, Grafana
* **Methodologies:** Agile, Scrum, Clean Architecture, Test-Driven Development

---

## Certificates

* [Machine Learning Specialization - Coursera](https://www.coursera.org/account/accomplishments/specialization/certificate/YPIGDYEAF3JB)
* [Data Structures and Performance - Coursera](https://www.coursera.org/account/accomplishments/certificate/ZNV8LKNSR5KT)

---

## Languages

* **Persian / Farsi:** Native
* **English:** Professional working proficiency
* **French:** Beginner
