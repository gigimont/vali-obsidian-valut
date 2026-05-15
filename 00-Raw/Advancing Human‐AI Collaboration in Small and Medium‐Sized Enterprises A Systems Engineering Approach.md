---
title: "Advancing Human‐AI Collaboration in Small and Medium‐Sized Enterprises: A Systems Engineering Approach"
source: "https://incose.onlinelibrary.wiley.com/doi/10.1002/sys.70031"
author:
  - "[[Luis Flavio Ortolano]]"
  - "[[Erika E. Gallegos]]"
published:
created: 2026-05-15
description: "The integration of Artificial Intelligence (AI) into organizational processes presents unique challenges for Small and Medium-sized Enterprises (SMEs), particularly in fostering effective human-AI c..."
tags:
  - "clippings"
---
[PDF](https://incose.onlinelibrary.wiley.com/doi/epdf/10.1002/sys.70031 "ePDF")

## ABSTRACT

The integration of Artificial Intelligence (AI) into organizational processes presents unique challenges for Small and Medium-sized Enterprises (SMEs), particularly in fostering effective human-AI collaboration. Unlike large corporations with extensive resources for AI adoption, SMEs require adaptable frameworks tailored to their specific constraints and operational needs. This paper introduces the novel Human-AI Collaboration Maturity Model (HAIC-MM), which is a systems engineering framework designed to assess, guide, and enhance AI integration within SMEs. Developed through the synthesis of AI maturity models, digital transformation frameworks, and human-machine teaming research, HAIC-MM identifies seven dimensions and 32 capabilities across five maturity levels that are essential for successful AI adoption in SME contexts. Empirical validation through survey analysis (*N* = 100) confirmed the model's robustness. Subsequent focus group analyses (*N* = 10, repeated across five sessions) further validated HAIC-MM's practical utility and alignment with the operational realities of SMEs, emphasizing its relevance to everyday challenges faced by these organizations. Pilot testing with industry practitioners (*N* = 3) confirmed the usability and usefulness of the final HAIC-MM tool. HAIC-MM provides SME leaders with a structured, human-centered, and systematic approach to evaluate and cultivate human-AI collaboration, addressing key areas such as resource optimization, workforce empowerment, ethical AI oversight, and adaptive organizational culture. This research contributes to AI-enabled systems engineering by offering a practical framework for harmonizing human and AI capabilities within resource-constrained environments, ultimately supporting SMEs in achieving sustainable and ethically grounded AI integration across the organization.

### Summary

This paper introduces the Human-AI Collaboration Maturity Model (HAIC-MM), a framework designed to address the unique AI adoption challenges faced by Small and Medium-sized Enterprises (SMEs). The model identifies critical dimensions and capabilities needed to foster effective collaboration between humans and AI systems. The model also defines five maturity levels within each capability, allowing a granular assessment within the holistic framework. HAIC-MM provides a practical, step-by-step guide to assess and enhance AI integration for SMEs. The model emphasizes ethical AI oversight, workforce empowerment, and adaptive organizational culture, while addressing key challenges like resource constraints. HAIC-MM represents a significant contribution to the fields of systems engineering and organizational behavior, offering researchers investigating socio-technical systems, AI integration processes, and SME innovation strategies a rigorous framework for both theoretical advancement and practical implementation. With its focus on real-world application, HAIC-MM equips practitioners with actionable insights to build trust, optimize collaboration between human and AI capabilities, and achieve sustainable, ethically sound AI adoption, ensuring their organizations remain competitive in an increasingly digital economy.

## 1 Introduction

In today's rapidly evolving digital landscape, artificial intelligence (AI) has become essential for driving efficiencies and elevating productivity across industries. For small and medium-sized enterprises (SMEs), AI has shifted from being an emerging trend to a crucial tool for maintaining a competitive edge \[[1](#sys70031-bib-0001)\]. SMEs are vital to global employment and economic growth. For instance, 33.2 million small businesses in the U.S. alone account for 99% of all businesses and nearly half of the private workforce \[[2](#sys70031-bib-0002)\]. However, many SMEs struggle to adopt AI due to limited resources, a lack of technical expertise, and inconsistent strategic planning \[[3](#sys70031-bib-0003), [4](#sys70031-bib-0004)\]. Successfully addressing these challenges requires more than just adopting AI tools; it demands collaboration between AI and human capabilities. This paper introduces and validates the HAIC-MM, a systems engineering framework developed to prepare for effective AI integration.

SMEs, often defined by their employee count (e.g., under 500 in the United States, or fewer than 250 in the European Union), are essential to economies worldwide, yet they operate in fundamentally different circumstances than large corporations. To elaborate, SMEs typically encounter a specific combination of operational and financial limitations that significantly influence their approach to adopting technology, particularly artificial intelligence (AI). These limitations commonly present themselves as tighter budgetary constraints, restricting their capacity to invest in cutting-edge technologies and specialized AI personnel \[[3](#sys70031-bib-0003)\]. Furthermore, SMEs frequently experience reduced access to specialized technical expertise, encompassing both internal staff and external consultants, which complicates navigating the intricacies of AI implementation.

Adding to these technical challenges, less formalized operational procedures within SMEs can pose difficulties in seamlessly integrating AI into existing workflows, which often lack the structured data and standardization required for smooth AI adoption. Finally, given that individuals within SMEs often fulfill multiple roles and responsibilities, there may be less dedicated time and resources available for focused AI projects and change management initiatives \[[3](#sys70031-bib-0003)\]. These combined factors underscore the necessity for AI integration strategies specifically tailored to the SME context. Such strategies should prioritize practicality, adaptability, ease of use, and a clear path of AI adoption, even with limited resources.

Human-AI collaboration helps SMEs overcome adoption barriers by blending AI's analytical power with human intuition and judgment, complementing each other's limitations. Rather than replacing human roles, AI complements human capabilities, compensating for each other's limitations. This dynamic is particularly valuable for resource-constrained environments, where the combination of AI-driven automation and human flexibility maximizes productivity \[[1](#sys70031-bib-0001), [5](#sys70031-bib-0005)\]. Studies indicate that organizations employing human-AI collaboration can achieve up to 40% productivity gains, underscoring AI's value as a partner in enhancing human capabilities rather than replacing them \[[6](#sys70031-bib-0006)\].

Despite these benefits, high costs and limited AI expertise hinder many SMEs from adopting AI \[[5](#sys70031-bib-0005)\]. This highlights the need for a practical framework tailored to their specific challenges \[[3](#sys70031-bib-0003)\]. The Human-AI Collaboration Maturity Model (HAIC-MM) introduced in this paper offers a structured framework that enables SMEs to assess and enhance their AI-human collaboration maturity. Drawing upon systems engineering principles and leveraging Becker et al.’s methodology for maturity models \[[6](#sys70031-bib-0006)\], the HAIC-MM focuses on ethical and collaborative AI integration tailored to the needs and limitations of SMEs \[[2](#sys70031-bib-0002)\]. Core dimensions include AI literacy among leadership, ethical governance, and building trust, all aimed at guiding SMEs towards responsible AI adoption \[[5](#sys70031-bib-0005)\]. This model's validity is reinforced through insights from both quantitative surveys and qualitative focus groups, ensuring its practical relevance for SME stakeholders.

This research contributes to the broader AI and systems engineering discussions, proposing practical methods for SMEs to integrate AI effectively. Furthermore, HAIC-MM addresses critical areas in systems engineering, adding to the dialogue on the responsible integration of AI in complex business settings by focusing on three fundamental research questions:
1. How can a maturity model be specifically designed to address the unique operational constraints, resource limitations, and collaboration needs of Small and Medium-sized Enterprises (SMEs) aiming to effectively integrate Artificial Intelligence?
2. What core capabilities should SMEs emphasize to foster balanced and effective human-AI collaboration within practical resource limitations?
3. What key performance indicators can SMEs use to measure and guide the internal advancement of human-AI collaboration, ensuring continued alignment with their operational goals?

## 2 Literature Review

An extensive review of existing and relevant models was conducted. Through this, we identified 10 established models of AI maturity, 10 of digital transformation (DT), and 10 of human-machine teaming (HMT) to assess in great depth for their applicability to small and medium-sized enterprises (SMEs). Existing models often fail to align practically with the unique operational constraints of SMEs, especially when it comes to fostering collaborative, human-centered AI applications. An in-depth comparative analysis of these 30 models was conducted against maturity model standards \[[7](#sys70031-bib-0007)\], systems engineering principles and standards \[[8](#sys70031-bib-0008)\], Human-Computer Interaction (HCI) principles \[[9](#sys70031-bib-0009)\], and MITRE's HMT guidelines \[[10](#sys70031-bib-0010)\], allowing us to identify gaps and inform the development of our HAIC-MM model. Our analysis revealed that while existing models cover important domains, their applicability diminishes when considering the specific resource limitations and operational agility required within typical SME environments.

### 2.1 AI Maturity Models

To ensure a comprehensive yet focused literature review, we adopted a strategy of examining 10 prominent models within each of the three relevant domains: AI maturity, digital transformation (DT), and human-machine teaming (HMT). This number was determined based on the principle of thematic saturation, a recognized approach in literature reviews and maturity model development by Becker et al. \[[6](#sys70031-bib-0006)\] Following this principle, we iteratively reviewed frameworks within each category until we observed diminishing returns in the novelty of insights gained regarding the key dimensions, capabilities, and theoretical underpinnings relevant to the development of our Human-AI Collaboration Maturity Model (HAIC-MM). At this point, subsequent frameworks largely reiterated concepts and approaches already identified, indicating that thematic saturation had been reached and allowing us to proceed with a robust and representative set of source models for synthesis.

AI maturity models serve as structured frameworks for evaluating an organization's readiness to adopt AI, guiding the planning, implementation, and scaling of AI initiatives across various business functions. Among the 10 models reviewed, notable examples included IBM's AI Ladder, which prioritized ethics and trust \[[11](#sys70031-bib-0011)\], and Microsoft's AI Maturity Model, which facilitated AI integration with a focus on business-technology alignment, making it accessible to many SMEs \[[12](#sys70031-bib-0012)\]. Models like StatWorkx offered simplicity, ideal for SMEs seeking to adopt AI without high technical barriers \[[13](#sys70031-bib-0013)\], while Gartner's AI Maturity Model emphasized growth-oriented strategies for scalable AI implementation \[[14](#sys70031-bib-0014)\]. These models tend to focus on technical readiness, data governance, and automation, often overlooking the importance of collaborative human-AI interactions, employee upskilling, and fostering staff trust in AI outputs, all of which are crucial for effective AI adoption in SMEs.

### 2.2 Digital Transformation Maturity Models

Digital transformation maturity models help organizations align their technology initiatives with overall strategy and organizational culture, focusing on the digitization of operations, modernization of point-of-sale systems, and adoption of cloud solutions. From the 10 DT models analyzed, PwC's Digital Enterprise Framework emphasized agile digital models \[[15](#sys70031-bib-0015)\], Deloitte's Digital Maturity Model focused on infrastructure and data management as key enablers for transformation \[[16](#sys70031-bib-0016)\], and McKinsey's Digital Transformation Model prioritized customer experience and data-driven decision-making \[[17](#sys70031-bib-0017)\]. Each framework addressed essential DT domain areas; however, they primarily concentrated on technology infrastructure, innovation, and agility, often overlooking the unique constraints and resource limitations faced by SMEs during digital transformation \[[18](#sys70031-bib-0018)\].

### 2.3 Human-Machine Teaming Frameworks

HMT frameworks aim to foster teamwork and adaptability between humans and AI, emphasizing trust-building, communication, and the integration of human skills with AI. Of the 10 HMT models reviewed, including the collaborative intelligence framework \[[19](#sys70031-bib-0019)\] and collaborative maturity framework (CMF) \[[20](#sys70031-bib-0020)\], key elements emerged like trust, common ground, and observability, supporting cohesive team dynamics. Models like team situation awareness for control (TSAC) and human-autonomy teaming (HAT) improved situational awareness and adaptability in AI-integrated environments \[[20](#sys70031-bib-0020)\]. While these provided guidance on team dynamics and decision-making, they lacked structured, maturity assessments tailored to SMEs, underscoring the need for a model that integrates HMT principles with SMEs' operational constraints.

### 2.4 Gaps in Existing Literature

While the reviewed AI maturity, digital transformation, and HMT frameworks offer valuable insights, they often presuppose organizational structures, resources, and data capabilities more typical of large enterprises. Key challenges for SMEs, such as severe resource constraints (financial and human), less formal governance structures, the need for employees to assume diverse and cross-functional roles (limiting specialization), and a heightened sensitivity to implementation costs and disruptions, are frequently under-addressed. For instance, complex data infrastructure requirements or extensive change management processes outlined in some models may be prohibitive for SMEs. This necessitates a framework like HAIC-MM, designed with SME realities in mind, emphasizing scalability, accessibility, and clear guidance on achieving human-AI synergy within typical operational constraints.

## 3 Theoretical Framework

HAIC-MM integrates three theoretical domains to address the complexity of human-AI collaboration \[[21](#sys70031-bib-0021)\] in SMEs: (1) systems engineering principles; (2) human-computer interaction theory; and (3) organizational behavior theory.

### 3.1 Systems Engineering Principles

Guided by industry standards in systems engineering (SE), including the ISO/IEC/IEEE 15288 framework and principles supported by INCOSE (International Council on Systems Engineering) \[[22](#sys70031-bib-0022)\], HAIC-MM leverages the following approaches for human-AI collaboration:
- *Systems Thinking*: Views AI integration as a socio-technical system with emergent properties affecting both technical and human elements.
- *Lifecycle Management*: Guides iterative systems development from initial assessment through continuous improvement.
- *Requirements Engineering*: Ensures AI capabilities align with SME constraints and needs.

### 3.2 Human-Computer Interaction Theory

Human-Computer Interaction (HCI) principles provide essential guidelines for designing AI systems that prioritize usability, accessibility, and effectiveness \[[9](#sys70031-bib-0009)\]. Rooted in extensive research on user-centered design, HCI provides essential guidelines that ensure AI systems are intuitive, approachable, and aligned with the needs and cognitive patterns of end-users. HCI principles guide the design of AI systems in the following key areas:
- *User Understanding*: Ensures AI systems operate in ways that users can comprehend and predict, promoting confident interaction.
- *Ease of Use*: Focuses on creating simple, intuitive interfaces that reduce complexity and make AI tools accessible to all employees.
- *Trust Building*: Develops user confidence through clear communication of AI capabilities and limitations.

### 3.3 Organizational Behavior Theory

### 3.4 Synergy of Theories: A Unified Approach

Figure [1](#sys70031-fig-0001) illustrates the integration of theoretical foundations that form the backbone of the HAIC-MM framework. The synergy of systems engineering, human-computer interaction, and organizational behavior theories is visualized, highlighting how each domain contributes uniquely to the framework:
- SE provides structured methodology and lifecycle management, essential for a systematic approach to AI integration.
- HCI principles ensure AI solutions are usable, understandable, and trust-building, facilitating effective human-AI collaboration.
- Organizational behavior emphasizes change readiness, cultural adaptation, and sustained AI adoption within SME contexts.

![Details are in the caption following the image](https://incose.onlinelibrary.wiley.com/cms/asset/0c236dc9-65a9-49a4-888b-08073e0ef4c9/sys70031-fig-0001-m.jpg)

FIGURE 1 Open in figure viewer PowerPoint Synergy of theoretical foundations in HAIC-MM.

The central overlap in the diagram represents the unified approach HAIC-MM offers, balancing technical rigor with human-centered design and organizational adaptability to meet SMEs' unique constraints. This unified perspective is crucial for fostering sustainable and balanced human-AI collaboration in resource-constrained settings.

## 4 Development Methodology

Our research methodology for developing the HAIC-MM follows a structured, iterative framework, combining Becker et al.’s maturity model development \[[6](#sys70031-bib-0006)\] with Hevner et al.’s design science research principles \[[27](#sys70031-bib-0027)\]. This hybrid approach was selected after evaluating seven prominent procedural models for maturity model development, focusing on validation rigor, multidisciplinary inputs, adaptability, and accessibility for SMEs.

The systematic development process, illustrated in Figure [2](#sys70031-fig-0002), unfolds across six distinct stages, each incorporating feedback loops to ensure continuous refinement and alignment with SME requirements. These stages guide both the theoretical development and practical application of the HAIC-MM:
1. *Problem Identification*: Identified SME-specific challenges in AI adoption, staff skill gaps, and resource limitations, which were accomplished through the literature review.
2. *Analysis*: Conducted a comprehensive review of 30 frameworks (10 AI, 10 DT, 10 HMT). This was also completed during the literature review phase, and highlights the strengths and limitations of current models, particularly their gaps in addressing SME-specific needs in human-AI collaboration.
3. *Determine Development Approach*: Based on our analysis, we adopted a synthesis approach to develop HAIC-MM. This method integrated elements from AI, DT, and HMT models, grounded in the core principles of systems engineering, human-computer interaction, and organizational behavior. By integrating these diverse frameworks with a focus on these underlying theories, we created a model that balances technical, organizational, and human-centered dimensions.
4. *Iterative Design and Development*: This phase moved systematically from initial models to the structured HAIC-MM framework, detailed in the next section. We began with metamodels to decompose 30 AI, DT, and HMT models, isolating key components. These informed pivot models, which synthesized and organized core constructs into comprehensive supersets.
5. *Validation*: Employed a mixed-methods approach, incorporating both surveys and focus groups to gather diverse perspectives and validate the framework's relevance and applicability.
6. *Refinement*: Enhanced the model through iterative adjustments based on empirical feedback, resulting in a theoretically release-ready version tailored for practical application in SMEs.

![Details are in the caption following the image](https://incose.onlinelibrary.wiley.com/cms/asset/86181847-92b8-48f1-898a-b564490441be/sys70031-fig-0002-m.jpg)

FIGURE 2 Open in figure viewer PowerPoint HAIC-MM development lifecycle.

These stages guide both the theoretical development and practical implementation of the HAIC-MM.

## 5 Preliminary Model Development

Our model was developed using an iterative approach. We first reviewed existing literature and synthesized these findings to develop our preliminary model (Section 5 of this paper). Then, we validated the model components using a survey study (Section 6). Finally, we refined the model's descriptions and components based on feedback from multiple focus group sessions with industry experts (Section 7), resulting in our finalized HAIC-MM (Section 8).

### 5.1 Development Process Overview

We began by executing a detailed synthesis process to construct the HAIC-MM, as illustrated in Figure [3](#sys70031-fig-0003). This involved analyzing 30 key models relating to AI, DT, and HMT. We employed metamodels and pivot models as techniques to systematically decompose, select, and integrate relevant elements from these existing frameworks. As recommended by Becker et al. \[[6](#sys70031-bib-0006)\], this synthesis technique is the ideal approach when working with a broad range of maturity models in similar or related domains.
- *Metamodels*: These were used to systematically isolate key components and recurring themes from the 30 models. In doing so, we gained important insights into strategic, technical, and collaborative elements crucial for SMEs.
- *Pivot Models*: Created as comprehensive supersets, pivot models organized and synthesized the isolated components from the metamodels. By cross-referencing elements across AI, DT, and HMT models, pivot models helped us identify the most relevant components to build an adaptable framework tailored to SMEs.

![Details are in the caption following the image](https://incose.onlinelibrary.wiley.com/cms/asset/6cd55bfd-db8d-4d98-b6d2-2c336af78a91/sys70031-fig-0003-m.jpg)

FIGURE 3 Open in figure viewer PowerPoint HAIC-MM development process flow diagram.

These techniques enabled us to develop a model structure specifically designed to address the unique demands of SMEs, integrating technical, organizational, and human-centered elements in a balanced way. The resulting product was the draft structure of our HAIC-MM for testing.

### 5.2 Selection of Source Models

We examined 30 existing models and frameworks across three distinct categories: AI and DT models, and HMT frameworks. The selection process prioritized models with strong empirical validation, industry recognition, and demonstrated relevance to SME environments. Table [^1] lists the 10 core AI frameworks evaluated, with their strengths relevant to SMEs.

| Model | Industry focus | Implementation complexity | SME relevance | Key strengths |
| --- | --- | --- | --- | --- |
| IBM AI Digital | General | Medium | High | Strong ethics & trust focus |
| Microsoft AI | Tech | Low | High | Business-tech alignment |
| ElementAI | Tech | Medium | Medium | Human-centric approach |
| StatWorkx | General | Low | High | Simple, actionable |
| Gartner AI | General | Low | Medium | Growth-oriented strategy |
| OVUM AI | Tech | High | Low | Sharp operational focus |
| Alsheibani AIMM | General | Medium | Medium | Innovation emphasis |
| AppliedAI | General | Medium | High | Operational excellence |
| Accenture AI | General | Medium | Medium | Holistic analysis |
| AIMI | General | High | Medium | Innovation management |

Similarly, Table [^2] details the 10 models evaluated relating to digital transformation, providing a summary of their scope, cost, and focus areas for SMEs.

| Model | Industry focus | Maturity levels | Implementation cost | Capability coverage | Primary focus |
| --- | --- | --- | --- | --- | --- |
| PWC digital | General | 4 | High | High | Value chain digitization |
| IMPULS | Manuf. | 6 | Medium | High | Smart operations |
| VTT digital | General | 5 | Low | High | Strategy integration |
| Capgemini | General | 4 | High | High | Customer experience |
| BCG digital | General | 4 | High | High | Leadership commitment |
| Forrester | Tech | 4 | Medium | High | Cultural transformation |
| McKinsey | General | 3 | High | Medium | Strategic alignment |
| Deloitte | General | 5 | High | High | Customer-centricity |
| Acatech | Manuf. | 5 | Medium | Medium | Smart solutions |
| KPMG digital | General | 5 | High | High | Digital readiness |

Lastly, the 10 human-machine teaming models evaluated for HAIC-MM are summarized in Table [^3].

| Model | Collab. focus | Technical depth | Implement. guidance | Key HMT principles | Primary application |
| --- | --- | --- | --- | --- | --- |
| CIQ | High | Medium | Medium | Common ground, observability | Team dynamics |
| CMF | High | Medium | High | Trust, directability | Process optimization |
| TSAC | Medium | High | Medium | Adaptability, trust | Situational awareness |
| HAT | High | High | Medium | Observability, directability | Autonomy integration |
| HMHR | Medium | High | Low | Direction, adaptability | Robot collaboration |
| FAHMT | High | Medium | High | Adaptability, solutions | Adaptive teaming |
| TST | Medium | High | Medium | Common ground, trust | Synthetic teammates |
| MUHMT | High | Medium | High | Trust, information | Mutual understanding |
| MAHMT | High | High | High | Adaptability, solutions | Model-based HMT |
| R-HMT | High | High | High | Common ground, trust | Resilient teaming |

### 5.3 Model Decomposition and Integration

To develop the HAIC-MM, we identified key components from the 30 source models necessary for integration into our model. The recurring themes and overlapping elements provided insight into strategic, technical, and collaborative components required for our model. Specifically, from the AI models we identified the following dimensions: strategy, infrastructure, process, and skills. From the DT models, we identified: digital strategy, technology, operations, and culture. Lastly, from the HMT models, we identified the following important principles: common ground, observability, directability, and adaptability.

### 5.4 Preliminary Model Structure

The results of integrating the deconstructed elements and identified gaps from the 30 AI, DT, and HMT models yielded a preliminary version of HAIC-MM. At this point, the HAIC-MM seven distinct *dimensions*, each targeting essential aspects of human-AI collaboration: (1) Collaborative Strategy and Leadership; (2) Empowerment and Adaptive Culture; (3) Integrated Technology and User Experience; (4) Process Harmonization; (5) Human-Centric Customer Engagement; (6) Data Ethics and Human Oversight; and (7) Inclusive Governance and Continuous Learning. Within each dimension, four core *capabilities* were defined to provide further granularity and enable focused assessment in each area. For example, Collaborative Strategy and Leadership can be evaluated through its capabilities: (1) AI-Enhanced Decision Making; (2) Leadership AI Literacy; (3) Collaborative Vision Communication; and (4) AI Integration in Business Plans.

Each capability is intended to be assessed on a 5-point maturity scale, where maturity levels reflect increasing proficiency and sophistication in human-AI collaboration. For example, a capability's *maturity* may progress as follows: (1) Initial; (2) Developing; (3) Cooperative; (4) Advanced; and (5) Symbiotic. After refining and validating the HAIC-MM, the finalized HAIC-MM tool will provide detailed assessment criteria and evaluation metrics to enable organizations to accurately score their maturity levels across each capability. It is important to clarify that, for the purposes of this research and validation, the maturity levels themselves served as a descriptive framework for assessing the progression of human-AI collaboration capabilities. The numerical scores presented in the validation sections (Sections 6 and 7) relate to participant agreement and sentiment towards the dimensions, capabilities, and maturity level descriptions, and not to a calculated ‘maturity level score’ for any specific SME. The development of a quantitative scoring mechanism for SMEs using HAIC-MM to determine their specific maturity level is planned for future work, during the development of the assessment tool, and pilot tests, as mentioned in Section 8.

## 6 Validation of Dimensions and Capabilities

A quantitative analysis via an online survey was conducted to validate the dimensions (7) and capabilities (28) of the proposed HAIC-MM framework. This survey targeted industry experts, subject matter specialists, and AI practitioners to assess the model's applicability, relevance, and construct validity within professional settings.

### 6.1 Methodology

A total of 100 participants (50 males, 50 females) completed the survey. Participants represented diverse organizational roles: middle management (*N* = 29), senior management (*N* = 9), director (*N* = 51), and c-level executive (*N* = 11). There was also a wide range of age groups represented: 25–34 years old (N = 22), 35–44 y.o. (*N* = 43), 45–54 y.o. (*N* = 21), and 55+ y.o. (*N* = 14). They were recruited through a paid panel via PollFish, targeting working professionals in the United States who met the following inclusion criteria: (1) at least 18 years old; (2) completed at least a bachelor's degree; (3) currently employed at a company with 100–500 employees; and (4) at least some involvement with AI adoption, usage, or planning within their organization.

The survey took on average 14.5 min to complete. The survey included demographic questions and 47 questions related to their perceptions of AI within their organization. Specifically, there were 14 questions used to assess our HAIC-MM dimensions (2 questions per dimension) and 27 questions to assess our HAIC-MM capabilities (1 question per capability).

The questions were asked using a 6-point Likert scale, with higher scores indicating stronger agreement or perceived importance. Participants were asked questions related to each dimension and capability without being presented with the HAIC-MM directly. For example, to assess the “Collaborative Strategy and Leadership” dimension, participants responded to statements about the importance of integrating AI into strategic planning and leaders being knowledgeable about AI tools.

### 6.2 Results

#### 6.2.1 Participant Experience With AI Within Organizations

Participants reported varying levels of involvement with AI in their organizations. The majority (65%) reported “direct involvement in strategic planning and decision-making for technology, including AI.” There were 17% that reported that they “contribute to the evaluation and selection of technology and AI-based solutions.” And 9% each to the categories of “participate in discussions or provide input on adopting new technologies or AI-based solutions” and “regularly use technology or AI-based solutions as part of job functions.”

#### 6.2.2 Validation of HAIC-MM Dimensions

Participants were asked about their perceptions of each dimension relative to successful integration of human-AI teaming within the workplace. Each dimension was assessed across two questions. Depending on the wording of the question, participants were asked on a 6-point Likert scale to assess the importance, significance, agreement, criticality, essentialness, beneficial, or vitalness of the statement. Results indicate that across all seven dimensions, mean scores were above 4.3 out of 6, displaying support for inclusion in the HAIC-MM (see Table [^4]).

<table><thead><tr><th rowspan="2">HAIC-MM dimension</th><th colspan="2">Question 1</th><th colspan="2">Question 2</th></tr><tr><th><i>Mean</i></th><th><i>Scale</i></th><th><i>Mean</i></th><th><i>Scale</i></th></tr></thead><tbody><tr><td>Collaborative strategy leadership</td><td>5.2</td><td>Importance</td><td>5.0</td><td>Agreement</td></tr><tr><td>Empowerment and adaptive culture</td><td>4.4</td><td>Importance</td><td>4.2</td><td>Criticality</td></tr><tr><td>Integrated tech. and user experience</td><td>4.8</td><td>Importance</td><td>4.7</td><td>Essential</td></tr><tr><td>Process harmonization</td><td>4.8</td><td>Importance</td><td>4.8</td><td>Beneficial</td></tr><tr><td>Human-centric customer engagement</td><td>4.3</td><td>Significance</td><td>4.5</td><td>Essentialness</td></tr><tr><td>Data ethics and human oversight</td><td>4.8</td><td>Importance</td><td>4.5</td><td>Vitalness</td></tr><tr><td>Inclusive goals and continuous learning</td><td>4.6</td><td>Importance</td><td>4.6</td><td>Significance</td></tr></tbody></table>

#### 6.2.3 Validation of HAIC-MM Capabilities

Similarly, 6-point Likert scale questions were used to assess each capability. Given the relatively large number of capabilities, only one question per capability was asked. Each question described the capability, and asked participants about their perceived significance of the statement on integrating humans with AI effectively. Figure [4](#sys70031-fig-0004) presents these mean scores for each capability within its respective dimensions. This visualization demonstrates a consistently high level of significance assigned to individual capabilities across dimensions, reflecting positive evaluations of the framework's approach to measuring effective human-AI collaboration.

![](https://incose.onlinelibrary.wiley.com/cms/asset/a1b6b900-e951-4429-993f-e2948b8fbc9a/sys70031-fig-0004-m.jpg)

FIGURE 4 Open in figure viewer PowerPoint Mean scores (out of 6) for capabilities by dimension.

### 6.3 Summary

While the survey results indicated consistently high perceived importance across most capabilities rather than sharp differentiation (Figure [4](#sys70031-fig-0004)), this quantitative analysis (*N* = 100) served a crucial purpose: it provided broad validation that the fundamental dimensions and capabilities identified for the HAIC-MM resonated as relevant and comprehensive with industry professionals involved in AI adoption. This confirmation provided a solid foundation for the subsequent, more in-depth qualitative refinement through focus groups, where nuances and specific contextual factors could be explored in greater detail.

## 7 Refinement of Dimensions and Capabilities

There were five focus group sessions conducted to further validate and refine the HAIC-MM. The first set (Sessions 1 and 2) focused on reviewing the model's dimensions, capabilities, and maturity levels to establish their necessity and comprehensiveness. The second set (Sessions 3, 4, and 5) concentrated on refining the “current state” descriptions for each capability across the five maturity levels, ensuring they accurately reflect small and medium-sized enterprises (SMEs) realities. These current state descriptions provide the context within each capability and maturity level cross-section for an SME to identify how they score for each capability.

### 7.1 Methodology

A total of 10 participants from various leadership roles and industry backgrounds participated in the focus groups. The job positions of each participant are as follows: Director of IT Operations; VP of Engineering; Director of Process Improvement; VP of Human Resources; VP of Claims Management; Director of Customer Service; Marketing Manager; Digital Product Manager; Finance Director; and VP of Sales.

All participants attended both Sessions 1 and 2. In these sessions, participants reviewed the HAIC-MM dimensions, capabilities, and maturity levels. Each session took approximately 90 min. Discussions in these focus groups were guided by two primary questions: (1) Is there a clear and defined need for a Human-AI Collaboration Maturity Model, and (2) Do the proposed capabilities in the HAIC-MM comprehensively assess the ways in which humans and AI collaborate.

Participants were then divided into smaller groups for the subsequent set of focus group sessions, where each participant only participated in one session. In Session 3 (*N* = 3), Session 4 (*N* = 4), and Session 5 (*N* = 3), participants reviewed the current state descriptions for each capability within each of the five maturity levels. To allow for deeper discussion, each session only evaluated a subset of the current state descriptions. Specifically, Session 3 evaluated the first 11 capabilities, Session 4 evaluated the next 11 capabilities, and Session 5 evaluated the last 10 capabilities. Since each capability had a current state description across all five maturity levels, each session reviewed 55, 55, and 50 current state descriptions, respectively. Discussion in these focus groups was guided by three key questions: (1) Do the current state descriptions accurately reflect SME realities? (2) Are the descriptions realistic and relevant for SMEs? and (3) Do they demonstrate a logical progression across maturity levels?

The audio of participant discussions was recorded for all five sessions. A sentiment analysis of these audio transcripts is provided to demonstrate their positive, neutral, and/or negative assessments towards the HAIC-MM components. A sentiment score was calculated using Equation ([^5]), which could range from −1 (entirely negative) to +1 (entirely positive).

(1)

Sentiment analysis was conducted through manual coding of the focus group transcriptions. Each comment was reviewed and classified as positive, neutral, or negative based on the expressed sentiment towards the HAIC-MM dimensions, capabilities, or maturity levels. Positive comments indicated agreement, support, or positive evaluation of the model components. Negative comments expressed disagreement, criticism, or identified weaknesses. Comments that were factual, clarifying, or did not express a clear positive or negative evaluation were classified as neutral. Discrepancies in coding between the two researchers were resolved through discussion to ensure consistency and agreement on the final sentiment classification for each comment.

### 7.2 Results

#### 7.2.1 Focus Group Sessions 1 and 2

The initial two focus group sessions were conducted to gather essential feedback on the HAIC-MM's purpose and to refine the value and scope of its capabilities, laying a foundation for aligning the model with real-world human-AI collaboration needs.

A sentiment analysis was performed across all the comments that each participant said throughout Sessions 1 and 2, see Table [^6]. This revealed varying feedback across roles. Marketing (0.78) and Engineering (0.77) recorded the highest scores, showing strong model support in technical and customer-facing roles. The lowest score (0.00) from IT Operations, which was neutral, indicated a balanced, cautious view. The overall 0.54 sentiment score from the 185 comments reflected broad support for the HAIC-MM model, while highlighting the need for attention in technical and operational areas. This feedback distribution indicates that the model aligns with diverse stakeholder needs, yet requires targeted refinements.

| Participant | Positive | Neutral | Negative | Total | Sentiment score |
| --- | --- | --- | --- | --- | --- |
| Manager, Marketing | 15 | 2 | 1 | 18 | 0.78 |
| VP Engineering | 18 | 3 | 1 | 22 | 0.77 |
| VP Sales | 13 | 2 | 2 | 17 | 0.65 |
| Manager, Digital Products | 11 | 2 | 1 | 14 | 0.71 |
| Dir. Customer Service | 12 | 2 | 2 | 16 | 0.63 |
| VP Human Resources | 12 | 3 | 1 | 16 | 0.69 |
| Dir. Process Improvement | 14 | 4 | 2 | 20 | 0.60 |
| Dir. Finance | 8 | 5 | 1 | 14 | 0.50 |
| VP of Claims Management | 10 | 8 | 2 | 20 | 0.40 |
| Dir. IT Operations | 8 | 12 | 8 | 28 | 0.00 |
| Total | 121 | 43 | 21 | 185 | 0.54 |

The analysis in Table [^7] revealed considerable sentiment improvement across all HAIC-MM dimensions following the review and refinement of their purposes and descriptions. Initial sentiments were notably negative toward overall purposes, ranging from −0.5 (Harmonizing Processes) to −0.1 (Governance & Learning), indicating substantial initial concerns. Post-refinement, all dimensions achieved positive sentiments, with Ethics & Oversight and Customer Engagement showing the most dramatic improvements, reaching 0.9 from −0.3 and −0.2, respectively. The observed improvement in initial to final sentiment scores across all dimensions demonstrates the successful refinement of the model's dimension purposes and strong stakeholder alignment with their final concept.

<table><thead><tr><td></td><th colspan="3">Before</th><th colspan="3">After</th><td></td><td></td></tr><tr><th>Dimension</th><th>+</th><th>0</th><th>—</th><th>+</th><th>0</th><th>—</th><th>Initial Score</th><th>Final Score</th></tr></thead><tbody><tr><td>Harmonizing processes</td><td>1</td><td>3</td><td>6</td><td>6</td><td>3</td><td>1</td><td>−0.5</td><td>0.5</td></tr><tr><td>Empowerment & culture</td><td>1</td><td>4</td><td>5</td><td>6</td><td>3</td><td>1</td><td>−0.4</td><td>0.5</td></tr><tr><td>Ethics & oversight</td><td>2</td><td>3</td><td>5</td><td>9</td><td>1</td><td>0</td><td>−0.3</td><td>0.9</td></tr><tr><td>Human-centric integration</td><td>2</td><td>3</td><td>5</td><td>8</td><td>1</td><td>1</td><td>−0.3</td><td>0.7</td></tr><tr><td>AI-enhanced leadership</td><td>2</td><td>3</td><td>5</td><td>7</td><td>2</td><td>1</td><td>−0.3</td><td>0.6</td></tr><tr><td>Customer engagement</td><td>2</td><td>4</td><td>4</td><td>9</td><td>1</td><td>0</td><td>−0.2</td><td>0.9</td></tr><tr><td>Governance & learning</td><td>3</td><td>3</td><td>4</td><td>8</td><td>2</td><td>0</td><td>−0.1</td><td>0.8</td></tr></tbody></table>

A similar analysis for the capabilities is shown in Table [^8], which also revealed significant improvements post-refinement. Of the original 28 capabilities, conversations led to 24 of the capabilities getting revised. These revised capabilities showed substantial enhancement, moving from −0.5 initial sentiment to 0.6 final sentiment. The four unchanged capabilities maintained a consistent 80% sentiment throughout, validating their original design.

<table><thead><tr><td></td><td></td><th colspan="3">Before</th><th colspan="3">After</th><td></td><td></td></tr><tr><th>Category</th><th># of Capabilities</th><th>+</th><th>0</th><th>—</th><th>+</th><th>0</th><th>—</th><th>Initial Score</th><th>Final Score</th></tr></thead><tbody><tr><td>Revised capabilities</td><td>24</td><td>1</td><td>2</td><td>5</td><td>7</td><td>2</td><td>1</td><td>−0.50</td><td>0.60</td></tr><tr><td>Unchanged capabilities</td><td>4</td><td>8</td><td>2</td><td>0</td><td>8</td><td>2</td><td>0</td><td>0.80</td><td>0.80</td></tr><tr><td>New capabilities added</td><td>4</td><td>—</td><td>—</td><td>—</td><td>7</td><td>2</td><td>1</td><td>—</td><td>0.60</td></tr></tbody></table>

During the focus group sessions, four new capabilities were identified as missing aspects of human-AI collaboration and were added to strengthen the model: AI Adoption Readiness Assessment, Human Trust in AI Assessment, Data Quality Assurance for AI, and Equity and Fairness Assessment. These new additions achieved a 0.6 final sentiment, indicating successful integration into the model.

A similar analysis of HAIC-MM maturity levels is shown in Table [^9], also illustrating significant improvements following the refinement of level descriptions and titles against their relevance within human-AI collaboration. Four of the five levels showed substantial positive changes in sentiment, with initial negative scores improving to positive scores. The most dramatic improvement was seen in Level 4, which evolved from “Strategic” to “AI-Aligned.” Notably, Level 5 “Symbiotic” maintained its strong positive sentiment of 0.8 throughout, requiring no revision and validating its original conceptualization as the model's highest maturity level. These improvements demonstrate the effectiveness of the refinement process in creating more clearly defined and meaningful maturity levels.

| Level | Initial title | Initial score | Revised title | Revised score |
| --- | --- | --- | --- | --- |
| 1 | Exploratory | −0.20 | AI exploration | 0.50 |
| 2 | Developing | −0.30 | AI-enabled | 0.50 |
| 3 | Integrated | −0.20 | AI-embedded | 0.40 |
| 4 | Strategic | −0.20 | AI-aligned | 0.60 |
| 5 | Symbiotic | 0.80 | Symbiotic | 0.80 |

Last, the analysis of stakeholder responses to the two primary questions, Table [^10], revealed strong support for the HAIC-MM. Regarding the question relating to the need for the HAIC-MM, seven participants expressed positive support, with two neutral responses and one negative response, achieving a moderate consensus level. The second question regarding the comprehensiveness of HAIC-MM demonstrated even stronger support with eight positive responses, one neutral, and one negative position, reaching a high consensus level. The higher consensus on comprehensiveness suggests that while there is solid agreement on the need for the model, there is even stronger confirmation that the proposed model effectively captures the essential elements of human-AI collaboration. Only IT Operations maintained consistent concerns, while Finance remained neutral, indicating potential areas for technical and operational consideration in future refinements.

| Overall questions | Positive | Neutral | Negative | Total | Sentiment score |
| --- | --- | --- | --- | --- | --- |
| Need for HAIC-MM | 7 | 2 | 1 | 10 | 0.60 |
| HAIC-MM comprehensiveness | 8 | 1 | 1 | 10 | 0.70 |

In Summary, focus group Sessions 1 and 2 demonstrated substantial improvement in the HAIC-MM's structure and stakeholder acceptance. Initial sentiment analysis revealed strong support from technical and customer-facing roles, while highlighting concerns in IT Operations. All seven dimensions progressed from negative sentiments to achieve positive final sentiments, while capability refinement showed similar success and introduced four new capabilities. Maturity level refinement saw four of five levels improve significantly. The strong consensus on the model's need and comprehensiveness (7 and 8 positive responses) validates the model's foundation while identifying key areas for technical implementation refinement.

#### 7.2.2 Focus Group Sessions 3, 4, and 5

The final three focus group sessions concentrated on validating and refining the HAIC-MM current state descriptions to better align them with the specific needs of SMEs. The primary objectives of this qualitative analysis were to assess participants' level of agreement on the accuracy of the maturity state descriptions, evaluate their realism and progression, and ensure that the HAIC-MM's capabilities were applicable to real-world SME contexts.

Each participant was asked to complete a pre-session evaluation, in which they were provided the current state descriptions for each of the capability + maturity level combinations that their group was assessing. They were asked if they agreed or disagreed with the description. For example, the original current state description for “Capability 1: Augmented Decision Making—Level 3” stated:

> “Organization achieves 45% AI-supported decision-making across core operations. Standardized data processes and improved AI models deliver consistent insights. Cross-functional teams regularly leverage AI analysis, though advanced applications remain limited.”

Prior to each focus group session, we identified the descriptions that did not have consensus and focused discussion only on these descriptions. Hence, each of these sessions centered around resolving these disagreements about the descriptions. Disagreement was defined such that at least one participant disagreed with the current state description.

For example, during the focus group discussion on the previous current state description, participants highlighted that the 45% metric was arbitrary and difficult to measure, the assumption of standardized data processes was too ambitious for SMEs, and the description needed clearer criteria for AI-supported decisions. This feedback led to the following revised current state description that better reflected SME realities:

> “Organization achieves 30% AI-supported decision-making across core operations, with clear criteria defining AI-supported decisions. Basic data quality standards and governance processes enable reliable insights. Cross-functional teams pilot AI analysis in specific departments, with documented success cases driving wider adoption. Focus remains on building trust and ensuring data quality while gradually expanding AI applications.”

This revision process exemplifies how the focus groups helped refine the HAIC-MM to be more practical and achievable for SMEs. While a table visualizing the agreement across all 160 current state descriptions would be lengthy, Table [^11] summarizes this feedback at the dimension level. This table shows the number and percent of current state descriptions within each dimension that had complete agreement (all participants approved). The current state descriptions with disagreement were evaluated in the focus groups.

<table><thead><tr><th rowspan="2">Dimension</th><th rowspan="2">Number of capabilities</th><th colspan="5">Maturity level</th></tr><tr><th>1</th><th>2</th><th>3</th><th>4</th><th>5</th></tr></thead><tbody><tr><td>AI-enhanced leadership & strategy</td><td>5</td><td><p>4</p><p>(80%)</p></td><td><p>1</p><p>(20%)</p></td><td><p>3</p><p>(60%)</p></td><td><p>4</p><p>(80%)</p></td><td><p>5</p><p>(100%)</p></td></tr><tr><td>Adaptive AI culture & empowerment</td><td>4</td><td><p>4</p><p>(100%)</p></td><td><p>3</p><p>(75%)</p></td><td><p>0</p><p>(0%)</p></td><td><p>4</p><p>(100%)</p></td><td><p>4</p><p>(100%)</p></td></tr><tr><td>Human-centric AI integration</td><td>5</td><td><p>4</p><p>(80%)</p></td><td><p>2</p><p>(40%)</p></td><td><p>1</p><p>(20%)</p></td><td><p>3</p><p>(60%)</p></td><td><p>3</p><p>(60%)</p></td></tr><tr><td>Harmonizing AI & human processes</td><td>4</td><td><p>2</p><p>(50%)</p></td><td><p>1</p><p>(25%)</p></td><td><p>2</p><p>(50%)</p></td><td><p>3</p><p>(75%)</p></td><td><p>4</p><p>(100%)</p></td></tr><tr><td>Human-centered AI customer engagement</td><td>4</td><td><p>1</p><p>(25%)</p></td><td><p>0</p><p>(0%)</p></td><td><p>1</p><p>(25%)</p></td><td><p>1</p><p>(25%)</p></td><td><p>1</p><p>(25%)</p></td></tr><tr><td>AI ethics & human oversight</td><td>6</td><td><p>4</p><p>(67%)</p></td><td><p>0</p><p>(0%)</p></td><td><p>1</p><p>(17%)</p></td><td><p>5</p><p>(83%)</p></td><td><p>6</p><p>(100%)</p></td></tr><tr><td>Inclusive AI governance & learning</td><td>4</td><td><p>1</p><p>(25%)</p></td><td><p>0</p><p>(0%)</p></td><td><p>1</p><p>(25%)</p></td><td><p>4</p><p>(100%)</p></td><td><p>4</p><p>(100%)</p></td></tr></tbody></table>

Based on these current state descriptions that required revision, we performed the focus group Sessions 3, 4, and 5, focusing on evaluating and improving the descriptions based on three key criteria: accuracy, clarity, and achievability. The analysis of these sessions is summarized in Table [^12], revealing significant improvements after revisions. Specifically, sentiment scores improved from all negative towards the current state descriptions to all positive, achieving scores above 0.65 across all criteria.

<table><thead><tr><th rowspan="2">Focus group</th><th rowspan="2">Current state description</th><th colspan="3">Before</th><th colspan="3">After</th><th rowspan="2">Initial score</th><th rowspan="2">Final score</th></tr><tr><th>+</th><th>0</th><th>—</th><th>+</th><th>0</th><th>—</th></tr></thead><tbody><tr><td rowspan="3">Session 3</td><td>Accuracy</td><td>2</td><td>3</td><td>12</td><td>14</td><td>2</td><td>1</td><td>−0.59</td><td>0.76</td></tr><tr><td>Clarity</td><td>1</td><td>2</td><td>14</td><td>15</td><td>1</td><td>1</td><td>−0.76</td><td>0.82</td></tr><tr><td>Achievability</td><td>3</td><td>2</td><td>12</td><td>13</td><td>3</td><td>1</td><td>−0.53</td><td>0.71</td></tr><tr><td rowspan="3">Session 4</td><td>Accuracy</td><td>1</td><td>4</td><td>19</td><td>20</td><td>3</td><td>1</td><td>−0.75</td><td>0.79</td></tr><tr><td>Clarity</td><td>0</td><td>3</td><td>21</td><td>19</td><td>4</td><td>1</td><td>−0.88</td><td>0.75</td></tr><tr><td>Achievability</td><td>2</td><td>3</td><td>19</td><td>18</td><td>4</td><td>2</td><td>−0.71</td><td>0.67</td></tr><tr><td rowspan="3">Session 5</td><td>Accuracy</td><td>1</td><td>2</td><td>14</td><td>15</td><td>1</td><td>1</td><td>−0.76</td><td>0.82</td></tr><tr><td>Clarity</td><td>0</td><td>3</td><td>14</td><td>14</td><td>2</td><td>1</td><td>−0.82</td><td>0.76</td></tr><tr><td>Achievability</td><td>1</td><td>2</td><td>14</td><td>13</td><td>3</td><td>1</td><td>−0.76</td><td>0.71</td></tr></tbody></table>

The validation process across these three sessions revealed both strengths and areas for improvement in the HAIC-MM framework. Analysis exposed a clear pattern of stronger validation at foundational levels with decreasing consensus as maturity levels increased. This pattern indicated challenges in describing advanced maturity states for SMEs. However, the subsequent revision process proved highly effective across accuracy, clarity, and achievability criteria among participants. The dramatic shift from predominantly negative responses pre-revision to strongly positive responses post-revision validates the iterative development approach and suggests the final framework better aligns with SME needs and practical implementation requirements.

## 8 Final Model Structure

Based on the iterative development and improvements, our resulting HAIC-MM contains 32 capabilities across 7 dimensions. For each capability, an SME could identify what maturity level they are currently at and use our model to identify how they could increase their maturity level further. In the next phase of our work, we will build these evaluation metrics and guidance for maturity advancement. However, the identification of HAIC-MM dimensions and capabilities provides current value to SMEs, where they can begin to assess important elements for successful human-AI collaboration, and even tailor the maturity levels to their own area of application. The final structure of our HAIC-MM is provided in Table [^13].

<table><thead><tr><th>Dimension</th><th>Capability</th><th>Condensed description</th></tr></thead><tbody><tr><td rowspan="5">AI-enhanced leadership and strategy</td><td>Augmented decision making</td><td>Use AI and data analytics to enhance leaders’ decision-making with accurate, data-driven insights.</td></tr><tr><td>Leadership AI literacy</td><td>Equip leaders with a deep understanding of AI to champion initiatives and leverage AI effectively.</td></tr><tr><td>Inclusive AI vision communication</td><td>Communicate the AI vision clearly across all levels, fostering alignment with organizational goals.</td></tr><tr><td>AI strategy alignment</td><td>Align AI initiatives with business objectives to maximize competitive advantage and ROI.</td></tr><tr><td>AI adoption readiness assessment</td><td>Assess readiness for AI by evaluating infrastructure, skills, and available resources.</td></tr><tr><td rowspan="4">Adaptive AI culture and empowerment</td><td>Comprehensive AI training & development</td><td>Build an AI-focused training program to enhance collaboration and adaptability.</td></tr><tr><td>AI partnership index</td><td>Develop metrics to assess the quality and effectiveness of human-AI collaboration.</td></tr><tr><td>Workforce AI adaptability</td><td>Enhance adaptability to AI-driven changes through targeted training and support.</td></tr><tr><td>Psychological safety in AI collaboration</td><td>Create a safe environment for employees to interact openly with AI, promoting innovation.</td></tr><tr><td rowspan="5">Human-centric AI integration and experience</td><td>Human-centered AI design</td><td>Design AI systems that prioritize user needs, ensuring usability and accessibility.</td></tr><tr><td>AI integration effectiveness</td><td>Ensure smooth AI integration into workflows, minimizing disruptions and enhancing productivity.</td></tr><tr><td>Employee experience with AI tools</td><td>Improve user interaction with AI through feedback-driven interface adjustments.</td></tr><tr><td>Human-AI collaboration quality</td><td>Measure collaboration productivity by evaluating communication, task completion, and outcomes.</td></tr><tr><td>Human trust in AI assessment</td><td>Assess and foster trust in AI through transparency, reliability, and employee involvement.</td></tr><tr><td rowspan="4">Harmonizing AI and human processes</td><td>AI-driven process optimization</td><td>Use AI to optimize processes, increase efficiency, and eliminate redundancies.</td></tr><tr><td>Human-AI collaboration index</td><td>Create metrics to quantify collaboration effectiveness between humans and AI.</td></tr><tr><td>Human-AI task flow</td><td>Design workflows that distribute tasks effectively between humans and AI.</td></tr><tr><td>Adaptive task allocation</td><td>Use real-time assessments to dynamically assign tasks to humans or AI, optimizing resources.</td></tr><tr><td rowspan="4">Human-centered AI customer engagement</td><td>AI-enhanced customer engagement</td><td>Personalize customer interactions with AI, improving experience and satisfaction.</td></tr><tr><td>Customer insights on AI experiences</td><td>Collect feedback on AI interactions to refine and improve customer-facing AI tools.</td></tr><tr><td>Human-AI Response integration</td><td>Enable seamless coordination between humans and AI in customer service for efficient support.</td></tr><tr><td>Human-AI collaborative resolution rate</td><td>Measure resolution success in issues solved through human-AI collaboration.</td></tr><tr><td rowspan="6">AI ethics and human oversight</td><td>AI ethical oversight</td><td>Establish governance structures to oversee ethical AI deployment.</td></tr><tr><td>AI data compliance</td><td>Ensure AI operations comply with data protection laws and standards.</td></tr><tr><td>AI governance effectiveness</td><td>Assess and strengthen AI governance for policy enforcement and risk management.</td></tr><tr><td>AI operational transparency</td><td>Maintain transparent communication about AI operations to foster trust.</td></tr><tr><td>Responsible AI practices</td><td>Adopt best practices to ensure ethical, fair, and accountable AI usage.</td></tr><tr><td>Equity and fairness assessment</td><td>Promote fairness in AI systems with inclusive policies and bias mitigation.</td></tr><tr><td rowspan="4">Inclusive AI governance and learning</td><td>Achieving diversity in AI training data</td><td>Ensure diverse and representative data in AI training to reduce biases.</td></tr><tr><td>Assessing AI impact on workforce roles</td><td>Analyze how AI impacts job roles and plan reskilling/upskilling as needed.</td></tr><tr><td>Implementing inclusive AI decision-making</td><td>Involve diverse perspectives in AI-related decisions to promote fairness.</td></tr><tr><td>Adaptive AI workforce upskilling</td><td>Provide ongoing AI skill development to maintain a proficient and adaptable workforce.</td></tr></tbody></table>

Further, Figure [5](#sys70031-fig-0005) provides a visual overview of the final HAIC-MM framework, illustrating the seven core dimensions and 32 associated capabilities designed to guide SMEs in assessing and advancing their human-AI collaboration maturity across five distinct levels, from initial exploration to a fully symbiotic partnership.

![](https://incose.onlinelibrary.wiley.com/cms/asset/8b3addd7-0f18-48f6-9494-c2f1dc5cd977/sys70031-fig-0005-m.jpg)

FIGURE 5 Open in figure viewer PowerPoint HAIC-MM's final framework structure.

### 8.1 HAIC-MM Tool and Implementation

An online platform was developed to operationalize the HAIC-MM, transforming the model into a practical tool for SMEs. The tool is freely available at [www.haicmm.com](http://www.haicmm.com/). The HAIC-MM interface follows a structured flow:
1. *Questionnaire Administration*: Respondents complete a series of questions aligned with the 32 capabilities to evaluate their organization's current practices, processes, and culture in relation to human-AI collaboration.
2. *Scoring Algorithm*: Responses are processed through the HAIC-MM assessment engine to calculate capability and dimension scores.
3. *Maturity Level Assignment*: Final scores are mapped to one of five maturity levels.
4. *Report Generation*: The tool generates a suite of reports, including an executive summary, gap analysis, dimension deep dive, strategic roadmap, and tactical action plan.

## 9 Pilot Testing

Pilot testing of the final HAIC-MM structure and online assessment tool was conducted as described in this section.

### 9.1 Methodology

The pilot testing involved three industry professionals external to the research team. The participants held the following positions within their organizations: Vice President of Engineering, Director of Customer Service, and Director of Finance. These participants were recruited through the authors’ professional network.

Each participant completed the full HAIC-MM assessment via the online platform. They were instructed to assess their division's practices related to human-AI collaboration. While early surveys and focus groups validated the model's content and structure, this pilot served as practitioner validation, confirming that the complete system produces useful, actionable insights for organizations.

Following completion, participants responded to a survey addressing the tool's usability, scope, real-world applicability, and practical insights. Questions used a 5-point Likert scale, with responses greater than 3 favorable, less than 3 unfavorable, and equal to 3 as neutral. Qualitative feedback was also gathered using open-ended questions.

### 9.2 Results

#### 9.2.1 Duration

Participants estimated the time required to complete the assessment: two reported 60–90 min, and one reported 30–60 min. In an open-ended prompt, all indicated the duration was appropriate:
- “The length is commensurate with the depth of analysis.”
- “The length is substantial but justifiable for the depth of analysis.”
- “It felt a bit long, but I understand you need lots of info.”

#### 9.2.2 Clarity

Participants were asked how strongly they agreed with the following three statements: (1) the assessment questions were clear and understandable, (2) the descriptions of the 32 capabilities were clear and understandable, and (3) the scoring methodology was explained clearly enough to understand why they received specific capability and dimension scores. For each of these questions, the average rating was 3.67, indicating the content was clear but could benefit from refinement.

#### 9.2.3 Scope and Balance

Participants reported that the HAIC-MM appropriately balanced human factors and technical AI capabilities (4.33), that the assessment questions effectively captured both human and AI information (4.00), and that the dimensions (4.67) and available response options (4.00) were comprehensive. They also evaluated the HAIC-MM as suitable for small- and medium-sized enterprises specifically (4.33), relevant to the current challenges in their industry (4.67), and organizations in general (4.67) regarding AI adoption.

#### 9.2.4 Applicability of Output

Participants rated the information (4.67) and the recommendations (4.67) in the results as useful. While opportunity for improvement, they agreed the reports enabled guidance for immediate action (3.67), were feasible to implement (3.67), and could inform strategic decision-making in their organization (3.67).

#### 9.2.5 Overall

Participants were satisfied with their overall experience using the HAIC-MM (4.00) and would recommend the HAIC-MM to other organizations looking to improve their human-AI collaboration (4.00). Lastly, they concluded that the HAIC-MM framework (i.e., model, assessment, and reports) provides valuable insights for improving human-AI collaboration (4.33).

## 10 Discussion

The development of the HAIC-MM involved a rigorous validation process using surveys, focus groups, and pilot testing. This multi-stage approach ensured that the model was not only theoretically robust but also practically aligned with the realities faced by SMEs. Through this process, we were able to refine the model's structure, validate its dimensions and capabilities with industry professionals, and confirm its usability as a publicly available assessment and planning tool.

The validated HAIC-MM offers SMEs a practical way to assess and improve their readiness for human-AI collaboration, but it also provides a structured pathway for action that extends beyond conceptual analysis. A central contribution of this work is the transformation of the model from an academic construct into a publicly available online tool that organizations can immediately use to evaluate their current practices, identify capability gaps, and generate actionable recommendations. While the model is built on rigorous theoretical foundations, its greatest practical value lies in helping SMEs move from awareness of AI challenges to a structured, staged approach for adoption. The HAIC-MM tool generates detailed outputs such as a gap analysis, maturity profiles, strategic roadmaps, and tailored action plans. These resources allow organizations with limited budgets and technical expertise to make informed, prioritized decisions about where to invest in capability development, leadership engagement, and workforce training, rather than pursuing costly, poorly targeted AI initiatives.

This study also highlights the practical impact of HAIC-MM for SMEs that often lack the resources of larger enterprises. The tool provides a way to diagnose readiness and capability gaps that are otherwise hidden in traditional technology adoption efforts. It supports leadership by clarifying how AI strategy can be aligned with core business objectives and by providing a systematic method to communicate that vision across the organization. The model's focus on teamwork, trust, and ethical oversight also helps build workforce confidence and reduce resistance to change, which are critical issues in small organizations where employees often carry multiple roles. Pilot testing demonstrated that the outputs of the tool are immediately valuable for planning; participants reported that the automated reports informed strategic decision-making, helped identify feasible AI use cases, and built confidence in advancing AI adoption responsibly.

A key feature of this work is the iterative evolution of the maturity model from its initial draft to the final validated framework. The model began as a conceptual synthesis of 30 existing AI, digital transformation, and human-machine teaming models, organized into early metamodels and pivot models that identified gaps specific to SMEs. These early versions were validated quantitatively through a survey of 100 industry professionals, which confirmed the relevance and comprehensiveness of the proposed dimensions and capabilities. Insights from the survey were then explored qualitatively through five focus group sessions with SME leaders and practitioners, which revealed where descriptions were unclear, overly ambitious, or misaligned with real-world SME conditions. Based on this feedback, four new capabilities were added (i.e., AI Adoption Readiness Assessment, Human Trust in AI Assessment, Data Quality Assurance for AI, and Equity and Fairness Assessment) while multiple maturity level descriptions were clarified and reframed to be more practical and measurable. The final step involved implementing the refined model as a digital tool and pilot testing it with industry practitioners to ensure that it produced actionable and usable outputs. This transparent, user-informed development process strengthens confidence in the model's rigor and relevance for SME contexts.

While HAIC-MM has been validated and operationalized, we acknowledge that the study concludes at the stakeholder approval phase of the development lifecycle rather than proceeding to full-scale, long-term deployment. This limitation is significant, as it means longitudinal evidence of organizational transformation and performance gains is not yet available. However, stopping at this stage reflects a deliberate focus on ensuring that the model is both conceptually sound and practically implementable before larger-scale adoption studies are undertaken. Future research should build on this foundation by tracking SMEs over time as they use HAIC-MM to guide AI adoption, quantifying outcomes such as return on investment, workforce adaptation, trust in AI, and ethical compliance.

By documenting this process, HAIC-MM demonstrates how rigorous, user-informed model development can bridge the gap between theory and application. It provides a human-centered, systems-engineering approach that balances technical AI capabilities with organizational readiness and workforce empowerment, offering both a practical adoption pathway for SMEs and a methodological blueprint for researchers creating maturity models in emerging technology contexts.

## 11 Conclusion

HAIC-MM addresses a critical gap in SME AI adoption by providing a validated framework and online assessment tool for cultivating effective human-AI collaboration. Through extensive validation incorporating survey data, focus group insights, and practitioner pilot testing, the framework demonstrates how organizations can balance technical capabilities with human factors while acknowledging resource constraints. Its strength lies in guiding the development of collaborative partnerships between employees and AI tools, emphasizing trust development, ethical leadership oversight, and adaptive task allocation.

By combining technical guidance with human-centered principles, the framework empowers SMEs to build trust, strengthen ethical oversight, and develop adaptive workforces while managing resource limitations. HAIC-MM thus serves as both an assessment instrument and a strategic enabler of organizational transformation, equipping leaders with actionable intelligence to balance human and AI strengths, mitigate risk, and prepare their organizations for a future of effective, ethical, and sustainable human-AI collaboration.

## Funding

The authors have nothing to report.

## Conflicts of Interest

The authors declare no conflicts of interest.

## Data Availability Statement

The data that support the findings of this study are available from the corresponding author upon reasonable request.

## References

## Citing Literature

[Download PDF](https://incose.onlinelibrary.wiley.com/doi/pdf/10.1002/sys.70031)

back

[^1]: | Model | Industry focus | Implementation complexity | SME relevance | Key strengths |
| --- | --- | --- | --- | --- |
| IBM AI Digital | General | Medium | High | Strong ethics & trust focus |
| Microsoft AI | Tech | Low | High | Business-tech alignment |
| ElementAI | Tech | Medium | Medium | Human-centric approach |
| StatWorkx | General | Low | High | Simple, actionable |
| Gartner AI | General | Low | Medium | Growth-oriented strategy |
| OVUM AI | Tech | High | Low | Sharp operational focus |
| Alsheibani AIMM | General | Medium | Medium | Innovation emphasis |
| AppliedAI | General | Medium | High | Operational excellence |
| Accenture AI | General | Medium | Medium | Holistic analysis |
| AIMI | General | High | Medium | Innovation management |

Similarly, Table [2](#sys70031-tbl-0002 "Link to table") details the 10 models evaluated relating to digital transformation, providing a summary of their scope, cost, and focus areas for SMEs.

[^2]: | Model | Industry focus | Maturity levels | Implementation cost | Capability coverage | Primary focus |
| --- | --- | --- | --- | --- | --- |
| PWC digital | General | 4 | High | High | Value chain digitization |
| IMPULS | Manuf. | 6 | Medium | High | Smart operations |
| VTT digital | General | 5 | Low | High | Strategy integration |
| Capgemini | General | 4 | High | High | Customer experience |
| BCG digital | General | 4 | High | High | Leadership commitment |
| Forrester | Tech | 4 | Medium | High | Cultural transformation |
| McKinsey | General | 3 | High | Medium | Strategic alignment |
| Deloitte | General | 5 | High | High | Customer-centricity |
| Acatech | Manuf. | 5 | Medium | Medium | Smart solutions |
| KPMG digital | General | 5 | High | High | Digital readiness |

Lastly, the 10 human-machine teaming models evaluated for HAIC-MM are summarized in Table [3](#sys70031-tbl-0003 "Link to table")

[^3]: | Model | Collab. focus | Technical depth | Implement. guidance | Key HMT principles | Primary application |
| --- | --- | --- | --- | --- | --- |
| CIQ | High | Medium | Medium | Common ground, observability | Team dynamics |
| CMF | High | Medium | High | Trust, directability | Process optimization |
| TSAC | Medium | High | Medium | Adaptability, trust | Situational awareness |
| HAT | High | High | Medium | Observability, directability | Autonomy integration |
| HMHR | Medium | High | Low | Direction, adaptability | Robot collaboration |
| FAHMT | High | Medium | High | Adaptability, solutions | Adaptive teaming |
| TST | Medium | High | Medium | Common ground, trust | Synthetic teammates |
| MUHMT | High | Medium | High | Trust, information | Mutual understanding |
| MAHMT | High | High | High | Adaptability, solutions | Model-based HMT |
| R-HMT | High | High | High | Common ground, trust | Resilient teaming |

[^4]: <table><thead><tr><th rowspan="2">HAIC-MM dimension</th><th colspan="2">Question 1</th><th colspan="2">Question 2</th></tr><tr><th><i>Mean</i></th><th><i>Scale</i></th><th><i>Mean</i></th><th><i>Scale</i></th></tr></thead><tbody><tr><td>Collaborative strategy leadership</td><td>5.2</td><td>Importance</td><td>5.0</td><td>Agreement</td></tr><tr><td>Empowerment and adaptive culture</td><td>4.4</td><td>Importance</td><td>4.2</td><td>Criticality</td></tr><tr><td>Integrated tech. and user experience</td><td>4.8</td><td>Importance</td><td>4.7</td><td>Essential</td></tr><tr><td>Process harmonization</td><td>4.8</td><td>Importance</td><td>4.8</td><td>Beneficial</td></tr><tr><td>Human-centric customer engagement</td><td>4.3</td><td>Significance</td><td>4.5</td><td>Essentialness</td></tr><tr><td>Data ethics and human oversight</td><td>4.8</td><td>Importance</td><td>4.5</td><td>Vitalness</td></tr><tr><td>Inclusive goals and continuous learning</td><td>4.6</td><td>Importance</td><td>4.6</td><td>Significance</td></tr></tbody></table>

[^5]: (1)

[^6]: | Participant | Positive | Neutral | Negative | Total | Sentiment score |
| --- | --- | --- | --- | --- | --- |
| Manager, Marketing | 15 | 2 | 1 | 18 | 0.78 |
| VP Engineering | 18 | 3 | 1 | 22 | 0.77 |
| VP Sales | 13 | 2 | 2 | 17 | 0.65 |
| Manager, Digital Products | 11 | 2 | 1 | 14 | 0.71 |
| Dir. Customer Service | 12 | 2 | 2 | 16 | 0.63 |
| VP Human Resources | 12 | 3 | 1 | 16 | 0.69 |
| Dir. Process Improvement | 14 | 4 | 2 | 20 | 0.60 |
| Dir. Finance | 8 | 5 | 1 | 14 | 0.50 |
| VP of Claims Management | 10 | 8 | 2 | 20 | 0.40 |
| Dir. IT Operations | 8 | 12 | 8 | 28 | 0.00 |
| Total | 121 | 43 | 21 | 185 | 0.54 |

The analysis in Table [6](#sys70031-tbl-0006 "Link to table") revealed considerable sentiment improvement across all HAIC-MM dimensions following the review and refinement of their purposes and descriptions. Initial sentiments were notably negative toward overall purposes, ranging from −0.5 (Harmonizing Processes) to −0.1 (Governance & Learning), indicating substantial initial concerns. Post-refinement, all dimensions achieved positive sentiments, with Ethics & Oversight and Customer Engagement showing the most dramatic improvements, reaching 0.9 from −0.3 and −0.2, respectively. The observed improvement in initial to final sentiment scores across all dimensions demonstrates the successful refinement of the model's dimension purposes and strong stakeholder alignment with their final concept.

[^7]: <table><thead><tr><td></td><th colspan="3">Before</th><th colspan="3">After</th><td></td><td></td></tr><tr><th>Dimension</th><th>+</th><th>0</th><th>—</th><th>+</th><th>0</th><th>—</th><th>Initial Score</th><th>Final Score</th></tr></thead><tbody><tr><td>Harmonizing processes</td><td>1</td><td>3</td><td>6</td><td>6</td><td>3</td><td>1</td><td>−0.5</td><td>0.5</td></tr><tr><td>Empowerment & culture</td><td>1</td><td>4</td><td>5</td><td>6</td><td>3</td><td>1</td><td>−0.4</td><td>0.5</td></tr><tr><td>Ethics & oversight</td><td>2</td><td>3</td><td>5</td><td>9</td><td>1</td><td>0</td><td>−0.3</td><td>0.9</td></tr><tr><td>Human-centric integration</td><td>2</td><td>3</td><td>5</td><td>8</td><td>1</td><td>1</td><td>−0.3</td><td>0.7</td></tr><tr><td>AI-enhanced leadership</td><td>2</td><td>3</td><td>5</td><td>7</td><td>2</td><td>1</td><td>−0.3</td><td>0.6</td></tr><tr><td>Customer engagement</td><td>2</td><td>4</td><td>4</td><td>9</td><td>1</td><td>0</td><td>−0.2</td><td>0.9</td></tr><tr><td>Governance & learning</td><td>3</td><td>3</td><td>4</td><td>8</td><td>2</td><td>0</td><td>−0.1</td><td>0.8</td></tr></tbody></table>

A similar analysis for the capabilities is shown in Table [7](#sys70031-tbl-0007 "Link to table"), which also revealed significant improvements post-refinement. Of the original 28 capabilities, conversations led to 24 of the capabilities getting revised. These revised capabilities showed substantial enhancement, moving from −0.5 initial sentiment to 0.6 final sentiment. The four unchanged capabilities maintained a consistent 80% sentiment throughout, validating their original design.

[^8]: <table><thead><tr><td></td><td></td><th colspan="3">Before</th><th colspan="3">After</th><td></td><td></td></tr><tr><th>Category</th><th># of Capabilities</th><th>+</th><th>0</th><th>—</th><th>+</th><th>0</th><th>—</th><th>Initial Score</th><th>Final Score</th></tr></thead><tbody><tr><td>Revised capabilities</td><td>24</td><td>1</td><td>2</td><td>5</td><td>7</td><td>2</td><td>1</td><td>−0.50</td><td>0.60</td></tr><tr><td>Unchanged capabilities</td><td>4</td><td>8</td><td>2</td><td>0</td><td>8</td><td>2</td><td>0</td><td>0.80</td><td>0.80</td></tr><tr><td>New capabilities added</td><td>4</td><td>—</td><td>—</td><td>—</td><td>7</td><td>2</td><td>1</td><td>—</td><td>0.60</td></tr></tbody></table>

During the focus group sessions, four new capabilities were identified as missing aspects of human-AI collaboration and were added to strengthen the model: AI Adoption Readiness Assessment, Human Trust in AI Assessment, Data Quality Assurance for AI, and Equity and Fairness Assessment. These new additions achieved a 0.6 final sentiment, indicating successful integration into the model.

A similar analysis of HAIC-MM maturity levels is shown in Table [8](#sys70031-tbl-0008 "Link to table"), also illustrating significant improvements following the refinement of level descriptions and titles against their relevance within human-AI collaboration. Four of the five levels showed substantial positive changes in sentiment, with initial negative scores improving to positive scores. The most dramatic improvement was seen in Level 4, which evolved from “Strategic” to “AI-Aligned.” Notably, Level 5 “Symbiotic” maintained its strong positive sentiment of 0.8 throughout, requiring no revision and validating its original conceptualization as the model's highest maturity level. These improvements demonstrate the effectiveness of the refinement process in creating more clearly defined and meaningful maturity levels.

[^9]: | Level | Initial title | Initial score | Revised title | Revised score |
| --- | --- | --- | --- | --- |
| 1 | Exploratory | −0.20 | AI exploration | 0.50 |
| 2 | Developing | −0.30 | AI-enabled | 0.50 |
| 3 | Integrated | −0.20 | AI-embedded | 0.40 |
| 4 | Strategic | −0.20 | AI-aligned | 0.60 |
| 5 | Symbiotic | 0.80 | Symbiotic | 0.80 |

Last, the analysis of stakeholder responses to the two primary questions, Table [9](#sys70031-tbl-0009 "Link to table"), revealed strong support for the HAIC-MM. Regarding the question relating to the need for the HAIC-MM, seven participants expressed positive support, with two neutral responses and one negative response, achieving a moderate consensus level. The second question regarding the comprehensiveness of HAIC-MM demonstrated even stronger support with eight positive responses, one neutral, and one negative position, reaching a high consensus level. The higher consensus on comprehensiveness suggests that while there is solid agreement on the need for the model, there is even stronger confirmation that the proposed model effectively captures the essential elements of human-AI collaboration. Only IT Operations maintained consistent concerns, while Finance remained neutral, indicating potential areas for technical and operational consideration in future refinements.

[^10]: | Overall questions | Positive | Neutral | Negative | Total | Sentiment score |
| --- | --- | --- | --- | --- | --- |
| Need for HAIC-MM | 7 | 2 | 1 | 10 | 0.60 |
| HAIC-MM comprehensiveness | 8 | 1 | 1 | 10 | 0.70 |

In Summary, focus group Sessions 1 and 2 demonstrated substantial improvement in the HAIC-MM's structure and stakeholder acceptance. Initial sentiment analysis revealed strong support from technical and customer-facing roles, while highlighting concerns in IT Operations. All seven dimensions progressed from negative sentiments to achieve positive final sentiments, while capability refinement showed similar success and introduced four new capabilities. Maturity level refinement saw four of five levels improve significantly. The strong consensus on the model's need and comprehensiveness (7 and 8 positive responses) validates the model's foundation while identifying key areas for technical implementation refinement.

[^11]: <table><thead><tr><th rowspan="2">Dimension</th><th rowspan="2">Number of capabilities</th><th colspan="5">Maturity level</th></tr><tr><th>1</th><th>2</th><th>3</th><th>4</th><th>5</th></tr></thead><tbody><tr><td>AI-enhanced leadership & strategy</td><td>5</td><td><p>4</p><p>(80%) <a href="#fnref:11">↩</a></p></td><td><p>1</p><p>(20%)</p></td><td><p>3</p><p>(60%)</p></td><td><p>4</p><p>(80%)</p></td><td><p>5</p><p>(100%)</p></td></tr><tr><td>Adaptive AI culture & empowerment</td><td>4</td><td><p>4</p><p>(100%)</p></td><td><p>3</p><p>(75%)</p></td><td><p>0</p><p>(0%)</p></td><td><p>4</p><p>(100%)</p></td><td><p>4</p><p>(100%)</p></td></tr><tr><td>Human-centric AI integration</td><td>5</td><td><p>4</p><p>(80%)</p></td><td><p>2</p><p>(40%)</p></td><td><p>1</p><p>(20%)</p></td><td><p>3</p><p>(60%)</p></td><td><p>3</p><p>(60%)</p></td></tr><tr><td>Harmonizing AI & human processes</td><td>4</td><td><p>2</p><p>(50%)</p></td><td><p>1</p><p>(25%)</p></td><td><p>2</p><p>(50%)</p></td><td><p>3</p><p>(75%)</p></td><td><p>4</p><p>(100%)</p></td></tr><tr><td>Human-centered AI customer engagement</td><td>4</td><td><p>1</p><p>(25%)</p></td><td><p>0</p><p>(0%)</p></td><td><p>1</p><p>(25%)</p></td><td><p>1</p><p>(25%)</p></td><td><p>1</p><p>(25%)</p></td></tr><tr><td>AI ethics & human oversight</td><td>6</td><td><p>4</p><p>(67%)</p></td><td><p>0</p><p>(0%)</p></td><td><p>1</p><p>(17%)</p></td><td><p>5</p><p>(83%)</p></td><td><p>6</p><p>(100%)</p></td></tr><tr><td>Inclusive AI governance & learning</td><td>4</td><td><p>1</p><p>(25%)</p></td><td><p>0</p><p>(0%)</p></td><td><p>1</p><p>(25%)</p></td><td><p>4</p><p>(100%)</p></td><td><p>4</p><p>(100%)</p></td></tr></tbody></table>

Based on these current state descriptions that required revision, we performed the focus group Sessions 3, 4, and 5, focusing on evaluating and improving the descriptions based on three key criteria: accuracy, clarity, and achievability. The analysis of these sessions is summarized in Table [11](#sys70031-tbl-0011 "Link to table"), revealing significant improvements after revisions. Specifically, sentiment scores improved from all negative towards the current state descriptions to all positive, achieving scores above 0.65 across all criteria.

[^12]: <table><thead><tr><th rowspan="2">Focus group</th><th rowspan="2">Current state description</th><th colspan="3">Before</th><th colspan="3">After</th><th rowspan="2">Initial score</th><th rowspan="2">Final score</th></tr><tr><th>+</th><th>0</th><th>—</th><th>+</th><th>0</th><th>—</th></tr></thead><tbody><tr><td rowspan="3">Session 3</td><td>Accuracy</td><td>2</td><td>3</td><td>12</td><td>14</td><td>2</td><td>1</td><td>−0.59</td><td>0.76</td></tr><tr><td>Clarity</td><td>1</td><td>2</td><td>14</td><td>15</td><td>1</td><td>1</td><td>−0.76</td><td>0.82</td></tr><tr><td>Achievability</td><td>3</td><td>2</td><td>12</td><td>13</td><td>3</td><td>1</td><td>−0.53</td><td>0.71</td></tr><tr><td rowspan="3">Session 4</td><td>Accuracy</td><td>1</td><td>4</td><td>19</td><td>20</td><td>3</td><td>1</td><td>−0.75</td><td>0.79</td></tr><tr><td>Clarity</td><td>0</td><td>3</td><td>21</td><td>19</td><td>4</td><td>1</td><td>−0.88</td><td>0.75</td></tr><tr><td>Achievability</td><td>2</td><td>3</td><td>19</td><td>18</td><td>4</td><td>2</td><td>−0.71</td><td>0.67</td></tr><tr><td rowspan="3">Session 5</td><td>Accuracy</td><td>1</td><td>2</td><td>14</td><td>15</td><td>1</td><td>1</td><td>−0.76</td><td>0.82</td></tr><tr><td>Clarity</td><td>0</td><td>3</td><td>14</td><td>14</td><td>2</td><td>1</td><td>−0.82</td><td>0.76</td></tr><tr><td>Achievability</td><td>1</td><td>2</td><td>14</td><td>13</td><td>3</td><td>1</td><td>−0.76</td><td>0.71</td></tr></tbody></table>

The validation process across these three sessions revealed both strengths and areas for improvement in the HAIC-MM framework. Analysis exposed a clear pattern of stronger validation at foundational levels with decreasing consensus as maturity levels increased. This pattern indicated challenges in describing advanced maturity states for SMEs. However, the subsequent revision process proved highly effective across accuracy, clarity, and achievability criteria among participants. The dramatic shift from predominantly negative responses pre-revision to strongly positive responses post-revision validates the iterative development approach and suggests the final framework better aligns with SME needs and practical implementation requirements.

[^13]: <table><thead><tr><th>Dimension</th><th>Capability</th><th>Condensed description</th></tr></thead><tbody><tr><td rowspan="5">AI-enhanced leadership and strategy</td><td>Augmented decision making</td><td>Use AI and data analytics to enhance leaders’ decision-making with accurate, data-driven insights.</td></tr><tr><td>Leadership AI literacy</td><td>Equip leaders with a deep understanding of AI to champion initiatives and leverage AI effectively.</td></tr><tr><td>Inclusive AI vision communication</td><td>Communicate the AI vision clearly across all levels, fostering alignment with organizational goals.</td></tr><tr><td>AI strategy alignment</td><td>Align AI initiatives with business objectives to maximize competitive advantage and ROI.</td></tr><tr><td>AI adoption readiness assessment</td><td>Assess readiness for AI by evaluating infrastructure, skills, and available resources.</td></tr><tr><td rowspan="4">Adaptive AI culture and empowerment</td><td>Comprehensive AI training & development</td><td>Build an AI-focused training program to enhance collaboration and adaptability.</td></tr><tr><td>AI partnership index</td><td>Develop metrics to assess the quality and effectiveness of human-AI collaboration.</td></tr><tr><td>Workforce AI adaptability</td><td>Enhance adaptability to AI-driven changes through targeted training and support.</td></tr><tr><td>Psychological safety in AI collaboration</td><td>Create a safe environment for employees to interact openly with AI, promoting innovation.</td></tr><tr><td rowspan="5">Human-centric AI integration and experience</td><td>Human-centered AI design</td><td>Design AI systems that prioritize user needs, ensuring usability and accessibility.</td></tr><tr><td>AI integration effectiveness</td><td>Ensure smooth AI integration into workflows, minimizing disruptions and enhancing productivity.</td></tr><tr><td>Employee experience with AI tools</td><td>Improve user interaction with AI through feedback-driven interface adjustments.</td></tr><tr><td>Human-AI collaboration quality</td><td>Measure collaboration productivity by evaluating communication, task completion, and outcomes.</td></tr><tr><td>Human trust in AI assessment</td><td>Assess and foster trust in AI through transparency, reliability, and employee involvement.</td></tr><tr><td rowspan="4">Harmonizing AI and human processes</td><td>AI-driven process optimization</td><td>Use AI to optimize processes, increase efficiency, and eliminate redundancies.</td></tr><tr><td>Human-AI collaboration index</td><td>Create metrics to quantify collaboration effectiveness between humans and AI.</td></tr><tr><td>Human-AI task flow</td><td>Design workflows that distribute tasks effectively between humans and AI.</td></tr><tr><td>Adaptive task allocation</td><td>Use real-time assessments to dynamically assign tasks to humans or AI, optimizing resources.</td></tr><tr><td rowspan="4">Human-centered AI customer engagement</td><td>AI-enhanced customer engagement</td><td>Personalize customer interactions with AI, improving experience and satisfaction.</td></tr><tr><td>Customer insights on AI experiences</td><td>Collect feedback on AI interactions to refine and improve customer-facing AI tools.</td></tr><tr><td>Human-AI Response integration</td><td>Enable seamless coordination between humans and AI in customer service for efficient support.</td></tr><tr><td>Human-AI collaborative resolution rate</td><td>Measure resolution success in issues solved through human-AI collaboration.</td></tr><tr><td rowspan="6">AI ethics and human oversight</td><td>AI ethical oversight</td><td>Establish governance structures to oversee ethical AI deployment.</td></tr><tr><td>AI data compliance</td><td>Ensure AI operations comply with data protection laws and standards.</td></tr><tr><td>AI governance effectiveness</td><td>Assess and strengthen AI governance for policy enforcement and risk management.</td></tr><tr><td>AI operational transparency</td><td>Maintain transparent communication about AI operations to foster trust.</td></tr><tr><td>Responsible AI practices</td><td>Adopt best practices to ensure ethical, fair, and accountable AI usage.</td></tr><tr><td>Equity and fairness assessment</td><td>Promote fairness in AI systems with inclusive policies and bias mitigation.</td></tr><tr><td rowspan="4">Inclusive AI governance and learning</td><td>Achieving diversity in AI training data</td><td>Ensure diverse and representative data in AI training to reduce biases.</td></tr><tr><td>Assessing AI impact on workforce roles</td><td>Analyze how AI impacts job roles and plan reskilling/upskilling as needed.</td></tr><tr><td>Implementing inclusive AI decision-making</td><td>Involve diverse perspectives in AI-related decisions to promote fairness.</td></tr><tr><td>Adaptive AI workforce upskilling</td><td>Provide ongoing AI skill development to maintain a proficient and adaptable workforce.</td></tr></tbody></table>

Further, Figure [5](#sys70031-fig-0005) provides a visual overview of the final HAIC-MM framework, illustrating the seven core dimensions and 32 associated capabilities designed to guide SMEs in assessing and advancing their human-AI collaboration maturity across five distinct levels, from initial exploration to a fully symbiotic partnership.

![](https://incose.onlinelibrary.wiley.com/cms/asset/8b3addd7-0f18-48f6-9494-c2f1dc5cd977/sys70031-fig-0005-m.jpg)

FIGURE 5 Open in figure viewer PowerPoint HAIC-MM's final framework structure.