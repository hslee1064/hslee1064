# Hyunsik Lee - Machine Learning Engineer Portfolio

Welcome! This repository serves as my professional portfolio showcasing key projects and technical work. I am a Machine Learning Engineer with extensive experience in LLM systems, agentic AI, RAG, MLOps, Kubernetes infrastructure, and GPU-accelerated computing.

## Professional Summary

Machine Learning Engineer at Samsung Electronics with 2+ years of specialized experience building enterprise-scale AI systems. Previously at Kakao Enterprise (3+ years) where I developed MLOps platforms serving 200+ organizations. Strong background in:

- **LLM & Agentic Systems**: Multi-agent orchestration, prompt engineering, ReAct/CoT techniques
- **RAG (Retrieval-Augmented Generation)**: Hybrid search, semantic ranking, vector databases
- **MLOps & Infrastructure**: Kubernetes, ArgoCD, Helm, GPU cluster management, distributed inference
- **ML Model Serving**: Triton Inference Server, TensorFlow Serving, optimization techniques
- **Cloud Platforms**: AWS, Google Cloud, Azure, Samsung internal infrastructure

## Featured Projects

### 1. 🏢 AI Playground (2025.03 - Present)
**Organization**: Samsung Research AI Center  
**Role**: Machine Learning Engineer  
**Status**: Production - Serving 7,000+ employees across 28 countries

Enterprise-grade AI productivity platform leveraging Samsung's Gauss LLM to deliver secure, personalized AI assistants for employees.

**Key Contributions**:
- Designed multi-agent infrastructure for orchestrating complex AI workflows
- Managed Kubernetes deployment pipelines using ArgoCD and Helm
- Built Knowledge Repository service with document intelligence capabilities
- Implemented secure multi-cluster monitoring system (coordinated with Samsung Research Philippines)
- Developed MCP (Model Context Protocol) integration for enhanced tool access

**Technologies**: Kubernetes, ArgoCD, Helm, Python, LangChain, PostgreSQL, Redis

---

### 2. 📊 Big Data Assistant (2023.11 - 2025.02)
**Organization**: Samsung Electronics, LLMOps Team  
**Role**: Machine Learning Engineer  
**Status**: Production - 30 countries, 215+ analysts

Advanced AI service enabling data-driven decision-making through natural language interfaces.

**Key Achievements**:
- Built GPU infrastructure collaboration with Samsung SDS, Google Cloud, and Azure teams
- Developed LLM Gateway with token-based access control and audit logging
- Optimized AI agents using Chain-of-Thought (CoT) and ReAct techniques
- Created BDA Studio LLMOps platform for model evaluation and deployment
- **Results**: 27% reduction in analysis time, 84% SQL generation accuracy, 25.7% cost reduction

**Technologies**: Python, Kubernetes, Google Cloud, Azure, LangChain, Llama Index, MongoDB

---

### 3. 🔬 Kakao i Machine Learning (KiML) (2022.04 - 2023.08)
**Organization**: Kakao Enterprise, ML Platform Team  
**Role**: Machine Learning Engineer  
**Status**: Production - 200+ organizations, $8.11M revenue

Commercial MLOps platform for AI model deployment and management.

**Key Contributions**:
- Led design of modular inference architecture (Model-Deployment-Endpoint)
- Developed secure inference gateway with enterprise-scale features
- Managed 2,000+ GPU cluster with InfiniBand interconnect
- Implemented MIG (Multi-Instance GPU) monitoring and visualization
- Supported KakaoBrain's large-scale LLM research

**Key Metrics**:
- 11x faster training speed vs traditional systems
- 120% improvement in GPU utilization efficiency
- Selected as core infrastructure provider for Korea's national HPC initiative

**Technologies**: Kubernetes, InfiniBand, Prometheus, Grafana, TensorFlow Serving, PyTorch, ONNX

---

### 4. 🧠 OASYS - Knowledge Graph Construction (2020.06 - 2022.03)
**Organization**: Kakao Enterprise, Knowledge Graph AI Team  
**Role**: Machine Learning Engineer

Automated system for constructing knowledge graphs from unstructured Korean text using NER, Entity Linking, and Relation Extraction models.

**Key Contributions**:
- Optimized inference pipelines: **10x latency reduction** using Triton Inference Server
- Enhanced data pipeline throughput: **40x improvement** through GPU optimization
- Implemented GPU-based autoscaling mechanism (presented at Korea Software Congress)
- Deployed semantic web technologies (RDF, ontology-based reasoning)

**Key Metrics**:
- 89.1% entity linking accuracy
- 57.8% relation extraction F1-score
- Real-world deployment: Kakao search, AI speakers, recommendation systems

**Technologies**: Python, Triton Inference Server, Hadoop, Keras, RDF/Semantic Web

---

### 5. ⚙️ Throughput-Based Autoscaler (TBA) (2022.03 - 2024.06)
**Organization**: Korea University, Distributed & Cloud Computing Lab  
**Role**: Graduate Researcher & Developer  
**Status**: Research → Production Implementation

Kubernetes autoscaling solution for ML microservices based on data processing throughput and message queue metrics. This work addresses the critical challenge of efficiently scaling ML inference pipelines with limited GPU resources.

**Research Problem**:
- Standard Kubernetes HPA (Horizontal Pod Autoscaler) relies solely on CPU/memory metrics, making it inadequate for ML workloads with GPU constraints
- GPU-bound ML services suffer from underutilization and bottlenecks when multiple models compete for limited resources
- Conventional autoscaling cannot identify which model is the bottleneck in multi-stage ML pipelines

**Key Contributions**:
- **Algorithm Design**: Developed throughput-based autoscaling algorithm that detects bottlenecks by monitoring queue lengths and model-specific processing throughput
- **Infrastructure**: Built real-time monitoring system using Prometheus, Redis Streams, and custom exporters for GPU and throughput metrics
- **Implementation**: Created Kubernetes Custom Controller (CRD) for automated, intelligent pod scaling
- **Validation**: Tested on OASYS knowledge graph pipeline with NER, Entity Linking, and Relation Extraction models

**Key Results**:
- **51.6% throughput improvement** vs standard HPA (8 GPU scenario)
- **42.3% improvement** with 6 GPUs, **17.4%** with 4 GPUs, demonstrating scalability benefits
- **Optimized GPU utilization**: All available GPUs actively used vs HPA only utilizing 30-40%
- **CPU efficiency**: TBA achieved 100% peak utilization vs HPA's 80% during same workload
- **Published**: Korea Software Congress 2023 - "ML Microservices Autoscaling Based on Message Queue and Real-Time Throughput on GPU Cluster"

**Technical Stack**:
- **Kubernetes**: Custom Controller, CRD, API extensions
- **Monitoring**: Prometheus, DCGM Exporter, Node Exporter, Grafana
- **Message Queue**: Redis Streams (ultra-low latency alternative to traditional MQ)
- **ML Pipeline**: NER, EL, RE models from Hugging Face & SpaCy
- **Cloud Platforms**: Tencent Kubernetes Engine (TKE), Google Kubernetes Engine (GKE)

**Architecture Highlights**:
- **Queue-aware scaling**: Monitors Redis Stream queue length at each pipeline stage
- **Throughput-based decisions**: Scales based on model's items/second capacity vs queue backlog
- **Multi-device support**: Intelligently allocates between CPU and GPU nodes based on workload
- **Real-time adaptation**: 10-second polling interval enables rapid response to load changes

**Thesis Contribution**:
Master's thesis: "ML 서비스의 데이터 처리량 기반 쿠버네티스 오토스케일링 기법" (Korea University, 2024)

**Technologies**: Kubernetes, Python, Prometheus, Redis, DCGM, Triton Inference Server, NLP Models

---

## Early Career Projects

### SportForAll (2016-10 to 2017-02)
Hybrid mobile application providing fitness and sports information. Led development team of 5 as technical lead. 1000+ downloads achieved before service discontinuation.
- **Technologies**: Android (Java), Spring, MySQL, AWS EC2
- **Role**: Development Team Leader

### WeddingBox (2014-06 to 2014-11)
Mobile app for wedding social networking and digital invitations. 500+ downloads achieved.
- **Technologies**: Android (Java)
- **Role**: Android Developer

### IPPS - Integrated Process Planning and Scheduling (2017-01 to 2017-12)
Research in manufacturing process optimization using meta-heuristic algorithms and deep learning.
- **Technologies**: Python, Keras, Meta-heuristic Algorithms, Reinforcement Learning
- **Organization**: Production Process Scheduling Lab, Hongik University

---

## Technical Skills

| Category | Skills |
|----------|--------|
| **AI/ML** | LLM, Agentic Systems, RAG, Chain-of-Thought, ReAct, Fine-tuning, Prompt Engineering |
| **Languages** | Python, Java, SQL, JavaScript, Bash |
| **Infrastructure** | Kubernetes, Docker, ArgoCD, Helm, AWS, Google Cloud, Azure |
| **ML Frameworks** | LangChain, Llama Index, Keras, TensorFlow, PyTorch |
| **Databases** | PostgreSQL, MySQL, Redis, Vector Databases, RDF |
| **DevOps/MLOps** | Prometheus, Grafana, EFK Logging, GPU Cluster Management, Triton Inference Server |
| **Cloud Services** | AWS (EC2, S3), Google Cloud Platform, Microsoft Azure, Samsung Internal Cloud |

---

## Education

**Master of Engineering in Artificial Intelligence**  
Korea University, Seoul (2022-2024)  
Thesis: ML Microservices Autoscaling Based on Processing Throughput on GPU Cluster

**Bachelor of Engineering in Computer Science**  
Hongik University, Seoul (2012-2020)  
Research: Integrated Process Planning and Scheduling (IPPS)

---

## Publications & Presentations

- **"ML Microservices Autoscaling Based on Message Queue and Real-Time Throughput on GPU Cluster"**  
  Korea Software Congress (KSC) 2023 | [Publication](https://github.com/hslee1064)

- **MongoDB Seminar Presentation**  
  BDA Project showcase - Database and data management community

---

## Notable Achievements

✅ **Samsung Electronics**: Leading infrastructure design for enterprise AI services (7,000+ users)  
✅ **Kakao Enterprise**: Generated $8.11M revenue through KiML platform commercialization  
✅ **Korea Software Congress**: Presented research on ML microservices autoscaling  
✅ **Kubernetes CKA**: Certified Kubernetes Administrator (Linux Foundation)  

---

## Contact

📧 **Email**: hyunsik1.lee@samsung.com | hslee1064@gmail.com  
💼 **LinkedIn**: [linkedin.com/in/hslee1064](https://linkedin.com/in/hslee1064)  
📱 **Phone**: +82-10-4696-1064  

---

## Notes for Recruiters

This portfolio includes:
- **Recent work** (2023-2025): Samsung Electronics - AI Playground, Big Data Assistant
- **MLOps expertise** (2020-2023): Kakao Enterprise platform development
- **Technical depth**: GPU infrastructure, Kubernetes, distributed systems
- **Research background**: Master's thesis on ML autoscaling

For detailed information on specific projects or technical discussions, feel free to reach out. I'm happy to discuss system design, ML infrastructure, or any aspect of the projects listed above.

---

*Last updated: 2025-06-16*
