
```
Transportation Research Record
2025, Vol. XX(X) 1–
©National Academy of Sciences:
Transportation Research Board 2025
Article reuse guidelines:
sagepub.com/journals-permissions
DOI: 10.1177/ToBeAssigned
journals.sagepub.com/home/trr
SAGE
```
### Sherida van den Bent^1 and Romana Pernisch1,2and Stefan Schlobach^1

**Abstract**
Knowledge Elicitation, the process of extracting and structuring expert knowledge, is crucial for fields ranging from Artificial
Intelligence (AI) to decision support systems. Traditionally, this process has relied on human experts, making it time
consuming and resource intensive. With the rapid advancement of Large Language Models (LLMs), there is growing
interest in their potential role in Knowledge Elicitation and ontology generation. This research investigates the feasibility of
using LLMs, specifically ChatGPT v4, for automated Knowledge Elicitation and compares AI-led approaches to traditional
human expert interviews.
To evaluate this, a series of interviews were conducted with both human experts and an LLM, and the extracted knowledge
was transformed into RDF ontologies using different pipelines, ranging from AI-generated to human-created ontologies.
The research employs OQuaRE metrics and structural analysis to compare the generated ontologies against a base-
truth ontology. The results indicate that AI-led interviews are more time-efficient and structured compared to human
expert interviews. However, a human approach works better for ontology generation: AI-generated ontologies are more
standardized but missed a lot of data, whereas human-created ontologies captured more information.
These findings suggest that a hybrid approach, using LLMs as stand-ins for experts in the interview phase, while relying
on human knowledge engineers for ontology generation, offers the best balance between speed and quality in Knowledge
Elicitation.

### Introduction

Knowledge transfer, the process of conveying knowledge
from one entity to another, has long been recognized as
a crucial aspect of organizational and individual learning.
The very nature of knowledge - its tacitness, complexity,
and context-specificity - makes its transfer a challenging
endeavor ( 1 ). Historically, knowledge transfer primarily
relied on personal interaction. While effective, it is often
limited by time and cost constraints.

The digitalization of information and the advent of sophis-
ticated computation tools have revolutionized the way knowl-
edge is stored, retrieved, and shared. Artificial Intelligence
(AI), with its potential for automated reasoning and data
processing, has opened new possibilities for automating
knowledge assimilation. Among the advancements in AI,
Large Language Models (LLMs) like ChatGPT ( 2 ) have
demonstrated a remarkable ability to process vast amounts
of textual data, drawing insights and generating coherent
responses. However, these models also have limitations. They
operate largely on pattern recognition, without a real under-
standing of the underlying concepts. This makes them prone
to errors that are hard to pinpoint and fix ( 3 ). The output

```
of these models, therefore, often lack the depth, nuance, and
verifiability that human experts bring to the table.
Given these challenges, there is a need for a synergistic
approach to Knowledge Elicitation. This paper aims to
bridge the gap between human-led knowledge engineering
and machine automation. By combining the expertise of
human professionals and the efficiency of machines, the goal
of this research is to create a starting point for a method
for Knowledge Elicitation that is both fast and trustworthy.
To increase the efficiency of Knowledge Elicitation, it is
important to reduce the process’s time and resource demands.
Therefore, this research explores how LLMs can accelerate
Knowledge Elicitation without compromising output quality.
We investigate two research questions:
```
```
RQ1:How can you use a Large Language Model for the
process of Knowledge Elicitation?
```
(^1) Vrije Universiteit Amsterdam, the Netherlands
(^2) Discovery Lab, Elsevier, Amsterdam, the Netherlands
**Corresponding author:**
Stefan Schlobach, k.s.schlobach@vu.nl
Prepared usingTRR.cls[Version: 2020/08/31 v1.00]


```
2 Transportation Research Record XX(X)
```
RQ2:How does using a Large Language Model for the
process of Knowledge Elicitation compare to using
human knowledge engineers?

```
Given its broad scope, RQ1 is divided into two parts. The
first focuses on the data collection stage, which is typically
conducted through expert interviews. An alternative is to use
an LLM as a data source Next is the translation of that data
into an RDF ontology, a task usually performed by human
knowledge engineers. This raises the second sub-question:
These questions are addressed through a literature study,
resulting in the development of a method that integrates
LLMs into the Knowledge Elicitation process. To evaluate
the method’s effectiveness, it is necessary to compare it
with a traditional human-led pipeline. Efficiency gains are
only valuable if they don’t come at the cost of accuracy
or completeness. This leads us to the second research
question. RQ2 is also divided into two parts, covering both
data collection and ontology creation. Therefore, we will
focus first on the interview phase and then on the ontology
generation compared to the traditional manual approach.
To answer the first research question, we conducted a
literature study into the current state of the art regarding
the use of LLMs in Knowledge Elicitation. The study
revealed that while LLMs such as ChatGPT v4 are not
yet capable of generating fully accurate ontologies on their
own, they show great promise in assisting with structured
data collection. Their ability to provide consistent and well-
organized responses to open-ended questions makes them a
viable stand-in for human experts during interviews. Based
on these findings, we developed a pipeline that integrates
LLMs in the data collection phase, followed by ontology
generation either through AI or human knowledge engineers.
This hybrid approach is the foundation for the comparative
method used to answer the second research question.
Building on this method, the second research question
investigates the quality and efficiency of AI-assisted versus
human-led Knowledge Elicitation pipelines. The results
showed that LLM-led interviews were faster and more
structured. However, when it came to ontology construction,
human knowledge engineers outperformed AI, producing
ontologies that were richer in content and closer in structure
to a manually created base truth. Interestingly, AI-generated
ontologies tended to be more standardized but included
less data and occasionally hallucinated facts. These findings
suggest that the most effective strategy may be a hybrid
model: using LLMs for rapid and consistent data elicitation,
while relying on human expertise for ontology creation.
The rest of this paper is structured as follows. In the
following section, we provide an overview of related work,
including a literature review on Knowledge Elicitation and
the use of Large Language Models (LLMs). The next section,
we outline the experimental design, detailing the research’s
pipeline and methods of evaluation, followed by a section on
results. Section Discussion offers a detailed view on these
```
```
findings in light of the research questions followed by a
reflection on limitations, and suggests directions for future
research. Finally, in the last section we conclude this paper
and summize the key insights gained.
```
### Related Work

```
In this section, the topics of Knowledge Elicitation, LLMs,
and the application of LLMs in the field of Knowledge
Elicitation are examined. The current state of the art in
the areas of using LLMs for data collection and ontology
generation are looked at, and how LLMs can contribute to
the extraction and structuring of knowledge is analyzed. This
section aims to identify a clear method of using LLMs for the
process of Knowledge Elicitation.
```
### Knowledge Elicitation

```
Knowledge Elicitation, the systematic process of extracting
knowledge from individuals or groups, has its roots in
the early days of expert systems and AI ( 4 ). The initial
focus was on codifying expert knowledge into rule-based
systems, leading to the development of various techniques,
such as structured interviews, repertory grids, and protocol
analysis ( 5 ). As the field evolved, researchers recognized
the importance and challenges of extracting tacit knowledge:
knowledge that experts might find hard to articulate
explicitly ( 1 ). This led to the exploration of more interactive
and iterative methods, such as concept mapping and cognitive
task analysis, which aim to capture deeper layers of expert
cognition ( 6 ). The 21st century saw the integration of
computational tools and machine learning algorithms, further
refining the elicitation process and allowing for more
extensive and nuanced knowledge capture. Throughout its
history, Knowledge Elicitation has continuously adapted to
address the complexities of human cognition and the ever-
expanding technological landscape.
Knowledge Elicitation plays an important role in capturing
the tacit and explicit knowledge of human experts ( 1 ). This
knowledge is crucial for various fields, ranging from use
in research and development (for example, the development
of expert systems in the early days of AI ( 4 )) to cultural
and historical (for example, the preservation of indigenous
knowledge in cultural studies ( 7 )) as well as for use in
business (for example, capturing the expertise of seasoned
employees to help give training, drive innovations, and ensure
continuity in operations ( 8 )). Furthermore, in domains like
healthcare and aviation, accurate Knowledge Elicitation can
be a matter of life and death, helping to codify best practices
and prevent mistakes ( 9 ). As one can see from the previous
examples, Knowledge Elicitation is an important tool for
progress and preservation across disciplines.
As stated earlier, the process of Knowledge Elicitation
is important across multiple disciplines. However, it often
comes with significant costs, mostly in terms of the time
```

van den Bent, Pernisch and Schlobach 3

investment required from both experts and knowledge
engineers. Experts, who typically have demanding schedules,
must allocate substantial time to participate in interviews,
games, and other elicitation activities, taking them away
from their primary responsibilities ( 6 ). Knowledge engineers,
on the other hand, spend a lot of time not only on direct
interaction with experts, but also in preparation beforehand,
and analysis, documentation, and verification afterwards. The
total amount of hours expended can translate into significant
financial costs for organizations, especially when considering
the extra costs associated with diverting experts, who are
usually important employees, from their core tasks.
The state of the art in Knowledge Elicitation has
evolved significantly, using a combination of traditional
methodologies with new technology. Today, Knowledge
Elicitation does not only rely on conventional techniques
like structured interviews and observation, but increasingly
incorporates advanced computational tools. For example,
interactive machine learning (iML) systems enable a more
collaborative approach to knowledge capture, by facilitating
real-time feedback and model adjustment, making them well-
suited for iterative knowledge extraction ( 10 ). For instance,
Dzyuba et al. ( 11 ) developed an iML framework for pattern
mining where users iteratively rank small sets of patterns; the
system learns from these rankings to surface more relevant
or insightful patterns over time. This enables domain experts
to guide the discovery of meaningful rules or associations.
Similarly, Amershi et al. ( 12 ) introduced an iML tool for
creating custom contact groups in social networks, where
user selections are treated as positive examples to train a
classifier, allowing the system to learn and refine grouping
criteria dynamically. These kinds of systems help externalize
tacit expert knowledge into structured, machine-readable
form, which is a central goal of Knowledge Elicitation.
While the previously mentioned work on iML has shown
promising results in supporting Knowledge Elicitation,
these systems rely on iterative human feedback loops
within domain-specific applications. In contrast, this research
explores a more generalizable and scalable approach by using
LLMs to directly generate structured knowledge from natural
language interviews.

### Large Language Models

Although recent advancements in LLMs have accelerated
their capabilities, applications, and popularity significantly,
the history of these models spans several decades. The early
developments in the field of Natural Language Processing
(NLP) began with systems like ELIZA in 1966, a simple
program that mimicked human conversation by use of pattern
matching and substitution methodology ( 13 ). IBM created
the first statistical language models in 1980 that predicted
the next word in a sentence ( 14 ). During the 1990s, N-
gram models became fundamental in language modeling.
These models estimated the probability of a word based

```
on the preceding ’n-1’ words, enhancing the accuracy of
tasks like speech recognition and text prediction ( 15 ).
Simultaneously, Statistical Machine Translation (SMT)
systems emerged, leveraging bilingual text corpora to learn
translation patterns, marking a significant advancement
over earlier rule-based translation systems ( 16 ). The early
2000s saw the integration of neural networks into NLP.
Recurrent Neural Networks (RNNs), particularly Long Short-
Term Memory (LSTM) networks, were utilized to model
sequential data, capturing long-range dependencies in text.
In the 2010s, deep learning techniques revolutionized NLP.
Convolutional Neural Networks (CNNs) and advanced RNNs
improved performance in tasks like sentiment analysis and
machine translation ( 17 ). Then, everything changed when
the Transformer Architecture was introduced in 2017 ( 18 ). It
paved the way for, and formed the backbone of, the first GPT
(Generative Pre-trained Transformer) model by OpenAI ( 19 )
and BERT by Google ( 20 ).
Concerns about the reliability and trustworthiness of LLMs
have been a significant topic lately, especially when these
models are used to generate factual or structured knowledge.
Since this research uses LLMs as a primary data source for
knowledge elicitation, it is important to establish whether
they can be considered reliable in this context. The TrustLLM
study ( 21 ) evaluated mainstream LLMs across multiple
trustworthiness dimensions, such as truthfulness, safety, and
fairness. It found that proprietary models like ChatGPT
generally perform better than their open-source counterparts.
Specifically, ChatGPT v4 exhibited strong performance in
tasks like stereotype categorization and natural language
inference, showing greater resilience to adversarial attacks.
These findings directly informed the decision to use ChatGPT
v4 in this study. Given the need for accurate and consistent
knowledge outputs, it was essential to select a model
with demonstrated robustness across multiple trust-related
benchmarks. As such, ChatGPT v4 was chosen as the AI
participant due to its relatively high reliability and safety
within the current state of the art.
While LLMs are not yet capable of independently
generating OWL ontologies of sufficient quality, they have
shown considerable potential in assisting human modelers
by providing valuable suggestions. Merono-Panuela et ̃
al. ( 22 ) investigate the ability of LLMs, particularly
ChatGPT v4, to generate OWL modelling suggestions
based on ontological requirements. It was found that while
ChatGPT v4 can offer suggestions of comparable quality
to those of novice human modellers, it still requires human
input to refine and implement these suggestions in a
modelling environment such as Prot ́ege. While LLMs may ́
not be capable of independently writing complete OWL
ontologies, they serve as effective tools for guiding human
ontology engineers by suggesting appropriate structures and
alternatives, making the ontology creation process more
accessible for inexperienced modellers.
```

4 Transportation Research Record XX(X)

While existing research has demonstrated that LLMs can
offer useful modelling suggestions in controlled settings, it
remains unclear how these models perform autonomously in
a full ontology engineering pipeline. This research extends
beyond isolated suggestion tasks by evaluating LLMs across
the entire process, from data collection through interviews
to the generation and evaluation of complete ontologies.
Rather than treating LLMs purely as support tools for
human modellers, this research explores their potential as
autonomous or semi-autonomous agents in the knowledge
elicitation workflow.

### Discussion

Given the literature review above, we can answer the
first research question (RQ1):How can you use a Large
Language Model for the process of Knowledge Elicitation?
Based on the studies mentioned above, we will continue
with using ChatGPT v4 in this work. In more detail, we can
seperate the above research question into two parts below

RQ1.1:What is the current state of the art in using
a Large Language Model for data collection? Studies
like TrustLLM ( 21 ) have evaluated LLMs on criteria like
truthfulness, safety, and fairness, showing that proprietary
models (e.g., ChatGPT v4) outperform open-source models
in these areas. ChatGPT v4 in particular has shown robust
performance across trust-related benchmarks, including
stereotype detection and natural language inference, which
supports its use in reliable data generation.

RQ1.2:What is the current state of the art in
using a Large Language Model for ontology generation?
LLMs like ChatGPT v4 can suggest OWL modelling
elements (e.g., classes, properties, axioms) based on natural
language descriptions or requirements. These suggestions
are comparable in quality to those produced by novice
ontology engineers. However, LLMs currently require human
supervision and refinement, especially for integration in
formal modelling environments like Prot ́ege. ́

### Experimental Design

This research is designed to investigate and compare the
efficiency and accuracy of knowledge acquisition from both
human experts and an AI model, with a particular focus on
the context of niche subjects. Before selecting a field for
data collection, it was important to establish key criteria.
The chosen field needed to have human experts available
for interviews, be familiar to the researcher to facilitate
analysis, and contain a substantial amount of publicly
available information to ensure that ChatGPT could generate
meaningful responses. Based on these requirements, the
tabletop role-playing game (TTRPG) Dungeons & Dragons
(D&D)*†was selected, as it met all criteria effectively.
All interviews, ontologies, and evaluation data used in this
study are publicly available in the accompanying GitHub

```
repository‡. This repository contains the transcripts of both
human and AI-led interviews, all RDF ontologies created
throughout the pipeline, and the OQuaRE evaluation results
as well as the competency questions for the base truth
ontology. In this section, we explain the experimental design
and the rationales behind the different decisions that have
been made throughout the process.
```
### Base Truth Ontology

```
The base truth ontology was developed to serve as a reference
point for evaluating the structure and accuracy of AI-
generated ontologies. However, despite the abundance of
online resources, no comprehensive ontology for D&D was
available at the time of this research. Given this gap, we
constructed a base truth ontology from scratch.
A manual document analysis of the Player’s Handbook for
Dungeons & Dragons 5ˆth Edition (2014)§was conducted.
This process involved a section-by-section review of the
source material, during which key ontology components
were identified and recorded. Ontology classes were derived
from major conceptual categories such asRace,Class,
Spell, Equipment, and AbilityScore. Individual
instances (e.g., Elf, Fireball, Longsword) were
noted under their corresponding classes. Relationships
between entities were extracted by analysing mechanics
and rule structures, for instance,HasProficiencyWith,
IsBackgroundFeatureOf, or KnowsLanguage,
while datatype properties were used to encode
specific attributes such as HasCastingTime or
HasSpellLevel.
To guide the design and evaluate the adequacy of the
ontology, a set of competency questions was developed based
on the kinds of queries one should reasonably be able to
answer within the D&D domain. Table 1 lists these questions
along with the number of results returned for each. They
served as a benchmark to ensure the ontology could support
structured reasoning and enable meaningful comparisons
with the other ontologies generated in this study. [Romi]: we
should execute these also for all the generated ontologies...
```
### The Pipeline

```
To create the ontologies used in this study, a structured
pipeline was followed. The process begins with an
unstructured interview, in which either a human domain
expert or an LLM serves as the interviewee. In the case
of human interviewees, the conversations are transcribed,
either manually or using an AI transcription tool. For this
```
```
∗https://www.dndbeyond.com/
†https://en.wikipedia.org/wiki/Dungeons_&_Dragons
‡https://github.com/sheridavandenbent/
automated-knowledge-elicitation
§https://www.dndbeyond.com/sources/dnd/phb-
```

van den Bent, Pernisch and Schlobach 5

**Table 1.** Competency questions and amount of results
Question Results
Which class features belong to a Bard? 17
What proficiencies does a Fighter have? 16
What is the casting time of “Chill Touch”? 1
Which spells have a spell range of
“Touch”?

#### 72

```
Which spells require material compo-
nents?
```
#### 199

```
What are the Ideals associated with the
Charlatan background?
```
#### 6

```
What are the Flaws associated with the
Folk Hero background?
```
#### 6

```
What is the damage of a Shortbow? 1
What starting equipment does a Wizard
begin with?
```
#### 7

```
Human Expert
Interviewee
```
```
Human
transcriber
```
```
Human ontology
engineer
```
```
LLM interview
ChatGPT v
```
```
AI Transcriber
Whisper
```
```
LLM ontology
ChatGPT v
```
**Figure 1.** Visual representation of the pipeline

research, Whisper¶was selected as the transcription tool due
to its high accuracy and suitability for transcribing natural
conversations ( 23 ). Its multilingual capabilities also offer
flexibility for research involving non-English speakers, which
is especially important since this research involves interviews
with experts in Dutch. Furthermore, since it is developed by
OpenAI, the creators of ChatGPT, it complements the use
of OpenAI LLMs in this pipeline. In the case of the LLM
interview, the output is already in textual format and therefore
does not require transcription. The resulting transcripts are
then used as input for the ontology construction phase, where
either a human expert or an LLM is responsible for translating
the information into a formal ontology. A visual overview of
the pipeline can be found in Figure 1.
This pipeline results in the creation of multiple ontologies,
as illustrated in Table 2. Since two human experts were
interviewed, each human interview setup produced two
versions, effectively doubling the number of human-derived
ontologies. In total, ten ontologies were created through
various combinations of human and AI involvement,
excluding the base truth ontology used as a point of reference.

### Testing The Pipeline

This section addresses Research Question 2:How does using
a Large Language Model for the process of knowledge
elicitation compare to using human knowledge engineers?
To investigate this, the outputs of both human-led and AI-
assisted knowledge elicitation pipelines are systematically
compared. The goal is to evaluate the quality, structure, and

```
Table 2. Overview of acronyms to identify the different
engineering processes
Code Description
BT Base Truth ontology
AI-AI AI interview (AI), AI ontology (AI)
AI-H AI interview (AI), engineered ontology (H)
H1-AI-AI Expert 1 interview (H1), AI transcription
(AI), AI ontology (AI)
H1-AI-H Expert 1 interview (H1), AI transcription
(AI), engineered ontology (H)
H1-H-AI Expert 1 interview (H1), manual transcrip-
tion (H), AI ontology (AI)
H1-H-H Expert 1 interview (H1), manual transcrip-
tion (H), engineered ontology (H)
```
```
content of the resulting ontologies, with particular attention
to their alignment with a base truth ontology. To answer the
two sub-research questions associated with this comparison,
different evaluation strategies are applied, as detailed below.
RQ2.1:What is the difference between using a Large
Language Model and human experts as a source to gather
data?In order to answer this research question, a comparative
data collection procedure was performed involving human
experts and an LLM (ChatGPT v4). This consisted of
having semi-structured interviews with (separately) two
human domain experts, and with ChatGPT. The objective
was to evaluate differences in data collection dynamics,
including topical relevance, conversational structure, and
overall efficiency - criteria commonly used in qualitative
research to assess the usefulness and coherence of interview
content ( 24 ). These aspects are especially relevant when
interviews are intended as inputs for downstream knowledge
representation tasks, such as ontology construction.
For both the human expert interviews and the interaction
with ChatGPT v4, the interview began with the same
initial open-ended question: “Tell me about Dungeons and
Dragons.” Based on the responses, key concepts were
identified and noted down during the conversation. These
concepts then served as the basis for follow-up questions,
which included prompts such as “Tell me more about X” or
clarifying questions aimed at deepening the discussion and
eliciting more detailed information. This approach follows
the Applied Cognitive Task Analysis (ACTA) method ( 25 ),
which begins with an open-ended question and builds
on emerging concepts through adaptive probing. ACTA is
commonly used in knowledge elicitation to uncover expert
insights in a structured yet flexible manner. This approach
ensured a consistent starting point and comparable interaction
structure across both human and AI interviews, allowing for a
more balanced comparison of the data elicitation process and
resulting content.
```
```
¶https://openai.com/index/whisper/
```

6 Transportation Research Record XX(X)

To evaluate the efficiency and accuracy of different
transcription methods, a comparison was conducted between
manual human transcription and automated transcription
using Whisper, an AI-based speech-to-text tool developed
by OpenAI. The interviews with human experts were
conducted in Dutch, and were audio recorded. For the human
transcription method, a researcher manually transcribed the
recordings by listening to the audio and typing out the
spoken content in Dutch. The resulting transcripts were then
translated into English by the researcher. In parallel, the same
Dutch audio recordings were transcribed using Whisper,
which performs automated transcription and translation
simultaneously. The tool automatically transcribed and
translated the spoken Dutch directly into English, producing
an end-to-end transcription-translation output without human
intervention. The resulting transcripts from both methods
were compared on the basis of:

- Accuracy: Assessed by reviewing transcription and
    translation quality, identifying errors such as omis-
    sions, incorrect terms, or misinterpretations.
- Efficiency: Considered in terms of the time and effort
    involved in the combined transcription and translation
    process.

This comparison aimed to explore the trade-offs between
human and AI-assisted transcription-translation pipelines in
a multilingual Knowledge Elicitation context.
After the interviews, the resulting transcripts were
analysed to identify differences in the structure, clarity, and
relevance of the responses. The interview with ChatGPT
was already text-based and in English, so it did not need
transcribing. For the intents of the pipeline, we consider the
ChatGPT interviews as “transcribed by AI”.

RQ2.2:What is the difference between using a Large
Language Model and humans to create RDF ontologies from
textual data?.
In order to answer this question, the created ontologies will
be compared with the base truth ontology, on multiple facets,
the first of which is metrics.
The metrics of the ontologies are the fundamental
components of the ontology, for example the number of
classes, properties, and axioms. Such metrics give insight into
the size and complexity of an ontology. Once these metrics
are calculated, they will be compared with one another to get
a measure of similarity between the ontologies and the base
truth ontology.
It is also important to not only look at the similarities
between the ontologies, but also the difference in quality.
Among the various methodologies proposed for ontology
evaluation, the OntoClean method ( 26 ) and OQuaRE. Onto-
Clean uses formal, domain-independent properties to evalu-
ate the taxonomic structure of ontologies, focusing on con-
cepts like rigidity, identity, and unity. The OQuaRE (Ontol-
ogy Quality Requirements and Evaluation) method ( 27 )

```
evaluates ontologies across several dimensions, such as struc-
tural, functional adequacy, and maintainability, providing
a detailed and systematic approach to quality evaluation.
OQuaRE’s evaluation process involves the definition of
quality requirements, the identification of relevant metrics,
and the measurement and analysis of these metrics. This
structured approach allows for a thorough and objective
assessment of ontology quality, facilitating the identification
of areas for improvement. Moreover, OQuaRE supports the
comparison of different ontologies, enabling the selection of
the most suitable ontology for a given application based on
empirical quality data. As such, it will be used in this research
to compare ontologies with each other.
To assess the structural quality of the ontologies, a
hierarchy comparison was conducted as part of the overall
quality evaluation. The focus of this analysis is to examine
how the class hierarchies of the various ontologies aligned
with the structure of the base truth ontology. The comparison
is performed through a side-by-side inspection in Proteg ́ ́e,
allowing for a direct visual and structural assessment. For
each ontology, the following steps were taken:
```
1. The ontologies are compared side-by-side in Proteg ́ ́e,
    to visually inspect differences in the class hierarchies.
2. For each class in the compared ontologies, it is
    checked whether the class also existed in the base-truth
    ontology.
3. If a class is present in both ontologies, its position in
    the hierarchy is examined. Specifically, it is verified
    whether the class had the same parent class and
    whether the same set of child classes (i.e., subclasses)
    is present.

```
This process enables a systematic comparison of hier-
archical consistency and structural alignment between the
generated ontologies and the base-truth ontology.
To ensure consistency in hierarchy comparisons across
ontologies, several normalization steps were applied to
standardize class names and minimize discrepancies due to
formatting differences. Hyphens, underscores, and white
spaces were removed to create a uniform naming convention.
Additionally, specific terminology adjustments were made
in non-base truth ontologies to align with the base-truth
structure. The term Objectwas replaced with Item,
NPC was expanded to NonPlayerCharacter, and
PC to PlayerCharacter. CharacterStats was
changed toCharacterStatistics. Further refinements
included the removal of the prefix Character from
CharacterLevel, CharacterAbilityScore,
CharacterBackground, CharacterClass,
and CharacterRace. The term Place
was changed to Location. Additionally,
CharacterAbilityModifiers became
AbilityModifier, CharacterAbilityScores
was shortened to AbilityScore, and
```

van den Bent, Pernisch and Schlobach 7

**Table 3.** Interview duration and setup for human experts and
ChatGPT v

```
Interviewee Duration Participants
Expert 1 36:10 Expert & researcher
Expert 2 35:31 Expert & researcher
ChatGPT v4 ∼10:00 Researcher only
```
CharacterCharacteristics was aligned with
CharacterStatistics. These modifications ensured
that structural comparisons accurately reflected differences
in ontology construction rather than inconsistencies in
naming conventions.
Lastly, we analysed some entities in the ontologies
in more detail. The entities chosen for analysis were
selected due to their centrality in D&D’s mechanics
and their frequent occurrence across ontologies. For each
selected entity, the parent class of the entity is identified
to determine its placement within the broader ontology
framework. Additionally, child classes are examined to
assess whether the ontology captured relevant subcategories
and whether they align with the expected hierarchical
structure. The presence of sibling classes, or concepts
positioned at the same hierarchical level, is also evaluated
to identify inconsistencies or deviations in classification.
Beyond structural relationships, it is also analysed whether
each entity contains instances (individuals) and, if so, how
many.

### Results

This chapter presents the results of the study, organized
around the two main sub-questions of RQ2: (1) the
comparison between AI and human experts in the data
elicitation phase, and (2) the differences in ontology quality
when constructed by AI versus human knowledge engineers.
First we will go into the efficiency of the interview
and transcription methods, then ontology metrics, OQuaRE
quality scores, class hierarchy evaluations, entity structure,
and, lastly, hallucinated content.

### Interview and Transcription Efficiency

In Table 3, we present the time and participants in the
three different interviews. The human interviews lasted
around 35 minutes and required participation from both the
domain expert and the knowledge engineer, doubling the
resources needed. In contrast, the interview with ChatGPT
v4 was completed in approximately 10 minutes, requiring no
coordination, scheduling, or conversational overhead. The AI
responses also tended to be more structured and stayed on
topic without prompting.
Table 4 shows the time spend on transcription efforts.
While no significant difference in transcription quality was
observed between human and AI-based approaches, the
time saved using an automated system was substantial.

```
Table 4. Comparison of manual and AI-based transcription
methods
Method Time Required
Manual transcription 2–3 hours/session
AI transcription 10–15 minutes/session
```
```
This suggests that AI-assisted transcription tools offer
a substantially more time-efficient alternative to manual
transcription, with comparable accuracy based on subjective
evaluation.
```
### Metrics

```
One of the most striking observations is the size discrepancy
between the base truth ontology and the generated ontologies,
seen in Table 5. The base truth ontology contains a much
larger number of axioms, classes, and properties compared
to any of the generated ontologies. This difference was
expected, as the base truth ontology was constructed using
the D&D Player’s Handbook in its entirety, while the
generated ontologies relied solely on interview data. Given
the limited scope of the interviews - whether conducted with
AI or human experts — the knowledge captured in these
sessions was inevitably more constrained, leading to smaller
ontologies.
Another notable pattern is the higher number of axioms
in AI-interview-ontologies, particularly in human-built
ontologies. The structured nature of AI-generated interview
transcripts appears to have played a significant role in
this outcome. Unlike human experts, who may introduce
implicit knowledge, go off-topic, or provide information
in a less structured manner, AI-generated responses tend
to be more direct, systematic, and information dense.
This structured format allows human knowledge engineers
to extract and formalize more axioms, leading to richer
ontologies. In contrast, human interviews, while potentially
more nuanced, may contain less explicitly stated information,
making it more difficult to translate into structured ontology
components.
Furthermore, a difference between AI- and human-
generated ontologies is the notably lower number of
individuals (instances) in AI-generated ontologies. Across all
AI-generated ontologies, the number of individuals remained
consistently low, suggesting a fundamental limitation in
how AI approaches ontology generation. One possible
explanation is that AI models prioritize class structures over
individual instances, as they are trained primarily on patterns
of conceptual relationships rather than specific examples.
Furthermore, AI may struggle to infer when an entity should
be treated as a class versus an individual, leading to under-
representation of instances.
```

8 Transportation Research Record XX(X)

**Table 5.** Metrics of all ontologies
Ontology Axioms Logical
Axioms

```
Declaration
Axioms
```
```
Classes Object
Prop.
```
```
Data
Prop.
```
```
Individuals
```
#### BT 7583 5890 1693 165 50 28 1462

#### AI-AI 207 87 75 53 9 6 7

#### AI-H 624 293 266 196 15 4 51

#### H1-AI-AI 160 67 56 38 5 7 6

#### H1-AI-H 232 121 109 59 19 7 24

#### H1-H-AI 149 57 46 28 6 6 6

#### H1-H-H 190 97 93 61 7 5 20

#### H2-AI-AI 157 66 46 28 8 5 5

#### H2-AI-H 232 121 109 59 19 7 24

#### H2-H-AI 197 82 58 38 8 7 5

#### H2-H-H 260 132 126 49 8 4 65

### OQuaRE

In order to calculate the OQuaRE metrics of the various
ontologies, the oquare-metrics module|| was used. The
resulting CSV file can be found in the accompanying GitHub
repository (See Footnote ‡). When looking at the subsequent
results, most of the metrics were fairly similar. This is not
surprising as the structure of the various ontologies should
be very similar. However, a few metrics had interesting
differences, namely the following four metrics:

- structural
- redundancy
- controlledVocabulary
- guidanceAndDecisionTrees

These metrics will be explained, and their differences
inspected, in the coming paragraphs. Table 6 reports the
scores and metrics.
The Structural score, which combines metrics like
cohesion, consistency, formal relation support, formalization,
redundancy, and tangledness, evaluates the connections
within an ontology and the attributes of the graph. The results
show that AI-generated ontologies (AI-AI, H1-AI-AI, H2-
AI-AI) have slightly higher structural scores (4.166–4.5).
This suggests that AI-generated ontologies tend to be more
structured or possibly more consistent in their approach.
Human-generated ontologies (H1-H-H, H2-H-H, H1-AI-
H, H2-AI-H) show more variability (scores3.833–4); this ̃
difference suggests that human involvement might introduce
more variability or nuance into the structural design, which
can result in a slightly less rigid but potentially more
contextually rich structure.
Redundancyis part of the structural statistic; it shows how
often similar or overlapping relationships and definitions are
present within the ontologies. A high score would mean
that all knowledge items are informative. The AI-generated
ontologies tend to have higher redundancy (values of 3–5).
This suggests that AI systems may be more prone to creating
duplicate or overlapping definitions, potentially due to a lack

```
Table 6. OQuaRE Structural (S) and Redundancy (R) scores,
and constrolledVocabulary (cV), guidanceAndDecisionTrees
(gDT) metrics
Ontology S R cV gDT
BT 3.5 1 1 5
AI-AI 4.167 3 3 4.
AI-H 4.167 2 2 3
H1-AI-AI 4.167 3 3 5
H1-AI-H 3.83 1 1 5
H1-H-AI 4.5 5 5 5
H1-H-H 3.83 1 1 1
H2-AI-AI 4.33 5 5 5
H2-AI-H 3.83 1 1 5
H2-H-AI 4.5 5 5 5
H2-H-H 4 1 1 5
```
```
of nuanced distinction between concepts or properties. The
human-generated ontologies have lower redundancy (mostly
1). This suggests that human input might contribute to more
concise and unique definitions within the ontology.
ThecontrolledVocabularymetric measures the terminol-
ogy of the ontology; is it consistent and standardized, are
labels or alternative terms used? A high score on this met-
ric means that the concepts are consistently represented,
and ambiguity is reduced. AI-generated ontologies generally
score higher (3–5). A score of 3 indicates moderate use
of standardized terms but still includes some flexibility or
custom terms. This suggests that AI-generated ontologies
generally maintain consistency while allowing for some vari-
ation. A score of 5 suggests a strong adherence to controlled
vocabularies. Human-generated ontologies score much lower
(mostly 1, except AI-H at 2), which means a low adherence to
a predefined set of terms. This suggests that human influence
tends to introduce more flexibility, using terms that might
be better suited to specific contexts or domain nuances. This
```
```
∥https://github.com/tecnomod-um/oquare-metrics
```

van den Bent, Pernisch and Schlobach 9

aligns with expectations that AI would be more controlled,
and humans would be more flexible.
TheguidanceAndDecisionTreesmetric in OQuaRE eval-
uates how well an ontology supports decision-making and
structured guidance within its domain. High scores (closer
to 5) suggest well-structured ontologies where concepts and
relationships are clear, helping with reasoning and auto-
mated decision-making. Lower scores indicate less structured
ontologies, where relationships might be ambiguous or lack
the necessary connections to guide decision-making. Most
ontologies score 5, meaning they follow a strong decision-
making structure. However, two AI-led interview ontologies
(AI-AI: 4.5, AI-H: 3) are outliers. The reason for these
differences remains unclear, as no cause was found in the
OQuaRE metrics code. This could indicate anomalies in AI-
led interviews or differences in how responses were struc-
tured, but further investigation is out of scope.

### Content Comparison

In this part, we compare the content of the ontologies in more
detail. First, we evaluated the nine competency questions on
all ontologies but unfortunately, they could not be answered,
except by the base-truth ontology. Given that the interviews
were conducted in an open-ended manner but were not
guided by the competency questions themselves, this is not
a surprising outcome. It signals that if not specifically asked
for, the information was not mentioned in the interview and
hence could not be modelled. This also highlights, that one
interview only covers a fraction of the content. Hence, it is
important to look at the content more closely, first at the
hierarchy and then at the entities.

Hierarchy Comparison.As shown in Table 7, the number
of correct hierarchy relationships, defined as matching
parent-child class links and correct top-level classes relative
to the base truth ontology, varies across the different
ontology generation pipelines. Human-generated ontologies
consistently outperform their AI-generated counterparts,
with the H1-H-H ontology achieving the highest accuracy
(19 correct relations). This suggests that human experts
are currently more effective at capturing the intended
class structure of a domain, particularly in representing
hierarchical relationships that align with an established
reference ontology.
The results show that human-generated ontologies exhibit
the highest degree of alignment with the base truth hierarchy,
suggesting that human knowledge engineers remain more
skilled at modeling nuanced relationships between concepts.
Particularly, they tend to capture both top-level category
structures and more fine-grained subclass placements with
greater fidelity. This is most clearly seen in the H1-H-H
ontology, which contained the highest number of correct
hierarchical relationships (19).
In contrast, the AI-generated ontologies consistently
performed the worst in replicating the correct hierarchy.

```
Table 7. Amount of Parent-Child Relationships also found in the
Base Truth ontology.
Ontology subClassOf Total Percentage correct
AI-AI 8 53 15.094%
AI-H 15 196 7.653%
H1-AI-AI 4 38 10.526%
H1-AI-H 13 59 22.034%
H1-H-AI 4 28 14.286%
H1-H-H 19 61 31.147%
H2-AI-AI 3 28 10.714%
H2-AI-H 15 59 25.424%
H2-H-AI 4 38 10.526%
H2-H-H 7 49 14.286%
```
```
These pipelines often lacked the structural depth needed
to accurately mirror the base truth, and frequently
misrepresented the relationships between key domain
concepts. This suggests that, in their current form, LLMs
struggle to independently construct ontologies with precise
hierarchical relationships.
Across both AI- and human-generated ontologies, one of
the most pervasive issues was the confusion between classes
and instances. For example, entities such asFighteror
Wizardwere often incorrectly modeled as subclasses of
Class, when in fact they should be individuals (instances).
These kind of misclassifications hint at a deeper conceptual
challenge in modeling real-world categories, where the
distinction between types and examples of those types is not
always trivial, especially in a creative domain like fantasy
roleplaying. Another structural challenge arose in the use of
synonymous or near-synonymous terms. Several ontologies
included classes like Town vs.City or Countryvs.
Kingdom, which, while conceptually related, introduce
inconsistencies in naming that complicate alignment with a
shared reference ontology.
In addition, certain recurring missteps emerged across
multiple generation methods, most notably the omission
of intermediate or bridge classes such as InGameItem
betweenItemand its more specific children likeWeapon
and Armor. Such gaps suggest that some structural
patterns are systematically difficult to model, regardless of
whether the pipeline is AI-driven or human-led. Similarly,
high-level misclassifications, such as repeatedly placing
Monster as a subclass of Character rather than a
sibling, point to frequent breakdowns in understanding
the top-level organization of the domain. Despite these
issues, however, many ontologies still captured a rough
semantic understanding of the domain. Classes were often
misclassified, but their inclusion nonetheless reflected a basic
grasp of the core concepts.
```
```
Entities Comparison.The entity comparison focused on key
ontology classes, includingCharacter(with its subclasses
PlayerCharacter and NonPlayerCharacter
```

10 Transportation Research Record XX(X)

(NPC)), Item (with subclasses Armor and Weapon),
Class, andRace. We looked specifically at the parent
class, children classes, siblings classes, and any possible
instances. Specific individuals were not compared as
classes were, because they were too varied; furthermore, AI
ontologies often had only a few individuals.

Human-generated ontologies, on the other hand, some-
times includedRacebut with variations in the specific
instances used. In some cases, the races listed differed from
those in the Base Truth Ontology.

The representation of PlayerCharacter was
largely consistent across both AI- and human-generated
ontologies, suggesting that this concept is well-defined
and universally recognized within the domain. However,
NonPlayerCharacter showed significant variation,
with both AI- and human-generated ontologies introducing
vastly different subclasses. This lack of agreement indicates
that there is no clear consensus on how to categorize
different types of NPCs. One possible reason for this is that
NPCs serve diverse roles in games - such as merchants,
quest givers, and enemies - which can lead to different
classification approaches. Humans may categorize NPCs
based on their function or narrative role, whereas AI may
rely on statistical patterns from training data that do not align
with a structured classification system.

AI- and human-generated ontologies showed notable
differences in how they representedItem, Armor, and
Weapon. AI-generated ontologies often simplified or
entirely omitted these entities, either grouping them into
broader categories without explicit subclassing or failing to
distinguish between different types of equipment. This sug-
gests a tendency toward generalization rather than detailed
classification. In contrast, human-generated ontologies fre-
quently renamed or restructured these categories, introducing
variations that made direct comparisons more difficult. While
this reflects domain knowledge and subjective interpretation,
it also highlights inconsistencies in terminology. Addition-
ally, both AI and human ontologies occasionally lacked
explicit subclassing, meaning that hierarchical relationships
between these entities were not always well-defined. This
inconsistency suggests that while AI may oversimplify struc-
tures, human conceptualizations also vary, leading to chal-
lenges in achieving a standardized ontology.

The absence ofRacein all AI-generated ontologies and
the near absence ofClass(with only one AI ontology
including it) raises interesting questions about how AI
handles these concepts. One possible explanation for the
omission ofClassis that the term ’class’ itself is commonly
used in ontology development, which might cause confusion
for AI models when determining whether it refers to a game-
related entity or an ontological construct. This ambiguity
could make it more challenging for AI to categorize and
include Classcorrectly in the ontology structure. The
omission ofRaceis particularly noteworthy. Given that

```
Table 8. Amount of hallucinated classes in AI-generated
ontologies
Ontologies Hallucinated Total Percentage
AI-AI 10 53 19%
H1-H-AI 7 28 25%
H1-AI-AI 16 56 29%
H2-H-AI 16 58 28%
H2-AI-AI 9 28 32%
```
```
LLMs are often designed with fail-safes to avoid sensitive
topics, it is possible that the AI avoided includingRace
due to built-in content moderation mechanisms. In real-world
contexts, the concept ’race’ is a highly sensitive and socially
complex topic, which may have led the AI to err on the
side of exclusion rather than risk generating problematic
classifications. In contrast, human-generated ontologies did
includeRace, though with notable variations. This variation
can likely be attributed to the influence of homebrew
elements in D&D, where players frequently expand upon
the standard ruleset outlined in the Player’s Handbook. As
a result, the races listed in human-created ontologies were
not necessarily incorrect but reflected additional, customized
interpretations beyond the base truth ontology.
```
### Hallucinated data in AI ontologies

```
As seen in Table 8, the percentage of hallucinated
classes ranges from 32% (9 out of 28, for ontology
H2-AI-AI) to 18% (AI-AI), suggesting that AI-generated
ontologies consistently include a non-trivial amount of extra
information. Interestingly, some hallucinated data was still
factually correct within the context of D&D, but it was never
mentioned in the interviews. This suggests that the LLM drew
from prior knowledge rather than purely fabricating content.
This phenomenon has implications for trustworthiness: while
the hallucinated data is not necessarily wrong, it still
represents a deviation from the interview data, which could
impact the accuracy of the process.
```
### Discussion

```
Now that we have the results, we can examine their
significance. As a reminder, this research aims to answer the
following research question (RQ2):How does using a Large
Language Model for the process of Knowledge Elicitation
compare to using human knowledge engineers?
RQ2.1:Given the broad scope of RQ2, it has been divided
into two sub-questions, the first of which is:What is the
difference between using a Large Language Model and
human experts as a source to gather data?
To address this, we conducted interviews with both
an LLM (ChatGPT v4) and two human experts. The
time required for human interviews was about 35 minutes
per session, effectively doubling when accounting for the
```

van den Bent, Pernisch and Schlobach 11

presence of both the expert and the knowledge engineer.
In contrast, the interview with ChatGPT was completed
in approximately 10 minutes. Beyond efficiency, ChatGPT
v4 demonstrated advantages in maintaining structured
responses, integrating more data into its answers, and staying
on topic. In terms of both time efficiency and response
quality, the AI outperformed human experts in the elicitation
phase.
Additionally, we compared the transcription of human
interviews performed by humans versus AI. While no
significant difference in quality was observed, the AI-based
transcription was notably faster. This suggests that, for
scenarios where human interviews remain necessary, AI-
assisted transcription is a clear recommendation due to its
efficiency without compromising accuracy.

RQ2.2:The second subquestion is the following:What is
the difference between using a Large Language Model and
humans to create RDF ontologies from textual data?
Despite the advantages of LLMs in the elicitation
phase, the results consistently show that human knowledge
engineers produce higher-quality ontologies - especially in
terms of structural accuracy and richness. Human-created
ontologies were far more successful at modeling correct
hierarchical relationships and including relevant individuals.
The H1-H-H ontology achieved the highest alignment with
the base truth hierarchy, and other human-led constructions
also showed stronger conceptual fidelity. The AI-generated
ontologies, on the other hand, tended to be smaller,
more rigid, and often missed critical components such as
individuals or intermediate classes.
Perhaps the most promising result comes from the hybrid
pipelines that combine AI-driven interviews with human-led
ontology construction. These combinations often produced
ontologies that were richer than fully AI-generated ones
but benefited from the structured data of the AI interview.
This suggests that a division of labor may be the most
effective approach: let AI do what it does best (quick,
structured elicitation), and let humans handle what they excel
at (interpretation, abstraction, and nuanced structuring).
Another notable observation was the consistent presence
of hallucinated content in AI-generated ontologies. Between
19% and 32% of the classes in these ontologies were
hallucinated, meaning they were not mentioned in the
interview data. Some of this content was factually accurate
within the D&D domain, suggesting that the LLM pulled
from background knowledge rather than fabricating entirely.
Nonetheless, these additions fall outside the scope of the
interview and raise trust and validation concerns.
The findings point to a clear conclusion: current LLMs
are highly useful in speeding up and structuring the early
stages of knowledge elicitation, but they are not yet
reliable enough to replace humans in ontology generation.
Human knowledge engineers remain essential for producing
accurate, semantically rich ontologies that align with domain

```
expectations. However, AI is not without value in this
space. It brings speed, standardization, and scalability to the
elicitation process and can serve as a powerful collaborator
when its outputs are validated and curated by human experts.
In future pipelines, a well-designed hybrid system may yield
the best results: one that leverages AI for initial data gathering
and human experts for final modeling.
```
### Limitations and Future Work

```
While this research provides valuable insights into the use
of LLMs and human experts for Knowledge Elicitation
and ontology development, several limitations should be
acknowledged. These limitations not only inform the
interpretation of the results but also highlight opportunities
for improvement and further exploration in future work.
Generalizability of the findings is limited due to several
aspects. One of these is the number of interviews, people and
LLMs involved, conducted and the second is the exploration
of one domain. This research was conducted using ChatGPT
v4, which, at the time of the interviews, represented the
state-of-the-art in LLMs. However, the field of generative
AI is developing rapidly. Since then, newer versions such as
ChatGPT v4o and ChatGPT v4.5 have been released, offering
potential improvements in reasoning, response quality, and
efficiency. It is expected that even more advanced models will
become available in the near future. These newer models may
yield different results or enable more effective Knowledge
Elicitation processes. Furthermore, this research focused
exclusively on one proprietary model. Future research could
expand the scope by exploring models from other providers,
as well as open-source alternatives, to assess whether similar
outcomes can be achieved across different platforms and
architectures.
The domain selected for this research was intentionally
chosen to be well-represented in publicly available sources,
ensuring that both human experts and LLMs could draw
on a wide range of accessible information. This made it
possible to explore the potential of AI-assisted Knowledge
Elicitation under relatively favorable conditions, where
the language model likely had substantial prior exposure
during training. However, in many real-world applications,
Knowledge Elicitation takes place in more specialized or
niche domains, where information is less prevalent online and
expert knowledge is harder to access. Future research could
explore how LLMs perform in such contexts, particularly
when compared to human domain experts. Key questions
include whether AI-generated interviews remain effective in
domains with sparse training data, whether the quality of the
elicited knowledge deteriorates, and whether human experts
outperform AI under these more challenging conditions.
During the ontology creation phase, it became apparent
that using LLMs directly introduced a number of challenges.
One major issue was the LLMs tendency to hallucinate data:
generating classes or relationships that were not grounded
```

12 Transportation Research Record XX(X)

in the provided input. Additionally, the LLM often produced
inconsistent results: identical prompts could lead to differing
ontological structures across runs, making it difficult to
ensure reproducibility and reliability. Another limitation
was its inability to fully carry over all the concepts it
identified during parsing. While the LLM might correctly
list relevant classes and subclasses during initial analysis,
many of these would fail to appear in the final ontology,
resulting in unexpectedly small and incomplete outputs. Due
to these shortcomings, the decision was made to manually
construct the ontologies using the LLM’s suggestions as
a starting point. This ensured that all identified elements
were accurately captured, albeit through a more labour-
intensive process. That said, it is worth noting that newer
versions of LLMs, such as ChatGPT v4o or other models,
may offer improved consistency and better support for
ontology generation. Future work could explore whether
these advancements address the limitations encountered in
this study.
An interesting direction for future research lies in the
potential integration or combination of these ontologies.
Merging the strengths of different ontologies—each captur-
ing distinct perspectives or structural nuances—may result
in a more comprehensive and accurate ontology that better
approximates the quality of the base truth ontology. Although
this idea presents a promising opportunity for enhancing
ontology quality, it remained outside the scope of the current
research. Future work could investigate methods for com-
bining ontologies and systematically evaluating the resulting
merged ontology in comparison to the base truth ontology.

### Conclusions

This research set out to explore the use of LLMs
in the process of Knowledge Elicitation and compare
their performance with that of traditional human domain
experts and human knowledge engineers. By designing and
evaluating a pipeline that incorporated different combinations
of human and AI involvement, ranging from fully human
to fully AI, the research aimed to assess both the efficiency
and quality of each approach, particularly in the context of
ontology creation.
The results show that LLMs offer significant advantages in
the data collection phase. AI-led interviews were faster, more
structured, and more information-dense than those conducted
with human experts. This makes LLMs highly suitable for
the initial stages of knowledge elicitation, especially in
well-documented domains. However, these advantages did
not translate directly into ontology generation. Ontologies
created solely by AI lacked detail, contained hallucinated
or inconsistent content, and struggled with basic modelling
distinctions, such as those between classes and instances.
In contrast, human knowledge engineers outperformed AI
in building richer, and more accurate ontologies. They were
better at preserving conceptual nuance, correctly modelling

```
hierarchical relationships, and ensuring alignment with a
reference ontology. Hybrid approaches, where AI conducted
the interview and a human built the ontology, emerged as the
most promising solution, combining the speed and structure
of AI with the precision and contextual understanding of
human modellers. This approach reduces time and labour
while maintaining the quality and depth of human-led
ontology development.
As LLMs continue to evolve, future research may find that
many of the current limitations are overcome, opening up
new possibilities for automating even more of the knowledge
elicitation process. This study provides a foundation for such
future work and highlights the need for continued exploration
into the balance between automation and expert oversight
in building reliable, trustworthy knowledge systems. In the
end, the most effective knowledge elicitation may not come
from choosing between, but from collaboration with AI and
humans.
```
```
References
```
1. Polanyi M. The Tacit Dimension; 1966.
2. Brown TB, Mann B, Ryder N, Subbiah M, Kaplan J, Dhariwal
    P, et al.. Language Models are Few-Shot Learners. arXiv; 2020.
    ArXiv: 2005.14165 [cs]. Available from:http://arxiv.
    org/abs/2005.14165.
3. Marcus G. The Next Decade in AI: Four Steps Towards Robust
    Artificial Intelligence. arXiv; 2020. ArXiv:2002.06177. Avail-
    able from:http://arxiv.org/abs/2002.06177.
4. Lavrac N, Mozetic I. Methods for knowledge acquisition and
    refinement in second generation expert systems. SIGART Bull.
    1989 Apr;(108):63-9. Available from:https://dl.acm.
    org/doi/10.1145/63266.63274.
5. Solomon P. The think aloud method: A practical guide
    to modelling cognitive processes. Information Processing
    & Management. 1995 Nov;31(6):906-7. Available from:
    https://linkinghub.elsevier.com/retrieve/
    pii/0306457395900314.
6. Cooke NJ. Varieties of knowledge elicitation techniques.
    International Journal of Human-Computer Studies.
    1994 Dec;41(6):801-49. Available from: https:
    //www.sciencedirect.com/science/article/
    pii/S1071581984710834.
7. Sillitoe P. The Development of Indigenous Knowledge : A
    New Applied Anthropology1|Current Anthropology: Vol 39,
    No 2; 1998. Available from:https://www.journals.
    uchicago.edu/doi/abs/10.1086/204722.
8. Davenport T. Working Knowledge: How Organizations
    Manage What They Know. Estudios de la Gestion. 2024 ́
    Jun;(15):213-5. Publisher: Universidad Andina Sim ́on
    Bol ́ıvar: Sede Ecuador. Available from:http://scielo.
    senescyt.gob.ec/scielo.php?script=sci_
    abstract&pid=S2661-65132024000100213&lng=
    es&nrm=iso&tlng=en.


```
13
```
9. Hoffman RR, Crandall B, Shadbolt N. Use of the Critical
    Decision Method to Elicit Expert Knowledge: A Case Study
    in the Methodology of Cognitive Task Analysis. Human
    Factors. 1998 Jun;40(2):254-76. Publisher: SAGE Publications
    Inc. Available from: https://doi.org/10.1518/
    001872098779480442.
10. Wondimu NA, Buche C, Visser U. Interactive Machine
Learning: A State of the Art Review. arXiv; 2022.
ArXiv:2207.06196. Available from:http://arxiv.org/
abs/2207.06196.
11. Dzyuba V, Van Leeuwen M, Nijssen S, De Raedt L.
Active preference learning for ranking patterns. In:
2013 IEEE 25th International Conference on Tools with
Artificial Intelligence. IEEE; 2013. p. 532-9. Available
from: https://ieeexplore.ieee.org/abstract/
document/6735296/.
12. Amershi S, Fogarty J, Weld D. Regroup: interactive machine
learning for on-demand group creation in social networks.
Proceedings of the SIGCHI Conference on Human Factors in
Computing Systems. 2012 May:21-30. Conference Name: CHI
’12: CHI Conference on Human Factors in Computing Systems
ISBN: 9781450310154 Place: Austin Texas USA Publisher:
ACM. Available from:https://dl.acm.org/doi/10.
1145/2207676.2207680.
13. Weizenbaum J. ELIZA—a computer program for the study
of natural language communication between man and machine.
Communications of the ACM. 1966 Jan;9(1):36-45. Available
from:https://dl.acm.org/doi/10.1145/365153.
365168.
14. Rosenfeld R. Two decades of statistical language modeling:
where do we go from here?|IEEE Journals & Magazine|IEEE
Xplore; 2004. Available from:https://ieeexplore.
ieee.org/abstract/document/880083.
15. Brown PF, Della Pietra VJ, deSouza PV, Lai JC, Mercer
RL. Class-Based n-gram Models of Natural Language.
Computational Linguistics. 1992;18(4):467-80. Available
from:https://aclanthology.org/J92-4003/.
16. Brown PF, Cocke J, Della Pietra SA, Della Pietra VJ, Jelinek
F, Lafferty JD, et al. A Statistical Approach to Machine
Translation. Computational Linguistics. 1990;16(2):79-
17. Available from:https://aclanthology.org/
J90-2002/.
18. Kim Y. Convolutional Neural Networks for Sentence Classifi-
cation. arXiv; 2014. ArXiv:1408.5882 [cs]. Available from:
[http://arxiv.org/abs/1408.5882.](http://arxiv.org/abs/1408.5882.)
19. Vaswani A, Shazeer N, Parmar N, Uszkoreit J, Jones L, Gomez
AN, et al. Attention is All you Need. 2017.
20. Radford A, Narasimhan K, Salimans T, Sutskever I. Improving
Language Understanding by Generative Pre-Training. 2018.
21. Devlin J, Chang MW, Lee K, Toutanova K. BERT: Pre-
training of Deep Bidirectional Transformers for Language
Understanding. 2019.
22. Huang Y, Sun L, Wang H, Wu S, Zhang Q, Li Y, et al..
TrustLLM: Trustworthiness in Large Language Models. arXiv;
23. ArXiv:2401.05561 [cs]. Available from:http://
arxiv.org/abs/2401.05561.
24. Saeedizade MJ, Blomqvist E. Navigating Ontology Develop-
ment with Large Language Models. In: Mero ̃no Penuela A, ̃
Dimou A, Troncy R, Hartig O, Acosta M, Alam M, et al.,
editors. The Semantic Web. vol. 14664. Cham: Springer Nature
Switzerland; 2024. p. 143-61. Series Title: Lecture Notes
in Computer Science. Available from:https://link.
springer.com/10.1007/978-3-031-60626-7_8.
25. Radford A, Kim JW, Xu T, Brockman G, McLeavey C,
Sutskever I. Robust Speech Recognition via Large-Scale Weak
Supervision. arXiv; 2022. ArXiv:2212.04356 [eess]. Available
from:http://arxiv.org/abs/2212.04356.
26. Ryan GW, Bernard HR. Techniques to Identify Themes.
Field Methods. 2003 Feb;15(1):85-109. Publisher: SAGE
Publications Inc. Available from:https://doi.org/10.
1177/1525822X02239569.
27. MILITELLO LG, HUTTON RJB. Applied cognitive
task analysis (ACTA): a practitioner’s toolkit for under-
standing cognitive task demands. Ergonomics. 1998
Nov;41(11):1618-41. Publisher: Taylor & Francis eprint:
https://doi.org/10.1080/001401398186108. Available from:
https://doi.org/10.1080/001401398186108.
28. Guarino N, Welty C. Evaluating ontological decisions with
OntoClean. Communications of the ACM. 2002 Feb;45(2):61-
29. Available from:https://dl.acm.org/doi/10.
1145/503124.503150.
30. Duque-Ramos A. OQuaRE: A SQuaRE-based approach
for evaluating the quality of ontologies | Journal of
Research and Practice in IT; 2011. Available from:
https://search.informit.org/doi/abs/10.
3316/ielapa.265844843145749.

# Appendices

### Hierarchy Comparison Details

```
AI-AI:ClassMonstershould be a sibling ofCreature,
rather than a subclass, though Creature is correctly
modelled as a sibling ofCharacter.CombatAction,
which is related to Action, should be a subclass of
CharacterAction, which would then be a subclass of
Action, rather than being directly related toAction.
Similarly,Talkis appropriately related toAction, but
it should be a subclass ofSocialInteraction, which
in turn should be a subclass ofCharacterAction, and
finally a subclass ofAction. Currently,Talkis incorrectly
positioned underInteractionActionin the hierarchy.
AI-H:Between the parent classItemand the subclasses
Weapon, Armor, and AdventuringGear, the class
InGameItemshould be included, as it is currently missing
in these relationships. Additionally, Monster should
```

14 Transportation Research Record XX(X)

be a sibling ofCharacter rather than a subclass of
NonPlayerCharacter, which in turn is a subclass
of Character. The subclasses of Background
(such as Criminal, Noble, and Soldier) should
be modeled as individuals of the Background class,
rather than as subclasses. Similarly, the subclasses
of Class (including Barbarian, Bard, Cleric,
Druid, Fighter,Monk,Paladin,Ranger, Rogue,
Sorcerer, Warlock, Wizard) and the subclasses of
Race (such as Dragonborn, Dwarf, Elf, Gnome,
Halfelf, Halforc,Halfling,Human, Tiefling)
should all be individuals of their respective classes, rather
than subclasses. Lastly, the classDialogueappears to
be similar to theTalkclass in the base truth ontology. In
this case, the parent class ofDialogue(Roleplaying)
is superfluous, andDialogueshould be a direct child
ofSocialInteraction, which is the parent class of
Roleplayingin the AI-H ontology.

H1-AI-AI:The subclasses ofPlayerCharacterin this
ontology should instead be modelled as individuals of the
Classcategory. In the base truth ontology, these entities
are notPlayerCharactersbut rather distinct instances
ofClass.

H1-AI-H:The class CharacterDetailsappears in
place ofCharacterStatistics. Additionally, although
the classes AbilityModifier, AbilityScore,
Background,Class, andRacedo not have the correct
parent class, they are correctly positioned as siblings,
maintaining their intended hierarchical relationships.
The class FantasySetting also closely aligns with
MedievalFantasySetting, which is included in the
base truth ontology.

H1-H-AI:The Class class includes Fighter and
Wizardas subclasses, whereas in the base truth ontology,
these are modelled as individuals (instances) of theClass
class. Additionally,CharacterhasDungeonMasteras
a subclass, which is incorrect;DungeonMastershould
instead be a subclass of Person. However, the class
Person is absent from this ontology, preventing the
correct hierarchical placement. Another notable discrepancy
is the classification of Monster, which appears as a
subclass ofNonPlayerCharacter. In the base truth
ontology,Monster is a sibling ofCharacter, not a
subclass. Furthermore,Characteritself is missing from
this ontology, though it should serve as the parent class of
NonPlayerCharacter.

H1-H-H:In the base truth ontology,Monsteris defined
as a sibling ofCharacter, whereas in H1-H-H, it is incor-
rectly modeled as a subclass. The classFantasySetting
is not included in the base truth ontology, but it closely aligns
withMedievalFantasySetting, which is included in
the base truth ontology. A key structural difference was
found in the classification of character attributes: theClass

```
class in H1-H-H includesCleric,Fighter,Paladin,
Sorcerer,Warlock, andWizardas subclasses, whereas
in the base truth ontology, these are modeled as individuals
(instances) of theClassclass. Similarly,DwarfandElf
appear as subclasses ofRacein H1-H-H, whereas in the base
truth ontology, they are individuals within theRaceclass.
H2-AI-AI:ClassDungeonMastershould be classified
as a Personrather than a Character. Additionally,
Creature is appropriately positioned as a sibling of
Character, butCreatureandMonstershould also be
siblings, not a parent class and subclass. Furthermore, in the
hierarchy between the parent classItemand the subclass
Weapon, the classInGameItemshould be included, which
also applies to the relationship betweenItemandArmor.
Lastly, the classTownclosely resembles the classCityin
the base truth ontology, and could be seen as synonymous.
H2-AI-H:The class CharacterStatistic is
incorrectly modeled as a subclass ofCharacterTrait,
whereas CharacterTrait should simply be
CharacterStatistic. Additionally, in the hierarchy
between the parent classItemand the subclassWeapon,
the classInGameItemshould be included, as it is missing
from the current structure.
H2-H-AI:The classes Character, Creature, and
Monster should be siblings in the hierarchy; however,
Monster is incorrectly modeled as a subclass of
Creature, which in turn is a subclass ofCharacter.
Additionally, in the hierarchy between the parent classItem
and the subclassWeapon, the classInGameItemshould
be included, which also applies to the relationship between
ItemandArmor.
H2-H-H:The class Creatureis incorrectly modeled
as a subclass of Character, whereas it should be
a sibling. Similarly, Enemy is structured as a direct
subclass ofCharacter, while in the base truth ontology,
it should be a subclass of NonPlayerCharacter,
which itself is a subclass of Character. Additionally,
Monster is incorrectly positioned as a subclass of
NonPlayerCharacter, whereas it should be a sibling of
Character. Lastly, the classCountryclosely resembles
Kingdomin the base truth ontology, suggesting a conceptual
overlap between the two.
```

[[RAW FILES]]