# Research Problem Areas in Computing and AI

This repository helps collect research questions in Computing and Artificial Intelligence and is intended as a resource for researchers, students, and educators looking for research project ideas. 

If you use or refer to this repository in your work, please cite it as follows:
> Rahul Kulkarni and contributors, Research Questions in Computing and AI. GitHub repository, 2025. Available at: https://github.com/rahul101001000/computing_ai_research

Contributions are welcome! If you have additional research questions to propose:
- Fork the repository
- Append your research problem statements to the end of the list
- Submit a Pull Request (PR) with a clear description of your addition

---

## 1. Privacy preserving algorithms for anonymization and aggregation of multi-modal data

**Background**
- Raw data e.g. prescriptions, test reports, Xrays, etc are used to create anonymized, consented patient journey records e.g. https://vaishnavimaguluri.blogspot.com/2023/07/general-medicine-case-report-osce.html. However the process of turning raw data into anonymized records is a manual, error prone painstaking one. The same is true with several data types e.g. publicly accessible reviews, business reports, et al.
- In this project we aim to uncover what algorithms best work for multi-modal (text, image, videos) anonymization and aggregation, especially with a view of meeting GDPR and DPDP requirements.

**Research questions**
- How can multi-modal medical data be anonymized effectively? (precision, recall)
- How efficient are anonymization algorithms? (speed, resource utilization)
- Which aggregation methods best preserve the value of anonymized data?

**Outputs**
- Scalable, open source, anonymization and aggregation tool for multi-modal medical data along the lines of remove.bg
- Benchmarks for effectiveness and efficiency of anonymization algorithms

---

## 2. Building a Compliant Data Economy: Operational Frameworks for Anonymization and Aggregation

**Background**
- Raw data e.g. prescriptions, test reports, Xrays, etc are used to create anonymized, consented patient journey records e.g. https://vaishnavimaguluri.blogspot.com/2023/07/general-medicine-case-report-osce.html. However the process of turning raw data into anonymized records is a manual, error prone painstaking one. The same is true with several data types e.g. publicly accessible reviews, business reports, et al.
- This project focuses on uncovering policies and operational best practices to streamline data handling and meet GDPR (https://gdpr.eu) and DPDP (https://www.dpdp.gov.in) requirements, while making data shareable and monetizable.     This will foster a compliant data economy that balances data utility, privacy, and business value.

**Research questions**
- How can innovative business models unlock new revenue opportunities by responsibly monetizing anonymized and aggregated data?
- What does the product development and operations cycle look like in the data economy?
- In what ways can organizations position themselves as policy leaders in ethical data practices to shape future regulatory developments?
- How can businesses streamline activities like data collection, consent adherence, revenue sharing and other practices in the data economy without burdening existing operations?

**Outputs**
- Comprehensive operational frameworks and policy guidelines for efficient, compliant data anonymization and aggregation.
- Benchmark reports outlining best practices for transforming raw data into valuable, aggregated data assets while ensuring regulatory compliance.

---

## 3. AI Model Training Using Confidential Containers

**Background**
- Confidential containers / Trusted Execution Environments enable the training of AI models without exposing raw or sensitive data to the model trainer.
- Frameworks such as https://depa.world/training/depa_training_framework, https://github.com/iSPIRT/depa-training/tree/main have been created to streamline data usage for AI without compromising on confidentiality.
- The project aims to validate secure and efficient model training that adheres to stringent data privacy standards.

**Research questions**
- How effective are confidential containers / Trusted environments in maintaining data isolation during AI model training?
- What performance trade-offs (e.g., speed, resource utilization) arise when using confidential computing compared to traditional methods?
- How can the DEPA training framework be further optimized to support a variety of AI models across multiple datasets?
- What are the regulatory, compliance, and governance implications of using confidential computing for AI training in sensitive sectors?

**Outputs**
- A playbook for AI model training based on confidential containers and the DEPA training framework for organizations with data.
- Benchmark reports detailing performance, security, and compliance metrics for the confidential computing approach to AI model training.

---

## 4. Authentication and Role-Based Access Control for Agentic AI and its Implications

**Background**
- Agentic AI systems require robust methods to authenticate agents and enforce role-based access control across diverse tasks and datasets.
- MCP and A2A have emerged the standards for agent to agent and agent to server communication. https://www.newsletter.swirlai.com/p/mcp-vs-a2a-friends-or-foes
- This project aims to understand the implications of using agentic AI with either  or a combination of MCP and A2A protocols on security and access of agentic AI systems.

**Research questions**
- How can integrating Model Context Protocol with A2A enhance security of inter-agent communications in agentic AI systems?
- What use cases emerge with agentic AI that can effectively and efficiently perform authentication and authorization?
- What mechanisms can be implemented to enforce fine-grained role-based access control, ensuring that agents only access the data and operations assigned to their roles?
- What is the performance impact (e.g., latency, throughput) of implementing these authentication and access control protocols in real-world AI systems?
- What potential security vulnerabilities and compliance challenges might arise from deploying this integrated framework at scale, and how can they be mitigated?

**Outputs**
- Implications of agentic AI on security assessment practices and user behavior
- Library of industry use cases requiring authentication and authorization with agentic AI
- Open source library/framework that implements authentication and role-based access control for agentic AI
- Benchmark reports detailing performance metrics, security enhancements, and compliance adherence of the developed library/framework.
- Comprehensive documentation and deployment guidelines to facilitate real-world adoption and integration into existing AI systems.

---

## 5. Observability for Indian AI Systems
**Background**
- Observability has always been a key part of any software system - whether to debug problems or to gain insights into usage. Mature observability systems - such as OpenTelemetry, PostHog, Matamo, Plausible, Open Web Analytics, Umami - have modular architectures with plugins and extensions that contributors use to enhance the functionality of the base product. Over time, a vast repository of plugins has been created, spanning various technologies, languages and use cases. 

**Gap**
- Observability in modern AI systems is critical for explainability, transparency and interpretability. However, traditional observability tools don’t work out of the box for AI systems because of the following reasons - 
- The content of API requests differ significantly (e.g. chain-of-thought trace) from traditional web requests (e.g. user-clicked-button events)
- Modern agentic AI systems are far more dynamic than traditional static web systems
- In developing regions with low internet speeds and high cost concerns, additional observability data may be required—data that traditional tools don’t provide.
- The range of languages, dialects, and domain-specific taxonomy covered by existing observability tools is narrow.
- Multimodal and multi-physical AI systems (including text, image, video, AR, and sensors) generate high-speed, diverse data that require additional fields and constructs for proper logging.

**Existing work in the Indian context**
- Several recent open-source and startup-driven product efforts aim to improve AI observability, e.g. OpenTelemetry, OpenObservability, Phoenix, Weights and Biases and Helicone. Additionally, collaborative standardization efforts exist, such as the OpenTelemetry Semantic Conventions for Generative AI, which define a structured approach to AI observability. However, most of these efforts focus primarily on the first gap (API request content differences), with only nascent work on gaps 2 and 5, and little to no work addressing gaps 3 and 4.

**Potential research questions**
- Extending Observability Frameworks: How can existing observability frameworks be modified to capture dynamic traces of agentic AI systems compared to traditional web-based systems?
- Contextual Adaptation for Low-Bandwidth Regions: What strategies can be developed to optimize observability for AI systems in regions with limited bandwidth, low resource devices and edge AI systems deployed in rural areas in India?
- Multilingual and Domain-Specific Support: How can observability tools be enhanced to support the linguistic diversity (languages, dialects, and domain-specific taxonomies) prevalent in India?
- Multimodal Data Logging: In what ways can observability frameworks be extended to effectively log and process high-speed, diverse data generated by multimodal AI systems (e.g., text, image, video, AR, sensor data)?
- Local Applications and Impact: How does improved observability influence the explainability, transparency, and interpretability of AI systems in critical local applications, such as healthcare, agriculture, or public governance in India?
- Integration with Existing Systems: How can real-time observability data be integrated with legacy systems or local infrastructures to enable effective monitoring and anomaly detection in AI applications used in India?
- Cost-Effective Implementation: What cost-effective, scalable models for implementing advanced observability in AI systems can be developed to meet the financial constraints often encountered in developing regions like India?

---

## 6. Database of Indian AI Safety Risks
**Background**
- Information provided or actions taken by AI systems may cause individual or societal harm due to hallucinations, jailbreaks and a variety of other causes that are characteristic of AI systems. While raw observability data may include harmful content (e.g. “women can’t do math”, “delete all files”), unless one has a clear definition of what data constitutes an AI safety risk, enabling detection and mitigation of these becomes prohibitive, given the scale of data passing through these systems. 

**Gap**
- Efforts such as MIT’s AI risk repository and NIST AI Risk Management Framework provide a clear causal and domain taxonomy and a database of risks. However, these are created using western sensibilities, societal beliefs, perceptions of harm and local country law. These miss out on - 
- Providing causal and domain taxonomy and a database of AI risks applicable to India (e.g. caste-based discrimination, tribal marginalization, religious polarization, misinformation, AI originated manipulative behavior)
- Mapping of risks to Indian Penal Code (e.g. section 153A on hate speech), Digital Personal Data Protection Bill 2023 (e.g. AI model trained on private data without consent) and Copyright Act 1957 (e.g. AI model outputting art similar to copyrighted work by an artist)
- Providing constructs to ensure the database is exhaustive including marginalized groups

**Existing work in the Indian context**
- India’s Responsible AI strategy document outlines various dimensions of AI safety and risks for India. Work by researchers in India document several risks associated with caste and gender bias. A recent think tank report provides a comprehensive analysis of AI regulation in India. The Asia Group’s report on AI governance in the Indo-Pacific provides proposals for the path ahead for countries in south-east Asia. While these offer a direction for Indian AI safety risks mentioned in 1, there is no such comprehensive AI safety risks database for India. Moreover, gaps 2 and 3 are not addressed at all by any existing work. 

**Potential research questions**
- AI Risk Taxonomy for India: How can an AI risk taxonomy be developed that captures culturally and legally relevant risks unique to India, such as caste-based discrimination, religious polarization, and tribal marginalization?
- AI Risk Taxonomy for India: How do AI safety risks in India compare with existing Western AI risk frameworks (e.g., NIST, MIT AI Risk Repository), and what modifications are required?
- Legal and Regulatory Mapping of AI Risks: How can AI-generated risks be systematically mapped to Indian laws, such as the Indian Penal Code (IPC), Digital Personal Data Protection Bill 2023, and Copyright Act 1957?
- Database Construction of AI Risks: How can a comprehensive AI risk database be built for India that is exhaustive, including perspectives from marginalized communities? 
- Database Updation of AI Risks: What methodologies can be used to ensure that the AI risk database stays updated with new and emerging AI risks in India?
- Societal and Ethical Considerations in AI Risk Management: What societal and ethical challenges arise when defining AI safety risks for diverse, multi-lingual populations in India? How can participatory AI governance models (involving citizens, NGOs, and policymakers) improve AI risk assessment frameworks in India?
- Practical Implementation: How can AI risk databases be integrated into existing AI governance systems used by Indian regulatory bodies and industry stakeholders? 
- Case studies: What case studies from real-world AI deployments in India highlight the most pressing AI safety risks, and how have they been managed?

---

## 7. Benchmarking AI models against India AI safety risks

**Background**
- Benchmarking is a common technique used to compare the effectiveness and efficiency of AI models. Given that an AI model may be good at certain tasks vs others, benchmarks exist around multiple dimensions such as SimpleQA, MATH, MMLU amongst numerous others. Open source frameworks such as Evals exist to facilitate measurement of these benchmarks. Leaderboards such as Vellum and LLM-stats provide results of all benchmarking tests in one place. 

**Gaps**
- All of the above referenced constructs are created by and for primarily US data and audience and are not around AI safety. MLCommon’s AILuminate is one benchmark specifically dedicated to AI safety. However, none of these are designed with the Indian context in mind - 
- No AI safety risks benchmarking data sets for India 
- No benchmarking framework or toolkit validated for AI safety use cases in India
- No benchmarking leaderboards for AI safety risks for India 
- No benchmarks for Indian foundational models or India enhanced foundational models against India AI safety risks

**Existing work** 
- Singapore’s AI Verify Toolkit provides a toolkit to benchmark LLMs for Singapore’s sensibilities of AI safety. There are papers around evaluating LLMs for algorithmic bias, however these don’t provide a comprehensive benchmark dataset that all LLMs can be benchmarked against. None of the gaps above are addressed currently. 

**Potential research questions** 
- Developing India-Specific AI Safety Benchmarking Datasets: What data sources and methodologies can be leveraged to develop a comprehensive AI safety risk benchmarking dataset tailored to India’s cultural, legal, and social contexts (e.g. real world incidents, local regulations)?
- Developing India-Specific AI Safety Benchmarking Datasets: How can a multilingual and multi-regional dataset be constructed to accurately reflect the spectrum of AI safety risks encountered in India (focus on dialectal variations and regional social issues)?
- Designing Benchmarking Frameworks and Toolkits: What modifications are required to adapt existing AI benchmarking frameworks (like Evals or AILuminate) to effectively evaluate AI safety risks within the Indian context? 
- Designing Benchmarking Frameworks and Toolkits: How can a new benchmarking toolkit be designed and validated specifically for assessing AI safety risks in India?
- Evaluating AI Model Performance on Safety Metrics: How do foundational AI models and their India-enhanced variants perform when benchmarked against AI safety risk datasets tailored for India?
- Evaluating AI Model Performance on Safety Metrics: What are the common failure modes of current AI models when subjected to benchmarks based on India-specific AI safety risks? (this would act as input to model creators) 
- Creating AI Safety Benchmark Leaderboards: What are the critical design parameters (e.g. metric standardization, data quality, and stakeholder engagement) for developing an open, transparent leaderboard that tracks AI safety risk benchmarks specifically for the Indian context? 
- Integration with Policy and Regulatory Frameworks: How can benchmarking results be mapped to Indian legal and regulatory requirements (e.g., hate speech, data privacy, copyright laws) to facilitate safer AI deployments?
- Integration with Policy and Regulatory Frameworks: What policy implications arise from benchmarking AI models against India-specific safety risks, and how can these findings influence the development of responsible AI governance in India?

---

## 8. Crowdsourced AI safety training dataset creation

**Background**
- While benchmarking datasets include tough corner cases, designed to make the AI model fail, there is always a need for separate training datasets that include both good and bad responses annotated with metadata for each request and response. This helps improve the accuracy of the AI model being trained. Benchmark datasets are small in size, while training datasets are large. Hence crowdsourced constructs are needed to create good training datasets. 

**Gaps**
- Chatbot Arena is a portal where users ask questions and get responses from two side by side compared AI models without revealing their names. While user preferences here help in evaluating the models, the questions they ask and responses given by the AI model are turned into an anonymized dataset that can be used for training purposes by other AI models. Humane Intelligence crowdsources AI safety data through incentivization structures such as bug bounties run in the US and Europe. ILINA is a fellowship program in Africa around AI safety. In the Indian context Bhashadaan is a portal for crowdsourcing language data, not AI safety data. Karya is like a Mechanical Turk for annotating data and requires a paid assignment to initiate any dataset creation. The following gaps exist for crowdsourcing an Indian AI safety dataset - No freely accessible crowdsourced constructs in India for AI safety
- No incentive structures figured out for crowdsourced data collection for AI safety in India
- No collation of crowdsourced data into AI safety datasets for India

**Potential research questions**
- Platform and Process Design: How can a freely accessible crowdsourcing platform be designed for AI safety data collection in India that overcomes current limitations (e.g. in Bhashadaan and Karya)?
- Dataset creation: What novel process architectures can be developed to integrate crowdsourced AI safety data into large-scale training datasets, ensuring high-quality annotations and metadata?
- Incentivization Structures and Engagement: What incentivization structures are most effective for motivating diverse contributors in India to participate in AI safety data collection, and how do these compare to models like bug bounties used in the US/Europe or fellowship programs in Africa? Explore cultural and economic factors affecting participation. 
- Incentivization Structures: How can gamification or alternative reward mechanisms be implemented to enhance both the quantity and quality of crowdsourced data for AI safety training?
- Incentivization Structures: How to ethically compensate contributors from informal economies?
- Quality Assurance and Annotation Standards: What methodologies (e.g. cross validation, consensus mechanisms, risk-reputation constructs) can be developed to ensure the reliability and validity of crowdsourced annotations for AI safety, especially in a multilingual and culturally diverse context like India? 
- Quality Assurance and Annotation Standards: How can metadata standards be designed to effectively capture the nuances of both good and bad responses in AI safety training datasets?
- Leveraging Existing AI Safety Initiatives: How can insights and data from existing platforms such as Chatbot Arena and Humane Intelligence be leveraged to develop a unified crowdsourced dataset that addresses the unique AI safety risks in India (applicability, interoperability)?
- Leveraging Existing AI Safety Initiatives: What strategies can be implemented to collate and harmonize crowdsourced AI safety data across disparate papers and platforms to form a comprehensive, India-centric training dataset?

