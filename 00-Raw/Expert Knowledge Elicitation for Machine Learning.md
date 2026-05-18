

Insights from a Survey and Industrial Case Study

**PAPER WITHIN** Computer Science
**AUTHORS:** Oskar Persson, Samuel Svensson
**JÖNKÖPING** August 2023


This exam work has been carried out at the School of Engineering in Jönköping in the subject area Com-
puter Science. The work is a part of the two-year Master of Science in Artificial Intelligence programme.
The authors take full responsibility for opinions, conclusions and findings presented.
Examiner: Vladimir Tarasov
Supervisor: Maria Riveiro
Scope: 30 credits
Date: 2023-08-

Mailing address: Visiting address: Phone:
Box 1026 Gjuterigatan 5 036-10 10 00 (vx)
551 11 Jönköping


#### EXPERT KNOWLEDGE ELICITATION I

## Acknowledgements

We want to express our sincere gratitude to all those who have contributed to the successful completion
of this thesis.

First and foremost, we would like to thank our supervisor, Maria Riveiro, for providing us with valuable
guidance, support, and feedback throughout the course of this thesis. Your insightful comments and
suggestions have been crucial in shaping this thesis.

A big thank you to Max Pettersson and Marcus Gullstrand, who have taken the time to discuss this
problem with us whenever we needed it.

We are also grateful to the coordinators and supervisors at Saab AB, Training and Simulation, who gen-
erously shared their time and insights with us and enabled this research.


#### EXPERT KNOWLEDGE ELICITATION II

```
Abstract
While machine learning has shown success in many fields, it can be challenging when there are lim-
itations with insufficient training data. By incorporating knowledge into the machine learning pipeline,
one can overcome such limitations. Therefore, eliciting expert knowledge can play an important role
in the machine learning project pipeline.
Expert knowledge can come in many forms, and it is seldom easy to elicit and formalize it in a way
that is easily implementable into a machine learning project. While it has been done, not much focus
has been on how. Furthermore, the motivations for why knowledge was elicited in a particular way
as well as the challenges that may exist with the elicitation, are not always focused on either. Making
educated decisions for knowledge elicitation can therefore be challenging for researchers. Hence, this
work aims to explore and categorize how expert knowledge elicitation has been done by researchers
previously. This was done by developing a taxonomy that was then used for analyzing articles.
A total of 43 articles were found, containing 97 elicitation paths that were categorized in order to
identify trends and common approaches. The findings from our study were used to provide guidance
for an industrial case in its initial stage to show how the taxonomy presented in this work can be applied
in a real-world scenario.
```
```
Keywords:knowledge elicitation; machine learning; expert knowledge; informed machine learn-
ing; hybrid machine learning; survey; taxonomy.
```

## EXPERT KNOWLEDGE ELICITATION III

- 1 Introduction Contents
   - 1.1 Industrial case
   - 1.2 Purpose and research questions
   - 1.3 Scope and delimitations
   - 1.4 Disposition
- 2 Background
   - 2.1 Informed Machine Learning
   - 2.2 Knowledge elicitation
- 3 Related work
   - 3.1 Decisions making
   - 3.2 Expert knowledge
- 4 Methodology
   - 4.1 Search strategy and selection
   - 4.2 Content analysis
- 5 Elicitation taxonomy
   - 5.1 Machine learning pipeline
   - 5.2 Elicitation medium
   - 5.3 Knowledge target
   - 5.4 Knowledge representation
   - 5.5 Motivations and challenges
- 6 Survey Results
   - 6.1 Problem specification
   - 6.2 Feature engineering
   - 6.3 Model structure
   - 6.4 Model training
   - 6.5 Model evaluation
   - 6.6 Motivations
   - 6.7 Challenges
- 7 Discussion
   - 7.1 Results discussion
   - 7.2 Method discussion
- 8 Application to the industrial case
- 9 Conclusions and future work


## 1 Introduction

When technical equipment malfunctions, human experts are responsible for determining what happened
and the steps to repair it. While this is a valid strategy, it could become more cost-efficient, faster, and
more effective if an Artificial Intelligence (AI) model could do it instead. However, that might not always
be possible, so an initial step would be to give the experts currently making these assessments AI support
in their decision-making process. Nevertheless, for that to work, these models must be accurate and
trustworthy.

The idea of moving the decision-making to a computer has existed since at least the 1960s [1]. AI and
Machine Learning (ML) have seen many advances over the last years, ranging over many areas such as
speech and image recognition [2], [3] as well as self-driving vehicles. However, even if it has shown great
success, ML still has limits when there is insufficient training data [4], something that is especially true
within new technologies [5].

To achieve human-level or superior performance on a given task, AI models require vast amounts of data
for training. However, this training process restricts the AI’s capabilities compared to humans, who can
naturally transfer knowledge between tasks by selecting suitable sources of knowledge that can be applied
to new tasks [6]. Furthermore, even if the data is available, it is not necessarily the most effective learning
process. While there have been advancements in multiple areas, the success usually relies on having large
amounts of data to train on [7], [8]. The solution is not always having sufficient data but being able to use
the data meaningfully. For example, the amount of data created until the year 2012 was 2.72 zettabytes
(10^21 bytes), with a prediction that it would double every two years [9]. That shows how rapidly and to
what extent data is collected today.

Nevertheless, it says nothing about the quality of the data itself, something which is a precondition for
successfully analyzing and using it [10], [11]. Furthermore, pure data-driven approaches can only predict
what is in the dataset, i.e., decisions taken and recorded outcomes. That is why, although significant vol-
umes of data may be available, machine learning methods solely based on data may not provide accurate
predictions or the insights necessary for improved decision-making [11].

Therefore, if the goal is to have effective learning processes, the aim should be to use valuable data and
the knowledge available in the problem space instead of only exploiting the available training samples.
Furthermore, such approaches allow for already-known knowledge to be included in the ML pipeline to
potentially achieve a more effective learning process. Another important aspect is that purely data-driven
approaches are not clearly related to already proven and validated knowledge or given security guidelines,
which are vital aspects in trustworthy AI [4], [12].

The idea of incorporating knowledge into the ML pipeline has resulted in what is known as Informed Ma-
chine Learning (IML) [4]. There have been multiple studies in the domain of informed machine learning.
However, most studies have been around integrating well-formalized knowledge sources [4]. One key
aspect of this is that the more formalized knowledge is, the easier it is to implement in the ML pipeline.
When considering the degree offormalizationof knowledge, there are mainly three criteria to consider.
Firstly, if the knowledge is in writing; secondly, how structured the writing is; and lastly, how formal the
language is, see Section 2 for additional information. However, this leaves expert knowledge a bit on the
side where most of the research in this domain has been about human feedback and probabilistic relations
[4]. Furthermore, as Bauckhage, Ojeda, Schücker,et al.[8] points out, one of the major problems with
integrating expert knowledge is how to gather and formalize the knowledge systematically.

It is necessary to make particular distinctions when discussing knowledge. Making a definition of knowl-
edge is arguably difficult. Vonrueden, Mayer, Beckh,et al.[4] summarised knowledge as useful infor-
mation that is somehow validated. Expert knowledge, using the terminology from Vonrueden, Mayer,
Beckh,et al.[4] refers to knowledge such as intuition or implicit knowledge. This is the knowledge that
specific individuals or teams gain through experience in the domain. This knowledge can differ between
teams or personnel. This knowledge is harder to use partly because it needs to be better formalized, and
maybe it is impossible to formalize.


The process of gathering knowledge from domain experts is called elicitation. However, this process
varies a lot across the literature. Expert knowledge can enter the ML pipeline in many ways. Further-
more, conducting the expert knowledge elicitation in such a way that elicited knowledge is useful can be
challenging [13]. Because of the multiple knowledge targets and methods, it is not always clear what is
the best way forward. Therefore, this study aims to investigate the process of eliciting and representing
expert domain knowledge in a manner that enables its utilization in an ML pipeline first, from a the-
oretical perspective. Thus, this report reviews current approaches for eliciting and representing expert
domain knowledge. The study examines and analyzes these approaches and presents a taxonomy to aid
the elicitation process and its integration into an ML pipeline. Secondly, to provide a context from a prac-
tical perspective, we provide suggestions and a discussion, based on our study, on how expert knowledge
elicitation can be applied to an industrial case.

### 1.1 Industrial case

The industrial case examined in this research centers around the elicitation of expert knowledge regarding
equipment repairs from Saab AB, Training and Simulation, with the ultimate goal of being able to further
improve the decision-making process when repairing equipment in the field.

Saab AB, Training and Simulation in Huskvarna provided the initial motivation for this project and a
practical case to study the research questions. Saab AB started in 1937 with the primary goal of providing
military aircraft for Sweden. Today Saab AB provides world-leading products for both civil and military
security. One of their main focuses is developing simulation applications to help train military and defense
personnel in a safe and controlled environment. This includes simulating large-scale combat scenarios
with various vehicles and ground personnel and providing target practice for training purposes. Training
and simulations have facilities worldwide, with central training sites in Sweden, the Czech Republic, the
UK, and the USA. Huskvarna, Sweden, houses the main office where most development occurs. Some
training sites have teams in charge of the maintenance and the reparation of equipment.

Saab AB, Training and Simulation aims to gain insight into how expert knowledge, primarily found in
maintenance personnel, can be elicited and incorporated into an ML pipeline to facilitate even more
informed repair decisions. However, the case is in its initial stage, and therefore the data requirements are
unclear for informed decisions. Moreover, while the products across sites are similar, their exposure to
environmental factors may differ due to geographic location and usage scenarios, potentially leading to
different understandings and views on what causes a problem and what actions are needed to fix a system
among different groups of domain experts. The nature of the case makes it ideal for studying from an ML
project pipeline perspective.

### 1.2 Purpose and research questions

The process of eliciting knowledge in specific scenarios may not always be straightforward, and multiple
approaches may be available. Our study aims to explore different methods of incorporating expert knowl-
edge into an ML pipeline. We will investigate these methods and examine their associated motivations
and challenges.

We collaborated with Saab AB, Training and Simulation to conduct this research and provide valuable
insights into knowledge elicitation. This leads to our research questions:

RQ1How do machine learning researchers elicit knowledge from domain experts, and how is that knowl-
edge structured and formalized?

RQ2What are the challenges and motivations for eliciting and integrating expert knowledge into the
machine learning pipeline?

We used articles [11], [14]–[54] for this research. We aim to help researchers and practitioners better
understand these methods.


### 1.3 Scope and delimitations

This research reviews elicitation methods using the elicited knowledge in an ML pipeline. Specifically,
the focus of this work is expert knowledge. Therefore, a delimitation is that other types of knowledge,
such asworld knowledgeorscientific knowledge, are not considered.

### 1.4 Disposition

The remainder of the report is structured as follows:
In theBackgroundsection, relevant concepts that are a prerequisite for this report are presented, such as
Informed Machine Learning and the different types of knowledge as well as an introduction to knowledge
elicitation.
In theRelated worksection, we summarize closely related works and discuss them in light of our work.
TheMethodologysection describes how the survey articles were collected and what information was
coded in the articles. We also refer to literature reviews as a research method.
TheElicitation taxonomysection presents the taxonomy generated by this research, such as how the
ML pipeline can be viewed, different ways that knowledge elicitation can be conducted along with how
challenges and motivations for knowledge elicitation were formalized in this setting. This is the first part
of the results of this research.
The categorized articles are presented and visualized regarding the taxonomy in theSurvey Results
section, which is the second part of the results. Elicitation mediums, knowledge representation, and the
knowledge target are all presented for every part of the ML pipeline. The formalized challenges and
motivations are also presented. This is what, in total, answers the research question of this study.
Then theDiscussionsection discusses the method used in this research and the results that have emerged.
TheApplication to the industrial casesection is where we apply the knowledge gathered from this
research and apply it to the practical industry case.
Finally, in theConclusions and future worksection, we highlight the major results, followed by different
suggestions for future work.

## 2 Background

As our work spans both IML and expert knowledge elicitation, this section aims to provide a basic un-
derstanding of these research domains.

### 2.1 Informed Machine Learning

ML is the task of making a computer learn through experience, which comes in the form of data. While
there are numerous different ML algorithms [55], a typical ML problem consists of quantitativefeatures,
which a model trains on to predict differentlabels. IML, on the other hand, is the term used by Vonrueden,
Mayer, Beckh,et al.[4] to describe machine learning which includes knowledge in the ML pipeline. This
differs from ML by incorporating qualitative data into the pipeline. Knowledge is arguably tricky to define
but can be summarised as useful information that is in some way validated. Furthermore, Vonrueden,
Mayer, Beckh,et al.[4] proposes a taxonomy of three dimensions connected to knowledge: knowledge
source, representation, and integration. These three dimensions are illustrated in Figure 1. Additional
details on these three dimensions are provided below.

### Knowledge source. Knowledge can come from many sources; Vonrueden, Mayer, Beckh,et al.[4]

uses three source categories to classify the knowledge source. There are a few differences between the
knowledge sources of key importance. The most prominent one is the degree of formalization of the
knowledge. When considering formalization, there are mainly three factors that are taken into account.
Firstly if the knowledge is in writing; secondly, how structured the writing is; and lastly, how formal
the language is i.e., if it is equations or language. Furthermore, it must consider how the knowledge is
validated and if it comes from a domain or a specific group of people.


```
Knowledge
Representation
```
```
Algebraic Equations
Differential Equations
Simulation Results
Spatial Invariances
Logic Rules
Knowledge Graphs
Probabilistic Relations
Human Feedback
```
```
Knowledge
Source
```
```
Scientific Knowledge
World Knowledge
Expert Knowledge
```
```
Knowledge
Integration
```
```
Training Data
Hypothesis Set
Learning Algorithm
Final Hypothesis
```
Figure 1.Visualisation of the taxonomy from Vonrueden, Mayer, Beckh,et al.[4].

Scientific knowledge. This knowledge is often well-formalized and validated through scientific meth-
ods. Among these are the laws of physics and mathematical rules. This knowledge can be used in various
ways, such as enforcing that our model’s output aligns with the already proven and validated laws of
nature [12].

World knowledge. This knowledge can be more or less formalized and consists of general knowledge
and facts from everyday life. It often describes relations, concepts, and objects appearing in the world, and
the domain consists of language, syntax, and grammar. This knowledge is often not validated as strictly
as scientific knowledge but can instead be validated through logical reasoning or intuition. Vonrueden,
Mayer, Beckh,et al.[4] does not have a definition of intuition; therefore, in this report, we defineintuition
as the ability to understand something instinctively without needing conscious reasoning.

Expert Knowledge. This knowledge can be found within groups of experts. However, in these groups,
this knowledge can be considered general knowledge. Furthermore, this knowledge is often not well
formalized and therefore needs to be formalized, i.e., collected and structured. Furthermore, such knowl-
edge can come from many years in the field and can be intuitive. For example, an engineer working with
engines can use the sound of an engine to determine how the engine is running. As stated before, the more
formalized knowledge is, the easier it is to implement it. This leaves this knowledge arguably harder to
implement in an ML process than a well-formalized knowledge source such as scientific knowledge.

### Knowledge representation. This category refers to how the knowledge is formally represented

in the IML pipeline. Knowledge can be represented in many forms. Vonrueden, Mayer, Beckh,et al.
[4] suggests classes of representation which can be seen in Figure 1. Most of these representations of
knowledge can be combined with any source classes and integration classes; however, due to the nature
of the knowledge, i.e., formalization, etc., some combinations will be more prominent than others.

Algebraic Equations. Such equations represent knowledge in the form of equality or inequality be-
tween mathematical expressions, i.e., constants and variables. Notable examples are using kinematic

laws such as the displacement of an object (x) at a given timet,x(t) =x 0 +v 0 t+at

```
2
2.
```
Differential Equations. These equations also describe relationships between equations but more so
the relationships between the temporal or spatial derivatives. Continuing on the track of Newtonian

mechanics, one notable example is Newton’s second lawF=md

(^2) x
dt^2. WhereFis the net force,mis the
mass of the object,xis its position, andtis the time.


Simulations results. This knowledge comes from simulation results of numerical outcomes in real
scenarios. This may be seen as the same as equations, although Vonrueden, Mayer, Beckh,et al.[4]
separates them in that equations are compact numerical mathematical models, while simulation results
are only numerical results of such. Examples of this are simulated pictures of traffic scenarios.

Spatial Invariances. This knowledge describes properties that do not change under transformations,
such as rotations and translations. If an object shows invariance in those kinds of transformations, e.g.,
a symmetrical triangle is the same when it is turned 120°, or an object that looks the same as seen from
two opposite sides.

Logical Rules. This maps facts and dependencies and thereby provides the possibility to translate nat-
ural language into formalized logical rules such asA =⇒Bor other logical notations(∧,∨,...)This
allows us to write rules such as ifAandBthenC.

Knowledge Graphs. Formally, a graph consists of vertices and edgesG(V,E). Knowledge graphs
normally describe objects or concepts, whereas the edges describe relations between such. Graphs can be
directed, meaning that relations can be in either one or both directions and weighted, meaning that edges
with the same concepts could have different magnitudes. In Figure 2, examples of graphs are shown.

#### A

#### B C D

#### E

#### F

#### 2

#### 2 2

#### 4 3

#### 3

#### 7

#### 4

```
Dog Cat
```
```
Animal
```
```
is is
```
Figure 2.Examples of graphs. The graph to the left is a weighted graphs and the to the right there is a directed graph. The weigthed
graph could be used for deescribing cities and travel time between them. The directed graph could be used to describe relationships
between where relations are either one way or two way.

Probabilistic Relations. Probabilistic relations refer to relationships of stochastic variables. The core
concept of a stochastic variable is that from such a variableX, we can draw values according to a prob-
abilistic distributionP(X). Probabilistic relations thereby refer to the relationship between two or more
stochastic variables. This kind of prior knowledge describes how they relate, i.e., assumptions of indepen-
dence or the joint probability distribution. What it is not, however, is the distribution or other statistical
metrics of single variables, due to that such knowledge is easily found in the data.

Human Feedback. The concept of human feedback is strictly technologies that transform knowledge
from humans into machines. The choice of such input can vary. This knowledge is often unformalized
and often includes relevance or preference feedback. More so, there is usually no need for a human to
explain a decision made or feedback given.

### Knowledge integration. Integrating knowledge in the ML process can also vary. Therefore, Von-

rueden, Mayer, Beckh,et al.[4] have separated them into four categories.

Training Data. Training data is perhaps the most used way of using knowledge in the process. This
primarily consists of feature engineering, where features are created using the expertise of the problem
domain. Although, according to Vonrueden, Mayer, Beckh,et al.[4]’s definition, this is not IML. Instead,
the IML approach is where a separate source of knowledge is used to gather information to create another
dataset. This dataset can then be used together with the original data. An example of this is using
simulated data as a data source.


Hypothesis Set. Knowledge can also be incorporated into the hypothesis set, normally done through the
hyperparameters of a Neural Network (NN). There are a few examples of this; one of the most common
ones is spatial invariances of objects in images. Furthermore, knowledge can be used when choosing the
structure of a model. An example is to design the network to map symbols or logic rules to layers or
specific neurons in the network.

Learning Algorithm. The most common types of this kind of integration are seen in loss functions
modified according to additional knowledge. Typical knowledge comes in the form of algebraic equa-
tions.

Final Hypothesis. Knowledge can also be used in the final hypothesis of an ML pipeline, i.e., the final
output of such pipelines. In this step, knowledge can be used to put constraints upon the output, such as
physical laws, thereby discarding predictions that do not agree with such constraints [12].

### 2.2 Knowledge elicitation

Expert knowledge can enter decision-making processes in multiple ways, one is through expert knowl-
edge elicitation. Expert knowledge elicitation is acquiring insights and expertise from domain experts in
a particular field, intending to improve ML models.

Despite the possible benefits, this process of eliciting such knowledge is challenging [13]. One of the main
challenges is that experts may have different mental models or ways of thinking about a problem, which
can lead to conflicting insights. This can make it challenging to extract valuable and consistent knowledge
that can be applied to machine learning models. Furthermore, even if experts have similar mental models,
they may sometimes have differing views on the relative importance of different factors, which can cause
disagreements and inconsistencies. This is why it is essential for experts and ML engineers to build
common ground and, thereby, a mutual understanding of the problem space. Furthermore, experts may
not always be able to formalize their knowledge explicitly. This is particularly true if the knowledge is
based on intuition or experience rather than formal rules or principles.

This can make it challenging to translate this knowledge into structured formats that can be used in
ML models. Additionally, the explicitly stated knowledge may be incomplete or inaccurate, which can
further complicate the process. Furthermore, domain experts may not have the technical knowledge or
understanding of machine learning models to communicate their knowledge effectively. This can lead
to misunderstandings and misinterpretations, which can limit the effectiveness of the elicited knowledge.
For example, experts may not be familiar with the concepts of over-fitting or regularization, which are
important considerations from an ML process perspective.

Another important aspect of expert knowledge elicitation is to consider what the goal of the elicitation
is. Kerrigan, Hullman, and Bertini [13] uses four categories for elicitation goals: problem specification,
feature engineering, model development, and model evaluations. Connected to the goal of the elicitation
is the elicitation target or knowledge representation, i.e., how the knowledge is represented in the ML
pipeline. Continuing with the taxonomy defined by Kerrigan, Hullman, and Bertini [13], we will go
through their general outlines. Background knowledge and process are two of the most seen elicitation
targets. This includes the domain knowledge and workflows of domain experts. Labeling functions try
to capture the logic behind how we classify differently. These can either be logical rules or heuristics.
Connected to labels, we can also find some elicited knowledge in the form of labels of data points and
comments or explanations of the reasoning behind a particular label. Furthermore, specific data points
can be elicited from the domain experts in some cases. These usually contain specific boundary points or
other points of interest that need more attention.

Elicitation of knowledge concerning features is also common. These can include explaining features, the
relationship between features, the relevance of features, transformation functions for specific features to
make them more usable, and weights for specific features. Furthermore, sometimes even the direction of
the features, i.e., if the feature has a positive or negative or no impact on the output of the model.


In several ways, elicited knowledge can impact the model and the results. First is model constraints.
This has several benefits but one of the most prominent ones is that such models with constraints from
domain experts will generally be more trustworthy [4]. Furthermore, model selection is another elicitation
target, which generally involves experts choosing between different trained models with their expertise
in mind. Furthermore, feedback on the results can be elicited from domain experts. This is usually an
iterative improvement of the model’s output and performance or if the model does not match the expected
behavior [13].

Continuing with the elicitation process, there are several results of interest if the elicitation process is
defined as the medium through which the domain expert(s) and ML researcher is communicating. [13]
highlights some of the most common approaches we will go through. One of these is a custom application.
A custom application is a computer application specifically made for that task and, thereby, that specific
problem. Next up are meetings or interviews where verbal communication is used to elicit knowledge.
These can be more or less structured. There are also several other that is seen on less scale. For example,
shadowing is where the researcher follows the domain experts to capture how and what knowledge is used.
Another approach is think-aloud, which includes the domain expert describing their thought process while
they are performing different tasks. Lastly, there is also writing, for example, gathering cheat sheets or
similar documents that are used on a daily basis.

## 3 Related work

This section provides a description of related work. Firstly by looking at related works focusing on
decision-making and secondly, by looking at previous related works that focus on the trends in the usage
of expert knowledge in applied ML.

### 3.1 Decisions making

In their paper, Loftus, Tighe, Filiberto,et al.[56] review weaknesses of human decision-making within
the medical field. Especially decisions made through hypothetical and deductive reasoning as well as
individual judgment. They continue by writing:"These factors can lead to bias, error, and preventable
harm."Their solution to this lies in using an automated AI system to make decisions by receiving con-
tinuous health record data. However, they mention a few challenges that need to be overcome in order to
use this approach entirely. Some of them arestandardizing data,increasing interpretability of the model,
accounting for model biasas well asaccountability for errors, to name a few [56]. Handling this while
preserving human intuition in the process of decision-making is key.

Yet, Perkins, Rasmussen,et al.[49] presents a methodology for building a Bayesian Network (BN) [57]
to support decision making. The method combines meta-analysis, expert knowledge, and data. In the case
study, they built a BN model to help make decisions during traumas of the lower extremities. The model
could accurately predict the viability of lower extremities with severe vascular trauma. Furthermore,
in a 10-fold cross-validation, the model outperformed the mangled extremity severity score, which is
a well-known scoring system for such injuries as well as four different solely data-driven approaches.
Similarly, Constantinou, Fenton, and Neil [17] proposed a method for incorporating expert variables into
a BN without changing the model’s expectations. Yet, Perkins, Fenton,et al.[11] proposes a method for
developing BNs with a combination of expert knowledge and data to predict acute traumatic coagulopathy
in trauma care. Their methodology also provide an iterative review by domain experts of the predictions
to refine the model.

Muralidhar, Islam, Marwah,et al.[37] proposes a network architecture that leverages prior domain
knowledge and compares the network with a vanilla network of similar architecture. They specifically
test this network with either noisy or sparse data. The authors show promising results both for noisy
and sparse data situations. Future work will focus on extending the model to use more complex network
architectures as well as more domain rules.

Another topic, called predictive maintenance, aims to predict beforehand whether a product or system is


likely to malfunction in the near future, which allows for planned maintenance rather than an unexpected
breakdown.

Nikitin and Kaski [58] elicits and incorporates expert knowledge as decision rules to give the system
additional information. A basic example is a human expert who could produce a decision rule that states,
"xis not broken becausey>−1", which they know due to their knowledge about a certain system. More
so, they write that the method is only applicable when the experts can elicit heuristic decision rules,
something they argue is possible for most modern ML problems [58].

While the fields of research might be different from one another (e.g., the field of equipment or system
repair vs. the medical field), especially regarding the harm that can be done by making mistakes in the
decision-making process, there are also similarities. A model would not be used if it made bad decisions
compared to an expert. Additionally, if an expert is required to make decisions after a model has made
an incorrect prediction, it could lead to cost and efficiency problems. Nevertheless, there are factors that
are important in most fields, such as having standardized data and the preservation of human intuition (by
formalizing that data). Increasing the interpretability of the model is also valuable for increasing trust in
the model.

### 3.2 Expert knowledge

Vonrueden, Mayer, Beckh,et al.[4] provide an overview of the field IML, which involves using prior
knowledge in machine learning to improve performance. They performed a survey and developed a
taxonomy to categorize different approaches. They continue to describe various approaches and discuss
the challenges and how to evaluate the effectiveness of said approaches. As this work builds upon that
foundation, a more detailed description of their work is provided in Section 2. However, our work differs
from theirs by looking at a broader perspective of the ML pipeline and we also consider the elicitation of
the knowledge.

Similarly, the work by Kerrigan, Hullman, and Bertini [13] also provide a foundation for our work. Their
article provide an overview of elicitation methods seen in applied ML research that used domain experts
to enhance the ML projects. They also provide a taxonomy and survey articles with a focus on elicitation,
however, without the context of knowledge representation, which is essential for our work. Furthermore,
we look at the ML pipeline in more detail. A more detailed description of their work is provided in
Section 2

O’Hagan [59] provides an overview of different challenges and approaches to elicit expert knowledge
probability distributions and highlights several pitfalls, e.g., anchoring, availability, range frequency, and
overconfidence. Furthermore, they also provide several practices for making the elicitation as rigorous
and scientific as possible and discussing the challenges of eliciting joint probability distribution for mul-
tiple uncertainty quantities.

Experts systems have been around for a long time and are one of the first approaches to use AI in decision-
making. Wagner [60] analyzed over 300 expert systems case studies ranging between the years 1984 to

2016. The authors provide an overview of expert systems and highlight the milestones and trends over
the years. The authors also discuss the limitations of such systems as well as the need for robust strategies
to avoid bias and validation of the elicited knowledge.

## 4 Methodology

The main goal of the survey and analysis is to gain insight into how ML practitioners elicit knowledge,
formalize, and structure that knowledge as well as the challenges and motivations associated with their
approach, i.e.,RQ1andRQ2. To achieve this, a number of peer-reviewed articles between 2003 and
2021 were collected. The remainder of the chapter explains how the articles were collected and analyzed.


### 4.1 Search strategy and selection

Since the aim of the review is in the intersection of both the domain of expert knowledge elicitation and
the expert knowledge domain of IML, the only articles considered were articles that focused on expert
knowledge elicitation for machine learning purposes and also articles that are in the domain of expert
knowledge IML. Additionally, the experts were aware that the elicitation was being done. Therefore,
this eliminated areas with already existing knowledge bases, such as world knowledge and scientific
knowledge, which is further explained in Section 2.

To begin this study, the primary search engines utilized were: Google Scholar, IEEE Xplore, and ACM
digital library to search for papers using a combination of keywords such as "Expert Knowledge," "In-
formed Machine Learning," and "Knowledge Elicitation." This yielded many articles, but by reading the
title, abstract, and if necessary the introduction and conclusion, irrelevant articles could be discarded if
they did not fit into this domain.

### 4.2 Content analysis

To achieve the aim of this study, research papers were analyzed, and several key aspects of the elicitation
process were identified. The first step was looking into the taxonomies of Vonrueden, Mayer, Beckh,
et al.[4] and Kerrigan, Hullman, and Bertini [13] and seeing which aspects were relevant to this study.
These first characteristics were discussed to be able to find what is usable for us. The initial list was then
iteratively updated when certain characteristics fit better clustered together, while others were eliminated
in order to find the right level of granularity. This process was conducted as follows.

The first focus was on the goal of the elicitation, i.e., where in the ML pipeline the elicited knowledge
was utilized. The next step was examining the type of information that was the target of the elicitation,
as well as how it was represented in the ML pipeline. Furthermore, the method used for the elicitation,
along with its motivations and challenges, was investigated. This whole process is what is referred to as
an elicitation path in this study. Important to know is that one article can have multiple elicitation paths,
for example, by integrating knowledge in different parts of the ML pipeline.

In addition to identifying the elicitation paths within research papers, information on the motivations
and challenges associated with each path was collected. Understanding these motivations and challenges
can provide a more comprehensive understanding of the elicitation process and can inform best practices
for future research. The motivation for using specific elicitation methods can vary depending on the
research question(s) and the type of information being sought. For example, interviews may be used to
gain a deeper understanding of a particular domain or to gather subjective opinions and experiences from
human experts. Conversely, surveys may be used to collect large amounts of quantitative data quickly
and efficiently.

Challenges in elicitation can arise at different stages of the process. For example, recruiting participants
with the necessary expertise or knowledge can be difficult, and there may be issues with participant bias
or incomplete responses. Additionally, the choice of elicitation method may impact the quality and relia-
bility of the data collected, and it can be challenging to balance the need for detailed information with the
practical limitations of time and resources. Overall, this analysis aimed to provide a comprehensive un-
derstanding of the elicitation process used in ML research and to identify the best practices and challenges
associated with it.

To summarize, multiple articles were analyzed to identify the elicitation paths used in ML research. The
questions below were created in order to have the right amount of granularity to be able to group articles
and elicitation paths together. The goal is to better understand trends, motivations, and challenges with
knowledge elicitation and facilitate future work that requires knowledge elicitation and integration.

- ML pipeline: Where in the pipeline was the knowledge integrated?
- Knowledge target: What was the target knowledge of the elicitation?
- Elicitation medium: How was the knowledge elicited, i.e., using what medium?


- Knowledge representation: How was the knowledge represented?
- Elicitation motivation: What was the motivation behind the choice of the elicitation method?
- Elicitation challenges: What were the main challenges faced during the elicitation process?

In some cases, multiple elicitation paths were identified within a single article. In those cases, information
was collected in each path with the goal of answering the questions above for each path. Overall, the
analysis aimed to provide a comprehensive understanding of the elicitation process used in ML research
and the challenges and motivations associated with it.

Furthermore, in cases where the elicitation medium is not explicitly written or demonstrated, assumptions
were made if possible. For example, if an expert gives direct feedback to a model, the elicitation medium
is consideredcustom application.

During the process, the classification for the different categories of interest was updated to better cover
necessary information. Every paper was classified by one of the authors, but complex cases or other
difficult judgments were discussed between both authors. After the initial coding phase, the next step
was to go through the data and discuss additional ambiguities, as well as the challenges and motivations
within the reviewed articles. More so, the challenges with the elicitation and the motivations for why that
method was used were grouped within specific categories in order to better understand and visualize the
data.

Lastly, to improve validity, 25% of the papers were selected at random for an additional read-through by
both authors, where they were classified anew; the consistency between the two coders was high. This
showed that the category definitions had clear definitions.

In total, 43 papers were analyzed, and 96 elicitation paths were found. In the following section, the
elicitation taxonomy will be described in detail.

## 5 Elicitation taxonomy

The top level of the proposed taxonomy consists of five phases that together represent the proposed
definition of a machine learning pipeline, see Figure 3. Thereafter, we continue describing theelicitation
mediums,knowledge target, andknowledge representation.

### 5.1 Machine learning pipeline

To provide context towards how elicitation approaches differ in different phases of an ML pipeline. We
hereby define our structure of an ML pipeline. An overview of the pipeline can be seen in Figure 3.

The first phase isproblem specification. In this phase of an ML project, the objectives and goals are
clearly defined, and the problem type is identified, i.e., classification, regression, clustering, and so on.
The criteria for success are established, taking into account the perspectives of domain experts and stake-
holders. The current practices, processes, and workflows related to the problem are analyzed to gain a
deeper understanding of the context and challenges of the problem. In addition, the data is collected
during this phase of the ML pipeline.

The next phase isfeature engineering. In this step, the data is preprocessed to ensure that it is clean,
consistent, and ready for use in the training phase. This step may involve removing missing values,
scaling features, or transforming the data into a suitable format for the model. This also involves selecting
the relevant features for the problem to solve.

Themodel structurephase involves choosing the appropriate model for the problem. This involves
selecting the model structure and model parameters according to the problem. In some cases of elicitation,
this can be a bit ambiguous from the previous phase. However, the distinction is that elicitation in this
phase affects the model’s behavior. More so, a limit is that this stage does not include the network’s
training process. as discussed next.


```
Problem
specification
```
```
Feature
engineering
```
```
Model
structure
```
```
Model
training
```
```
Model
evaluation
```
Figure 3.Machine Learning Pipeline.

Model trainingis the next phase and consists of a model’s actual training. We use this stage because
prior information enters this stage explicitly. For example, this may involve specific loss terms or that
training feedback from an expert is used in the training of the ML model. Furthermore, this also involves
parameters specific to the learning algorithms.

Lastly is themodel evaluation, which involves identifying appropriate measurements for evaluating the
model. This is typically measured with metrics such as accuracy, precision, or recall depending on the
goal of the model. This can also be using experts to evaluate the model subjectively.

### 5.2 Elicitation medium

Several approaches for the elicitation process were found, some similar to those presented by Kerrigan,
Hullman, and Bertini [13]. However, the definitions in this research differ somewhat from their taxonomy
in order to better fit what is relevant from the industrial case. The taxonomy used in this research is
presented below.

One well-known elicitation process is the use ofmeetings or interviews, which can be employed at
various stages of the ML pipeline and for different purposes. Here, it is defined as encompassing both
meetings among multiple experts and interviews with one or more experts. However, as previously noted,
the specific goals of the process can vary, as can the level of structure involved.

Another category iswriting and surveys, which involves written communication with experts, such as
cheat sheets or responses to specific questions that can be distributed to several experts without the need
to gather them in one place.

Shadowingof experts is another approach, which can involve observing an expert at work and studying
how they solve problems. It may also involve recording experts’ sessions as they work, such as through
audio, video, or screen recordings.

Practitioners have also createdcustom applicationsor interfaces to gather the information specific to the
problem at hand.

If the researcher(s) have not declared how the knowledge was elicited, and it cannot be derived from the
text, it is marked asunknown.

The rest of the section describes the different parts of the proposed definition for an ML pipeline, provid-
ing insights into different kinds of knowledge elicited in the different phases and how the knowledge is
represented. Furthermore, insights into the challenges with the elicitation are listed.

### 5.3 Knowledge target

For the knowledge target, our study’s approach is based on Kerrigan, Hullman, and Bertini [13]. How-
ever, the granularity in their definitions does not entirely align with this research’s goal. Therefore, the
approach in this research has to be clearly defined.

The term knowledge target refers to the specific type or form of knowledge that is intended to be obtained
from domain experts during the elicitation process. It refers to the target knowledge of the elicitation.

Model constraintsconcerns elicitation about range constraints for the values in the predictions, the ac-
cepted range that features can take on, or monotonicity constraints [61]. This also includes constraints


for the structure of models such as BN.

Results feedbackcovers elicitation approaches where domain experts are asked to evaluate a result of a
model or even the results of specific instances. The feedback can be used to evaluate the model as a whole
and give direct feedback to the training algorithm. Furthermore, in some cases, it can be seen that experts
evaluate the relevance of specific features or how good the model’s explanations for specific decisions
are.

Background knowledgecovers all information about the domain, such as experts’ current practices, pro-
cesses, and workflows. Potential challenges in the domain are also covered by background knowledge.

Labels, this category covers everything concerning the labeling of data, including specific labeling by
experts or experts providing functions or workflows for labeling data.

Related to labels arelabel explanations. This category is about experts discussing the reasoning or
providing explanations for selecting a particular label for a given instance.

Data instancesare specific data points provided by experts. Examples of this can be specific data points,
such as complex cases or edge cases that are hard to determine and need further study. These data
instances might not even exist in the data currently. Therefore, they have to be synthetically added by
experts.

Several knowledge targets concern features, the first beingfeature relevance. This approach typically
involves domain experts rating the relevance of each feature concerning the outcome. This includes
binary decisions if a feature is relevant and the possibility to rank features against each other regarding
how relevant they are, which can guide the selection of the most relevant features to be utilized in the
model.

Feature weightsconcern the magnitude of features, i.e., how much features impact the outcome of a
prediction. The distinction between this and feature relevance is that this is quantifiable, i.e., the features
have discrete weight values, while feature relevance does not.

Feature directionsapproach requires experts to provide information about the directionality of each fea-
ture with respect to the outcome variable. For example, experts may identify which features are positively
or negatively associated with the outcome variable.

Feature relationshipapproaches involve experts identifying and characterizing relationships between
different features. This can include identifying which features are likely to be correlated or which are
likely to interact with each other nonlinearly. This information can be used to engineer new features or to
create interaction terms that capture the relationships between different features.

Feature explanationsare additional information provided that explains a specific feature. This can be
information about how a feature is derived or other information about the feature.

Feature transformationare specific functions or workflows experts provide to transform a feature or
features towards a more relevant feature for the prediction.

Probability distributionsinclude prior distributions for things such as BN or when there might be an
already known distribution of one or several variables.

### 5.4 Knowledge representation

For the knowledge representation, the approach is based on Vonrueden, Mayer, Beckh,et al.[4] but with
alterations to better fit the structure and approach of this study.

Human feedbackis a category that involves all sorts of human feedback that can not be put into a specific
category. An example of human feedback is when humans evaluate the predictions of a model.

Algebraic Equationsrepresents knowledge in the form of equality or inequality between mathematical
expressions, i.e., constants and variables. These can represent specific loss term functions, ranges of


values, or other mathematical expressions.

Synthetic resultsknowledge can come from the simulation of numerical outcomes in real scenarios. This
may be seen as the same as equations; however, Vonrueden, Mayer, Beckh,et al.[4] separates them in
thatequationsis a compact numerical mathematical model while synthetic results are only numerical
results. Examples of this are simulated pictures of traffic scenarios. Furthermore, this also includes
gaining specific data points of interest to the case, such as edge cases that might not exist in the data.
These cases can either be manufactured, simulated, or in some cases, provided solely by experts that have
encountered them in the field.

Knowledge Graphsconsists of vertices and edgesG(V,E). Knowledge graphs normally describe objects
or concepts, whereas the edges describe their relations. Graphs can be directed, meaning that relations
can be either in one or both directions. They can also be weighted, meaning that edges with the same
concepts could have different magnitudes. In Figure 2, examples of graphs are shown.

Probabilistic Relationsrefer to relationships of stochastic variables. The core concept of a stochastic
variable is that from a variableX, values can be drawn according to a probabilistic distributionP(X).
Probabilistic relations thereby refer to the relationship between two or more stochastic variables. This
kind of prior knowledge describes how they relate, i.e., assumptions of independence or the joint prob-
ability distribution. For the approach in this study, the distribution or statistical properties for single
variables are also included, contrary to Vonrueden, Mayer, Beckh,et al.[4]

### 5.5 Motivations and challenges

The motivations were first and foremost collected from the articles, or listed asnot specified. The pa-
pers that did not specify motivations explicitly required a more contextual understanding to extract this
information. This meant that the first step was to write down the motivations stated by the papers in free
text, either directly or paraphrased. When that was done, they were simplified into their essences. Fi-
nally, categories were created in order to be better able to group the different motivations. Two examples
of this are: "Useful for small datasets with high variable counts" [34], which would be summarized as
dataset size, and "Performance & acceptance by other experts" [23] which would have two motivations;
improving performanceas well asincreasing trustworthiness.

In a similar fashion to how the motivations were collected, the challenges with knowledge elicitation
were also retrieved. One difference from the motivations was that the challenges were not extracted
using a contextual understanding of the papers. That means if no challenge was explicitly stated, it
was categorized asnot specified. Two examples of paraphrased challenges and what the final categories
they were placed in are as follows: "Features differ between experts’ data" [42], or "High-quality expert
knowledge difficult to obtain" [38]. The essence of these two examples would be "subjectivity" and "lack
of experts," respectively.

## 6 Survey Results

This section provides an overview of the results found in the survey. Then, for each part of the ML
pipeline, a more in-depth result presentation is made, pointing towards common elicitation trends as well
as noting some special cases. The most prominent paths can be seen in Figure 4. While the distribution
of paths over the different parts of the ML pipeline can be seen in Figure 5. The distribution is not equal
between the different parts of the pipeline, wheremodel trainingwas the most common with 36% and
problem specification25% of the total number of paths identified.

### 6.1 Problem specification

Theproblem specificationphase covers 25% of the total paths found. A visualization of the found results
can be seen in Figure 6. A few approaches appeared while reviewing articles in this phase of the ML
pipeline. By observing the left chart in Figure 7, it can be seen that the most notable category in the


```
Feature engineering
Model structure
```
```
Model training
```
```
Model evaluation
```
```
Problem specification
```
```
Feature relevance
```
```
Labels
```
```
Feature relationships
```
```
Label explanations
```
```
Feature weights
```
```
Feature explanations
```
```
Results feedback
```
```
Feature tranformation
Model constraints
```
```
Probability distribution
```
```
Background
```
```
Data instances
```
```
Feature direction
```
```
Logical rules
```
```
Synthetic results
```
```
Algebraic equations
```
```
Probabilistic relations
```
```
Human feedback
```
```
Knowledge graph Shadowing
```
```
Custom app
```
```
Writing / surveys
```
```
Meetings / interviews
```
```
Unknown
```
```
ML pipeline Knowledge target Knowledge representation Elicitation medium
```
Figure 4.The Sankey diagram shows the elicitation paths found. Each column represents one category in the taxonomy. The
taxonomy has four categories, each represented by a column. From left to right, these are the Machine Learning Pipeline (blue),
Knowledge Target (green), Knowledge Representation (purple), and Elicitation Medium (yellow). The paths between the categories
indicate their frequency, with the thickness of the paths representing their relative commonness

(^0) Problem specification Feature engineering Model structure Model training Model evaluation
20
40
60
80
100
Distribution of paths by part of ML pipeline
Percentage (%)
ML pipeline
Figure 5.Distribution of paths by part of ML pipeline, sorted by the order of the pipeline.
knowledge target isbackground knowledge. This is arguably a broad category, but it needs to be that way
due to the wide range of problem spaces found in research. In this category, specific information about
the domain or the processes and workflows of experts exists.
In some cases, experts can be seen providing data instances for edge cases. Some notable examples are
[24], [41], [47].
There are instances where domain experts have also provided labeling functions. In addition, various
information about labels is also included in this category. For example, Bowles, Ratcliffe, Potashnik,et
al.[52] provide labels for data instances by consulting multiple independent experts.
Due to the nature of the knowledge in this phase, the majority of theknowledge representationlevel
is dominated by thehuman feedbackcategory, as can be seen in the middle chart in Figure 9. This is


```
Problem specification
```
```
Background
```
```
Feature explanations
```
```
Data instances
```
```
Labels
```
```
Human feedback
```
```
Synthetic results
```
```
Algebraic equations Shadowing
Custom app
Writing / surveys
```
```
Meetings / interviews
```
```
Unknown
```
```
ML pipeline Knowledge target Knowledge representation Elicitation medium
```
Figure 6.The Sankey diagram shows the elicitation paths found for the problems specification phase in the machine learning
pipeline. The taxonomy has four categories, each represented by a column. From left to right, these are the Machine Learning
Pipeline (blue), Knowledge Target (green), Knowledge Representation (purple), and Elicitation Medium (yellow). The paths be-
tween the categories indicate their frequency, with the thickness of the paths representing their relative commonness

```
BackgroundData instances
```
```
Labels
```
```
Feature explanations
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Human feedbackSynthetic resultsAlgebraic equations
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Meetings / interviews
```
```
UnknownCustom appShadowing
Writing / surveys
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Problem specification
```
```
Percentage (%)
```
```
Knowledge target Knowledge representation Elicitation medium
```
Figure 7.A collection of charts describing the findings in the problem specification phase. The green area on the left shows the
intended knowledge target. The purple area in the middle represents the captured form of this knowledge. The yellow area on the
right indicates the medium used to elicit the knowledge.

because the majority of the knowledge in theproblem specificationphase is either not explicitly stated or
in a form that is not formalized. However, we can see a few approaches withsynthetic resultsas well as
algebraic equations[26].

The majority ofelicitation mediumsused in this phase of the ML pipeline falls under themeetings and
interviewscategory. However, it can be observed in the right chart in Figure 7 that there are some ap-
proaches usingcustom applicationandshadowing. Only one noted that they usedwriting or surveys.
The rest fall under theunknowncategory, which means that the elicitation medium was not declared and
could not be implicitly extracted.

### 6.2 Feature engineering

Thefeature engineeringphase covers 16% of the total paths found. A visualization of the found results
can be seen in Figure 8. There are several ways in which expert knowledge can enter the ML pipeline in
thefeature engineeringphase. By observing the left chart in, Figure 9, it is noted that the most common
knowledge target is thefeature importanceandfeature relationshipscategories. Together they make up
most of the found elicitation paths in this phase.Feature directioncan be found in a few cases, and similar
metrics can be seen withfeature weights,feature transformations, andfeature explanations. For exam-
ple, Hu, Granderson, Auslander,et al.[26] provide a very detailed description of what kind of knowledge
was the target of their elicitation.Probability distributionscan be seen in some cases where experts have


```
Feature engineering Feature relevance
```
```
Feature relationships
```
```
Feature weights
Results feedback
```
```
Feature tranformation
```
```
Probability distribution
```
```
Feature direction
```
```
Human feedback
```
```
Probabilistic relations
Algebraic equations
```
```
Shadowing
```
```
Custom app
```
```
Writing / surveys
```
```
Meetings / interviews
```
```
Unknown
```
```
ML pipeline Knowledge target Knowledge representation Elicitation medium
```
Figure 8.The Sankey diagram shows the elicitation paths found for the feature engineering phase in the machine learning pipeline.
The taxonomy has four categories, each represented by a column. From left to right, these are the Machine Learning Pipeline (blue),
Knowledge Target (green), Knowledge Representation (purple), and Elicitation Medium (yellow). The paths between the categories
indicate their frequency, with the thickness of the paths representing their relative commonness

```
Feature relationships
Feature relevanceFeature direction
Feature tranformation
```
```
Feature weights
Probability distribution
```
```
Results feedback
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Human feedback
Probabilistic relationsAlgebraic equations
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Meetings / interviews
```
```
Custom appShadowingUnknown
Writing / surveys
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Feature engineering
```
```
Percentage (%)
```
```
Knowledge target Knowledge representation Elicitation medium
```
Figure 9.A collection of charts describing the findings in the feature engineering phase. The green area on the left shows the
intended knowledge target. The purple area in the middle represents the captured form of this knowledge. The yellow area on the
right indicates the medium used to elicit the knowledge.

provided statistical data to enhance features.

The form ofknowledge representationis mainly thehuman feedbackcategory; see the middle chart
of Figure 9. There can be seen single cases where theknowledge representationis stated in a more
formalized form, i.e.,probabilistic relationsandalgebraic equations.

Continuing by looking at the right chart in Figure 9, it can be observed that the majority ofelicitation
mediums used fall under themeetings and interviewscategory. Although a few cases can be seen that
usedcustom applicationspecially made for the task. The same goes for theshadowingcategory, where
only a few cases can be seen.

### 6.3 Model structure

Themodel structurecovers 10% of the total paths found. A visualization of the found results can be seen
in Figure 10. We see a bit wider distribution of approaches in the model structure phase. By observing
the left chart in Figure 11, it can be seen that the majority ofknowledge targetis in the categorymodel
constraints. The majoritymodel constraintsare from the creating of a BN using expert knowledge of
the problem [11], [19], [32], [34], [38], [48]. There are a few approaches wherefeature relationship
has affected the model structure phase. These are mainly the same papers listed above, where they have
defined the arcs in the knowledge graphs in a static manner.

Several fascinatingknowledge representationswere seen in the collection of papers. By observing the
middle chart in Figure 11, we can see that most representations are in the category ofknowledge graph.


```
Model structure
```
```
Feature relationships
```
```
Model constraints Knowledge graph
```
```
Logical rules
Algebraic equations
```
```
Meetings / interviews
```
```
Unknown
```
```
Writing / surveys
```
```
ML pipeline Knowledge target Knowledge representation Elicitation medium
```
Figure 10.The Sankey diagram shows the elicitation paths found for the model structure phase in the machine learning pipeline.
The taxonomy has four categories, each represented by a column. From left to right, these are the Machine Learning Pipeline (blue),
Knowledge Target (green), Knowledge Representation (purple), and Elicitation Medium (yellow). The paths between the categories
indicate their frequency, with the thickness of the paths representing their relative commonness

```
Model constraints
Feature relationships
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Knowledge graphAlgebraic equations
```
```
Logical rules
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Meetings / interviews
```
```
Unknown
Writing / surveys
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Model structure
```
```
Percentage (%)
```
```
Knowledge target Knowledge representation Elicitation medium
```
Figure 11.A collection of charts describing the findings in the model structure phase. The green area on the left shows the intended
knowledge target. The purple area in the middle represents the captured form of this knowledge. The yellow area on the right
indicates the medium used to elicit the knowledge.

These are mainly the model constraints previously mentioned. Furthermore, it can be seen few instances
withlogical rules[42] in the form of decisions rules andalgebraic equations[26] describing value ranges
that are normal for specific features.

Continuing by observing the right chart in Figure 11, we can see that there is still a majority ofelici-
tation mediumin theinterviews and meetingscategory. However, we can also see some instances where
they have been described aswriting and surveys[48]. However, it should be noted that there are no
instances where this kind of knowledge is elicited usingcustom applications, which has an overall high
occurrence over the papers. Furthermore, it can still be observed that in a large part of the cases, the
elicitation medium was not clearly stated, i.e.,Unknown.

### 6.4 Model training

In themodel trainingphase, the majority of our observed cases of elicitation are, covering 36% of the
cases. A visualization of the found results can be seen in Figure 12. Several findings should be noted.
By observing theknowledge targetin the left chart in Figure 13, it can be seen that many cases used
experts to provideresults feedback. This is where experts have been used in the learning process. Notable
examples of this are by Cai, Reif, Hegde,et al.[54], where an interactive ML model can be adjusted
during training for the user’s specific needs. Furthermore, Knox and Stone [30] used a human in the loop
to provide a more effective learning algorithm.

Continuing by looking atfeature relationships, there are several approaches. Notable examples are
Masegosa and Moral [34], where the authors propose interactive learning of the relationships between


```
Model training
```
```
Feature relevance
```
```
Probability distribution
```
```
Feature relationships
```
```
Feature weights
```
```
Results feedback
```
```
Model constraints
```
```
Label explanationsData instances
```
```
Feature direction
```
```
Synthetic results
```
```
Algebraic equations
```
```
Probabilistic relations
```
```
Human feedback
```
```
Knowledge graph
```
```
Shadowing
```
```
Custom app
```
```
Writing / surveys
```
```
Meetings / interviews
```
```
Unknown
```
```
ML pipeline Knowledge target Knowledge representation Elicitation medium
```
Figure 12.The Sankey diagram shows the elicitation paths found for the model training phase in the machine learning pipeline. The
taxonomy has four categories, each represented by a column. From left to right, these are the Machine Learning Pipeline (blue),
Knowledge Target (green), Knowledge Representation (purple), and Elicitation Medium (yellow). The paths between the categories
indicate their frequency, with the thickness of the paths representing their relative commonness

```
Results feedback
Feature relationships
Feature relevance
Probability distribution
```
```
Feature directionModel constraintsData instancesFeature weightsLabel explanations
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Human feedback
Probabilistic relationsAlgebraic equations
```
```
Knowledge graphSynthetic results
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Custom app
Meetings / interviews
```
```
UnknownShadowing
Writing / surveys
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Model training
```
```
Percentage (%)
```
```
Knowledge target Knowledge representation Elicitation medium
```
Figure 13.A collection of charts describing the findings in the model training phase. The green area on the left shows the intended
knowledge target. The purple area in the middle represents the captured form of this knowledge. The yellow area on the right
indicates the medium used to elicit the knowledge.

nodes in three steps in a BN. Another prominent example is Fails and Olsen [22], where they used human
feedback to learn classifiers by marking pixels (by drawing on the picture) to provide feedback on what
features (pixels) relate to each other. Some cases can be seen to use thefeature relevanceapproach in
learning. Sundin, Peltola, Micallef,et al.[44] constructed a method that uses human feedback to provide
feedback on if a specific feature is relevant for predicting quantitative traits, such as cancer cells’ sensi-
tivity to a drug. In this case, the expert provides feedback by selecting either relevant (+) or relevant (-),
indicating thefeature directionand relevance, or that they do not know. Thereby providing bothfeature
relevanceandfeature direction.

Feature weightcan be observed in an article by Soare, Ammad-Ud-Din, and Kaski [43], where the more
relevant a feature is, the more weight is put on that feature. A notable approach in the training phase
also comes from Hester, Schaul, Sendonaris,et al.[24], where they combine a pre-training phase and
self-generating data phase called Q-learning from demonstration, thereby generatingdata instancesin
the training phase.Probabilistic distributioncan be seen in some approaches such as by Richardson and
Domingos [38] where they used multiple independent domain experts to learn both the structure of a
BN as well as theprobabilistic distributionof the network. Another case forprobability distributionis
by Altendorf, Restificar, and Dietterich [61], where the authors used domain experts from the medical
domain to estimate parameters for a probabilistic model.

Trends inknowledge representationcan be observed in the middle chart of Figure 13. Human feed-
backcontinuous to be a majority. This could be for several reasons, but one of the most prominent ones is
that in most articles in the survey, the author does not state how they represent the knowledge and thereby
only talk about the knowledge in an unformalized form, see Section 2. Some cases ofprobabilistic re-


lationscan also be seen BN, e.g., Feelders and Gaag [23] and Richardson and Domingos [38], but not
all forms of relations in a BN are represented in this manner. In some cases, they use only the priors
from experts and enhance it with data instead. Finally, a few cases ofAlgebraic equationscan be seen,
mainly in combination withmodel constraints. For example, Kurnatowski, Schmid, Link,et al.[31] and
Muralidhar, Islam, Marwah,et al.[37] uses monotonicity constraints from domain experts to compensate
for data shortages.

The most used elicitation medium in the model training phase iscustom applicationwhich was specif-
ically made for the task, which can be seen in the right chart in Figure 13. Notable examples here are
Brown, Liu, Brodley,et al.[53], where they made an application to accept user feedback to find data
patterns. As well as Fails and Olsen [22] that made an application to mark pixels to improve thefeature
relationships. In a number of cases, the elicitation medium ismeetings or interviews. One elicitation
medium approach that is not so prominent in other phases isshadowing. One example of this is Richard-
son and Domingos [38], where the authors tracked the actions of domain experts.Writing or surveyscan
only be seen in single instances in this stage [37].

### 6.5 Model evaluation

```
Model evaluation
```
```
Feature relevance
```
```
Results feedback Human feedback
```
```
Meetings / interviews
```
```
Unknown
```
```
Custom app
```
```
Writing / surveys
```
```
ML pipeline Knowledge target Knowledge representation Elicitation medium
```
Figure 14.The Sankey diagram shows the elicitation paths found for the model evaluation phase in the machine learning pipeline.
The taxonomy has four categories, each represented by a column. From left to right, these are the Machine Learning Pipeline (blue),
Knowledge Target (green), Knowledge Representation (purple), and Elicitation Medium (yellow). The paths between the categories
indicate their frequency, with the thickness of the paths representing their relative commonness

```
Results feedback Feature relevance
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Human feedback
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
UnknownCustom app
```
```
Meetings / interviews
```
```
Writing / surveys
```
```
0
```
```
20
```
```
40
```
```
60
```
```
80
```
```
100
```
```
Model evaluation
```
```
Percentage (%)
```
```
Knowledge target Knowledge representation Elicitation medium
```
Figure 15.A collection of charts describing the findings in the model evaluation phase. The green area on the left shows the
intended knowledge target. The purple area in the middle represents the captured form of this knowledge. The yellow area on the
right indicates the medium used to elicit the knowledge.

Themodel evaluationcovers 11% of the total paths found. A visualization of the found results can be
seen in Figure 14. In the model evaluation phase, it can be seen that a majority of the cases fall under
theresults feedbackcategory, as can be observed in the left chart in Figure 15. This includes almost all
cases where they used experts to evaluate a final model. However, the target of the evaluation differs
somewhat between articles. For example, some articles use domain experts to evaluate if the proposed


system improved the effectiveness of a task ([35], [47]) and others used experts for model refinement
([11], [42]). Furthermore, Lee, Siewiorek, Smailagic,et al.[33] used experts to compare their models for
personalized rehabilitation assessments.

However, one approach that differs from the others is using feature relevance in the evaluation stage.
Soare, Ammad-Ud-Din, and Kaski [43] evaluates how the model performs while increasing and decreas-
ing the budget for expert feedback in the form of feature relevance.

The knowledge representation follows the same trends with unformalized knowledge, as can be observed
in the middle chart in Figure 15.

Observing the right chart in Figure 15, it can be noted that the elicitation medium is not stated in most
cases. Although a few examples exist in thecustom applicationcategory [29], [54]. As well as some
approaches usingwriting and surveys, notably in Amershi, Lee, Kapoor,et al.[47]. Lastly, a few ap-
proaches can be seen in themeetings and interviewscategory, e.g., Seymoens, Ongenae, Jacobs,et al.
[42].

### 6.6 Motivations

(^0) Dataset size Trustworthiness Improve performance Data point creation
20
40
60
80
100
Distribution of specified motivations
Percentage (%)
Motivation
Figure 16.Challenges with "not specified" cases excluded.
In regard to the motivations for knowledge elicitation, the data distribution shown is from all paths, not for
every unique article. That is because researchers tended to motivate their different reasons for eliciting
knowledge for each path they took. The categories that motivations were categorized asdataset size,
improve performance,trustworthiness,data point creation, and lastly, the articles that did not specify any
motivation. While the purpose in one way or another is to increase the performance of a model, there
is a difference between having that as the primary or only goal or allowing for a more granular goal of
integrating qualitative data, for example.
Dataset sizeis categorized as either not having the amount of data required for the specific ML problem, or
for any other reason requiring to decrease the complexity necessary to solve the problem, by for example
enhancing the data.
Data point creationwas used for generating data points for edge cases that might not be in the data. The
difference between this anddataset sizeis that this is for specific data points in the same format as the
data, whiledataset sizewould aim to enhance the data by adding different kinds of data.


Improve performanceis directly related to improving the model’s performance without any direct sub-
goals.

Trustworthinessis another category that also included articles that specified their motivation as explain-
ability, as it can be argued is a sub-group of trustworthiness. Motivation such as "mimicking an expert"
would also be classified as part of trustworthiness.

In Figure 16, is the distribution of motivations but with the cases that do not specify any, removed. There
were a few articles that had multiple motivations specified. Those were individually added into their
respective categories. If an article had the motivationsdataset sizeandimprove performance, it was
counted as an entry in both categories.

The number of articles that did not specify any motivation was around 21%, see Figure 17.

(^0) Dataset size Not specified Trustworthiness Improve performance Data point creation
20
40
60
80
100
Distribution of motivations over full dataset
Percentage (%)
Motivation
Figure 17.Motivations with "not specified" cases included.

### 6.7 Challenges

Similarly to stating motivations for knowledge elicitation are the challenges with it, and they are grouped
into five different categories;subjectivity,accuracy,expensive,lack of expertsornot specified.

Subjectivity.There are a few reasons for an article to be placed into subjectivity regarding the challenges
with knowledge elicitation. In essence, it is categorized under subjectivity if different experts might
provide different answers to the same question(s). This could be due to their level of experience, education
level, or if the questions allow for subjective interpretation.

Accuracy. With accuracy, it means that the knowledge elicited from an expert might not necessarily
be accurate, for example, due to the difficulty or complexity of the problem. This differentiates from
subjectivity in two major ways. The first is if discrete values can represent the expert’s knowledge. The
second is that even if the expert is the best at this specific task, they might be unable to give accurate
answers.

Expensive.Expensive can refer to the elicitation being costly in terms of money. However, it would also
be classified as expensive if it took a lot of time or expert interaction.

Lack of experts. If the domain the expert is within is very specific or purely if the number of experts
available is sparse. This might make the elicitation difficult for others to replicate since experts might not
be available.


(^0) Subjectivity Expensive Lack of experts Accuracy
20
40
60
80
100
Distribution of specified challenges
Percentage (%)
Challenge
Figure 18.Challenges with "not specified" cases excluded.
Finally, if no challenges are mentioned, they fall into the category ofnot specified.
While one article might have multiple paths, when it comes to challenges, no article with more than one
path had more than one challenge specified. That means that even if an article had four different paths,
only one challenge was listed. Therefore the charts that present challenges are based on the number
of unique articles, which is 43. The distribution of challenges over the whole dataset, see Figure 18,
shows thatsubjectivityandexpensiveare the two primary challenges in 36% and 27% of the articles,
respectively. However, this excludes the papers which do not specify any challenges. The category ofnot
specifiedis by far the most common one, with almost 50% of the reviewed articles not specifying any
challenge with the knowledge elicitation. See Figure 19 for the distribution, including articles that are in
the categorynot specified.
(^0) Not specified Subjectivity Expensive Lack of experts Accuracy
20
40
60
80
100
Distribution of challenges
Percentage (%)
Challenge
Figure 19.Challenges with "not specified" cases included.


## 7 Discussion

This section provides a discussion split into two parts. Firstly we discuss the results and the challenges
associated with domain knowledge elicitation in general. Secondly, we discuss our approach and methods
for this work.

### 7.1 Results discussion

The most prominent result found in the study is that there is a general lack of descriptions of how expert
knowledge was elicited throughout the literature. In 26% of the elicitation paths found, theelicitation
mediumwas not described. Furthermore, in the most prominent categorymeetings and interviewsthat
make up for 34% of the elicitation mediums found, there is a lack of detailed description of how those
interviews or meetings were conducted. This is limiting for several reasons. First of all, if the elicitation
methods are not described properly, there is the potential risk of harming the reliability of such research
because it might not be possible to reproduce the research.

Furthermore, trustworthiness was one of the most significant motivators for eliciting knowledge found
in our survey. While we did not delve into how trustworthiness might have slightly different meanings
depending on the researcher but rather took the researchers’ own words for it. In general terms, we would
say that trustworthiness is when users of an AI system trust the system to make decisions, either with
them or for them. The level of trust is not something that we had in mind when conducting this research.

Continuing on with ensuring the trustworthiness of a model, we argue that at the very least, a clearly
documented path of the elicited knowledge should be included, i.e., how the knowledge was elicited, how
it was processed, as well as how and where the knowledge was used in the model. This, however, is not
the case in a majority of the articles in the survey. It might have the potential to impact the trustworthiness
of a model negatively. Comparing this to domains outside ML, clear documentation of elicitation seems
like standard practice to provide both traceability and transparency [13]. If this is done well, it provides
experts with clear paths on how their knowledge affects the ML model.

Furthermore, there is also a possible risk of conducting elicitation in such a way that it might provide bias
into the ML pipeline. Different approaches must be considered to ensure an unbiased approach depending
on the type of knowledge to be elicited. For example, for gathering statistical properties, there are many
pitfalls, such as anchoring and overconfidence [59]. More so, even though we do not specifically look at
the description level of the differentelicitation mediums, there is a general lack of description on how the
elicitation was done. Even if the method was specified ascustom application, that does not mean the user
interface is described. While formeetings and interviews, the questions were not described. This further
points towards the possible problem of reliability, transparency, and traceability of the work. However,
some papers clearly defined the questions asked, e.g., Hu, Granderson, Auslander,et al.[26].

There has been a clear motivation that the more formalized knowledge is, the easier it is to use from an ML
perspective [4]. However, we can see that 68% of the elicitation cases ended up in thehuman feedback
category for theknowledge representation. This is arguably a broad category because much knowledge
from theexpert knowledgedomain is informal [4]. However, there is a general lack of description of
the final form of the knowledge after elicitation, which leaves the question of how the knowledge was
integrated into the ML pipeline open for interpretation from the reader. We argue that in many cases that
fall under this category, a more detailed description would be possible, i.e., the knowledge elicited is not
impossible to formalize. If more detailed descriptions were available, splitting it up into two or more
categories would require a more granular category thanhuman feedback.

Another factor to consider is the path distribution by which part of the pipeline was relevant for that
particular path; see Figure 5. Problem specification, and more so,model trainingwas more common
than the others when it comes to knowledge integration in the ML pipeline. Model structurewas the
least common with only around 10%, as well asmodel evaluationat 12%. In reality, not all paths are
likely to be researched an equal amount, since different paths might be more interesting for researchers
overall. The articles that were chosen might not be completely representative of where the focus of


current research lie. Therefore, having covered more articles would better represent the whole population
of research, thus increasing the validity of claims regarding the research.

In regard to the categories of both challenges and motivations that we ended up with, they are in no way
the only necessary categories or perhaps not the optimal ones. We do believe, however, that they have
worked rather well for us. More so for the motivation categories than challenges, since they were usually
more straightforward, such as explicitly stating that the elicitation was done to increase trustworthiness.
The categories of challenges, for example,subjectivityandaccuracy, might arguably have a considerable
overlap since subjectivity might affect the accuracy and might need to be tweaked or combined in the
future. The bigger issue with the challenges is that almost 50% of the article paths did not specify any
challenge. That does not mean that there are no challenges with the knowledge elicitation, which is an
important distinction.

### 7.2 Method discussion

Finding the proper categories for the articles was iteratively done before we felt we had robust enough
categories. After all 43 articles with their 96 paths were categorized, we went over 11 of the articles
(around 25%) again individually in order to see whether we categorized them in the same way. Worth
noting is that while we did categorize them in the same way, we have been discussing the taxonomy with
all its categories for an extended period of time, which likely makes us have a similar mindset about it.
More so, given a larger time frame, it would be better to review all of the articles to ensure that we do not
accidentally pick a subset that is easily classified while potentially missing the more challenging articles.
Additionally, this sample of articles and our approach to classifying them is in no way a complete picture
of elicitation in applied ML. This is both due to the sample size. Also, due to that, there is a varying
language used to describe elicitation, knowledge, and similar concepts across the domains where ML is
applied.

Another way of validating, or at least improving, the categories would be to have one (or preferably more)
coders that would read a subset of the papers and have to follow our taxonomy to see if they would end
up with the same categories. While they might not categorize everything exactly like we did, that would
be a good topic for discussion. All in all, it would be beneficial to find better boundaries for the different
categories or possibly add or remove some of them.

The taxonomy with its categories was developed with regard to industry. What this means is that while
we developed the taxonomy, it was partly done with a focus on how the industry (Saab AB, Training and
Simulation in our case) could make use of existing expert knowledge in different stages of an ML project.
What this means, is that there is a risk with the reliability of this work since many factors are based on
what we as the authors deem important, both in terms of the actual categories, but also in terms of the
granularity of the categories. Even though we wanted to keep the categories broad enough, so they are
not only usable by specific companies or researchers. However, since we only worked with one company
there is always a risk that other companies or researchers might have wanted the focus to lie elsewhere.
The process of choosing the categories might be difficult to reproduce with the exact same results, mostly
due to a small difference in granularity could yield different results, and it could be its own research to
specify the exact granularity required for certain work. Instead, we argue that our work is sufficient as a
foundation when working with expert knowledge elicitation in different parts of the ML pipeline.

## 8 Application to the industrial case

The results presented in this section are based on the experience and knowledge gained from conducting
the survey and developing the taxonomy. But also through continuous communication, workshops, and
meetings with people working at Saab AB, Training and Simulation during the whole duration of this
project.

The incentive from Saab AB, Training and Simulation is to use our work as a foundation for eliciting
expert knowledge in the domain of equipment maintenance, with the goal of further improving their


decision-making. Specifically, they are interested in how to incorporate maintenance personnel’s ex-
pertise into an ML pipeline. However, the case is in its initial stage, and therefore the amount of data
necessary is not available, as well as what data should be collected to provide decision support in the fu-
ture. Additionally, variations in the environment across sites may lead to differing views among domain
experts on what causes problems and how to fix them.

In accordance with our findings in the survey, this section provides recommendations for the industrial
case. As the case is in an early stage, expert knowledge is valuable in every stage of the ML project
pipeline. While the cost of knowledge elicitation and integration is an important factor, initially it is more
important to focus on doing the expert elicitation correctly, since that is likely to lead the project forward.
Therefore we will now highlight and discuss possible approaches for the industrial case based on the
findings of this work.

Firstly, as noted by several articles as well as similar surveys [13], it is of utmost importance to create a
common understanding of the problem space between ML practitioners and domain experts. This kind of
elicitation is mainly done in theproblem specificationphase but is nevertheless true for the whole project.
For this, most approaches have usedmeetings and interviews. Furthermore, for this to be effective,
we argue that careful consideration of the questions ensures a correct view of theproblem description.
Alternatively, one could look at more rarely seen approaches such as shadowing the experts to highlight
workflows that might not be apparent to them.

For themodel structure, there are a few different approaches, such as using a BN [57] or alternatively
considering a multi-stage decision approach using logical rules. However, cases exist where it is not
possible to provide a decision through decision rules. In those scenarios, the recommendation from the
statistically most likely cause of the fault should be considered. Other approaches, such as decision trees
[62] might be considered at a later stage in the project. We argue, due to previous solutions found in
our survey for cases with similar characteristics, that a BN [57] is the most appropriate model for the
industrial case. A BN is a directed knowledge graph that tries to capture expert knowledge. Formally it is
a directed acyclic graph (see Section 2) that represents a set of edges and weighted vertices in the form of
probabilitiesG(V,E). The main reason for this is that the project is in its initial stage, where the data is
not sufficient by itself and BN does not necessarily need data. BN’s are ideal for providing probabilistic
estimates for which action is most likely to solve the problem thereby providing priority of which actions
to take.

We propose that the network is created in several stages. First off, learning the structure of the network
(model constraints) should be done by several experts (from multiple sites) individually and, after that,
discussed in a joint session with all experts included. This is due to potential environmental and op-
erational differences between the sites. For example, there could be differences in how equipment is
damaged between the sites or the general expertise available. Furthermore, one should evaluate the net-
work structure with additional independent experts not included in the previous stage. Traditionally this
has been done usingmeetings and interviews. However, an alternative approach could be to provide a
custom applicationorwritings and surveysto provide individual views of the problem before the joint
sessions.

When the network structure is established, estimations of the probability for different causes of a problem
should be estimated, again by several independent domain experts. This could be seen as amodel training
phase and the estimations should be concatenated to provide a more realistic estimate. Similarly, this
should also be evaluated with separate domain experts. Furthermore, when doing this, one must ensure
that the probabilities are as unbiased as possible, this can be done by following existing guidelines [59].

When a BN exists for a product, one should look at the ambiguous cases where it is hard to provide a
probability estimate on what action is most likely to solve the problem. The goal is to identify additional
features that could be relevant for determining the action. Normally, thefeature engineeringphase is
done earlier, but we argue by doing this at this point, the elicitation focuses on the important parts of the
problem, which might not be obvious at an earlier phase.

Different approaches exist when those features are found, depending on what type of feature it is. For


example, if the feature is of such a nature that it can be captured as data points, it is a candidate for addi-
tional data sampling; however, if it is not in the data, e.g., when additional observations or measurements
are required to be made by a person. Then, that additional task could be prompted to the user(s) of the
system in order to increase the certainty of the model. This could be built in as additional decision rules
for the system, similar to Nikitin and Kaski [58].

Although the goal is to have a complete system that can handle all kinds of products and faults, one of the
advantages of this is that groups of experts can develop sub-networks for a specific product. Furthermore,
there is the possibility of providing proof of concept for smaller parts before investing in developing the
whole system.

Evaluating the model is something that is not so straightforward in such cases. In the survey, there is
an even distribution betweenelicitation mediumsbut as an initial evaluation, one could use practition-
ers to compare the model’s decision with domain experts to see if they find it helpful and trustworthy.
Alternatively one could evaluate if the model provides the same decisions as a domain expert.

## 9 Conclusions and future work

Incorporating domain expert knowledge in the pipeline of an ML project has multiple benefits. However,
the process of eliciting this knowledge can often be challenging. To address this, we conducted a survey
of 43 articles that utilized expert knowledge in their ML project pipeline. From this survey, we identified
and analyzed 97 elicitation paths and developed a taxonomy that categorizes these paths based on theML
pipeline,knowledge target,knowledge representation, andelicitation medium.

The main goal of our research was to gain insight into how ML practitioners elicit knowledge, formalize,
and structure that knowledge as well as the motivations and challenges associated with their approach
(seeRQ1andRQ2). Additionally, we examined the trends for the different phases of the ML pipeline.
Through this analysis, we identified and discussed trends found in the survey and discussed the most
prominentchallengesandmotivationsfound across the literature. Finally, based on our survey findings,
we provide suggestions on how to proceed with an industrial case.

However, it is difficult to ensure an accurate representation of the elicitation practices in ML solely from
our work. This is further complicated by the fact that the way elicitation in ML is described varies greatly.
Therefore an obvious path forward is to include more articles in the analysis. Related to this is the spread
over the different knowledge domains, e.g., medicine and physics. One way forward is to see how the
domains’ elicitation approaches for ML differ. Furthermore, we did not look at how well elicitation
approaches worked. Such work could be valuable in guiding towards choosing elicitation approaches.

The level of detail in the content analysis can be extended in many directions. Firstly, there is the possi-
bility of providing more details about the elicitation, e.g., context, validity, and how structured interviews
are. This kind of work has been presented in [13], however, without the structure of the knowledge in
focus.

One approach for future work is to look specifically at the knowledge that is hard to formalize and struc-
ture, such asfeature relationshipandbackground knowledge. It is possible that in a more detailed analy-
sis, such approaches may capture concepts or other typologies.

Furthermore, one could look deeper into the ML pipeline. Our approach focuses on a project perspective,
but one could look into a more detailed approach by dividing the pipeline more. Alternatively, one could
focus on specific pipeline phases for a more extensive analysis. Furthermore, it is arguably hard to define
an ML pipeline that fits all kinds of models and projects. Therefore, a possibility for future work is to
improve the pipeline definition. Alternatively, one could try to define more accurate pipelines for specific
models, i.e., NN or BN.

Another approach for future work is to examine the elicited knowledge’s validity. While it might be
complex, it is nonetheless essential. There are aspects to consider for statistical properties to validate the
knowledge. An example of such things to address is anchoring, mainly when successive judgments are


made about related numerical quantities, where the first judgment acts as an anchor for the second [59].
Another example is availability, where more dramatic or uncommon events seem more likely than they are
[59]. Lastly, overconfidence is that domain experts are generally overconfident in their judgments, which
needs to be addressed [59]. This and many other things could be potential directions to advance in order
to investigate how well ML practitioners address such challenges for statistical properties. However, for
other kinds of knowledge, there need to be other sorts of validation techniques, which in itself could be a
possible direction for future work.

An important topic is improving trustworthiness in ML models, which is an essential motivation for elic-
iting domain expert knowledge. One could dig deeper into this area to highlight the effectiveness of
particular approaches regarding trustworthiness. As previously discussed, this can take many directions,
such as comparing trustworthiness between well-documented elicitation and undocumented elicitation or
including domain expert into the whole ML project. Additionally, one could take the path of explainabil-
ity, observing how trustworthiness is impacted by models that provide explanations for the predictions or
classifications. Alternatively, one could use experts to elicit feedback on how to correct the explanations
for predictions or classifications.

Finally, one could investigate the optimal relations between prior knowledge and data toward producing
the most effective learning algorithms.


## References

```
[1] H. A. Simon, “The new science of management decision.,” 1960.
[2] A. Krizhevsky, I. Sutskever, and G. E. Hinton, “Imagenet classification with deep convolutional
neural networks,”Communications of the ACM, vol. 60, no. 6, pp. 84–90, 2017.
[3] W. Chan, N. Jaitly, Q. Le, and O. Vinyals, “Listen, attend and spell: A neural network for large
vocabulary conversational speech recognition,”
in2016 IEEE international conference on acoustics, speech and signal processing (ICASSP),
IEEE, 2016, pp. 4960–4964.
[4] L. Vonrueden, S. Mayer, K. Beckh,et al., “Informed machine learning - a taxonomy and survey
of integrating prior knowledge into learning systems,”
IEEE Transactions on Knowledge and Data Engineering, 2021,ISSN: 15582191.
DOI:10.1109/TKDE.2021.3079836.
[5] T. Ching, D. S. Himmelstein, B. K. Beaulieu-Jones,et al., “Opportunities and obstacles for deep
learning in biology and medicine,”
Journal of The Royal Society Interface, vol. 15, no. 141, p. 20 170 387, 2018.
[6] L. Torrey and J. Shavlik, “Transfer learning,” inHandbook of research on machine learning
applications and trends: algorithms, methods, and techniques, IGI global, 2010, pp. 242–264.
[7] A. Karpatne, G. Atluri, J. H. Faghmous,et al., “Theory-guided data science: A new paradigm for
scientific discovery from data,”
IEEE Transactions on knowledge and data engineering, vol. 29, no. 10, pp. 2318–2331, 2017.
[8] C. Bauckhage, C. Ojeda, J. Schücker, R. Sifa, and S. Wrobel,
“Informed machine learning through functional composition.,” 2018, pp. 33–37.
[9] S. Sagiroglu and D. Sinanc, “Big data: A review,”
in2013 international conference on collaboration technologies and systems (CTS), IEEE, 2013,
pp. 42–47.
```
[10] L. Cai and Y. Zhu, “The challenges of data quality and data quality assessment in the big data
era,”Data science journal, vol. 14, 2015.

[11] B. Yet, Z. Perkins, N. Fenton, N. Tai, and W. Marsh, “Not just data: A method for improving
prediction with knowledge,”Journal of Biomedical Informatics, vol. 48, pp. 28–37, Apr. 2014,
ISSN: 1532-0464.DOI:10.1016/J.JBI.2013.10.012.

[12] A. Karpatne, W. Watkins, J. Read, and V. Kumar, “Physics-guided neural networks (pgnn): An
application in lake temperature modeling,”arXiv preprint arXiv:1710.11431, vol. 2, 2017.

[13] D. Kerrigan, J. Hullman, and E. Bertini, “A survey of domain knowledge elicitation in applied
machine learning,”Multimodal Technologies and Interaction, vol. 5, p. 73, 12 2021,
ISSN: 2414-4088.

[14] H. Afrabandpey, T. Peltola, and S. Kaski, “Human-in-the-loop active covariance learning for
improving prediction in small data sets,”arXiv preprint arXiv:1902.09834, 2019.

[15] J. Choo, C. Lee, C. K. Reddy, and H. Park, “Utopian: User-driven topic modeling based on
interactive nonnegative matrix factorization,”
IEEE Transactions on Visualization and Computer Graphics, vol. 19, pp. 1992–2001, 12 2013,
ISSN: 10772626.DOI:10.1109/TVCG.2013.212.

[16] P. F. C. OpenAI, J. L. DeepMind, T. B. B. G. Brain, M. M. DeepMind, S. L. DeepMind, and
D. A. OpenAI, “Deep reinforcement learning from human preferences,”
Advances in Neural Information Processing Systems, vol. 30, 2017.


[17] A. C. Constantinou, N. Fenton, and M. Neil, “Integrating expert knowledge with data in bayesian
networks: Preserving data-driven expectations when the expert variables remain unobserved,”
Expert Systems with Applications, vol. 56, pp. 197–208, Sep. 2016,ISSN: 0957-4174.
DOI:10.1016/J.ESWA.2016.02.050.

[18] P. Daee, T. Peltola, M. Soare, and S. Kaski, “Knowledge elicitation via sequential probabilistic
inference for high-dimensional prediction,”Machine Learning, vol. 106, pp. 1599–1620, 2017,
ISSN: 0885-6125.

[19] L. M. de Campos and J. G. Castellano, “Bayesian network learning algorithms using structural
restrictions,”International Journal of Approximate Reasoning, vol. 45, pp. 233–254, 2 2007,
ISSN: 0888-613X.

[20] M. El-Assady, F. Sperrle, O. Deussen, D. Keim, and C. Collins, “Visual analytics for topic model
optimization based on user-steerable speculative execution,”
IEEE transactions on visualization and computer graphics, vol. 25, pp. 374–384, 1 2018,
ISSN: 1077-2626.

[21] M. El-Assady, R. Kehlbeck, C. Collins, D. Keim, and O. Deussen, “Semantic concept spaces:
Guided topic model refinement using word-embedding projections,”
IEEE Transactions on Visualization and Computer Graphics, vol. 26, pp. 1001–1011, 1 2020,
ISSN: 1941-0506.DOI:10.1109/TVCG.2019.2934654.

[22] J. A. Fails and D. R. Olsen, “Interactive machine learning,”
International Conference on Intelligent User Interfaces, Proceedings IUI, pp. 39–45, 2003.
DOI:10.1145/604045.604056. [Online]. Available:
https://dl.acm.org/doi/10.1145/604045.604056.

[23] A. Feelders and L. C. van der Gaag, “Learning bayesian network parameters under order
constraints,”International Journal of Approximate Reasoning, vol. 42, pp. 37–53, 1-2 May 2006,
ISSN: 0888-613X.DOI:10.1016/J.IJAR.2005.10.003.

[24] T. Hester, T. Schaul, A. Sendonaris,et al., “Deep q-learning from demonstrations,”Proceedings
of the AAAI Conference on Artificial Intelligence, vol. 32, pp. 3223–3230, 1 Apr. 2018,
ISSN: 2374-3468.DOI:10.1609/AAAI.V32I1.11757. [Online]. Available:
https://ojs.aaai.org/index.php/AAAI/article/view/11757.

[25] H. Afrabandpey, T. Peltola, and S. Kaski, “Interactive prior elicitation of feature similarities for
small sample size prediction,”UMAP 2017 - Proceedings of the 25th Conference on User
Modeling, Adaptation and Personalization, pp. 265–269, Jul. 2017.
DOI:10.1145/3079628.3079698. [Online]. Available:
https://dl.acm.org/doi/10.1145/3079628.3079698.

[26] R. L. Hu, J. Granderson, D. M. Auslander, and A. Agogino, “Design of machine learning models
with domain experts for automated sensor selection for energy fault detection,”
Applied Energy, vol. 235, pp. 117–128, Feb. 2019,ISSN: 0306-2619.
DOI:10.1016/J.APENERGY.2018.10.107.

[27] J. Hullman and A. Gelman, “Designing for interactive exploratory data analysis requires theories
of graphical inference,”Harvard Data Science Review, vol. 3, 3 2021.

[28] R. Kaplan, C. Sauer, and A. Sosa, “Beating atari with natural language guided reinforcement
learning,” Apr. 2017. [Online]. Available:https://arxiv.org/abs/1704.05539v1.

[29] Y.-S. Kim, L. A. Walls, P. Krafft, and J. Hullman,
“A bayesian cognition approach to improve data visualization,”
Association for Computing Machinery, 2019, pp. 1–14,ISBN: 9781450359702.
DOI:10.1145/3290605.3300912. [Online]. Available:
https://doi.org/10.1145/3290605.3300912.


[30] W. B. Knox and P. Stone, “Interactively shaping agents via human reinforcement: The tamer
framework,”K-CAP’09 - Proceedings of the 5th International Conference on Knowledge
Capture, pp. 9–16, 2009.DOI:10.1145/1597735.1597738. [Online]. Available:
https://dl.acm.org/doi/10.1145/1597735.1597738.

[31] M. von Kurnatowski, J. Schmid, P. Link,et al., “Compensating data shortages in manufacturing
with monotonicity knowledge,”Algorithms, vol. 14, p. 345, 12 2021,ISSN: 1999-4893.

[32] H. Langseth and T. D. Nielsen, “Fusion of domain knowledge with data for structural learning in
object oriented domains,”The Journal of Machine Learning Research, vol. 4, pp. 339–368, 2003,
ISSN: 1532-4435.

[33] M. H. Lee, D. P. Siewiorek, A. Smailagic, A. Bernardino, and S. B. i Badia, “Interactive hybrid
approach to combine machine and human intelligence for personalized rehabilitation assessment,”
2020, pp. 160–169.

[34] A. R. Masegosa and S. Moral, “An interactive approach for bayesian network learning using
domain/expert knowledge,”
International Journal of Approximate Reasoning, vol. 54, pp. 1168–1181, 8 Oct. 2013,
ISSN: 0888-613X.DOI:10.1016/J.IJAR.2013.03.009.

[35] L. Micallef, I. Sundin, P. Marttinen,et al.,
“Interactive elicitation of knowledge on feature relevance improves predictions in small data sets,”
2017, pp. 547–552.

[36] E. E. Altendorf, A. C. Restificar, and T. G. Dietterich, “Learning from sparse data by exploiting
monotonicity constraints,”arXiv preprint arXiv:1207.1364, 2012.

[37] N. Muralidhar, M. R. Islam, M. Marwah, A. Karpatne, and N. Ramakrishnan,
“Incorporating prior domain knowledge into deep neural networks,” 2018, pp. 36–45.
DOI:10.1109/BigData.2018.8621955.

[38] M. Richardson and P. Domingos, “Learning with knowledge from multiple experts,” 2003,
pp. 624–631.

[39] L. Rieger, C. Singh, W. Murdoch, and B. Yu,
Interpretations are useful: Penalizing explanations to align neural networks with prior knowledge,
Nov. 2020. [Online]. Available:https://proceedings.mlr.press/v119/rieger20a.html.

[40] P. Schramowski, W. Stammer, S. Teso,et al., “Right for the wrong scientific reasons: Revising
deep networks by interacting with their explanations,”arXiv preprint arXiv:2001.05371, 2020.

[41] M. Sendak, M. C. Elish, M. Gao,et al.,
“" the human body is a black box" supporting clinical decision-making with deep learning,” 2020,
pp. 99–109.

[42] T. Seymoens, F. Ongenae, A. Jacobs, S. Verstichel, and A. Ackaert, “A methodology to involve
domain experts and machine learning techniques in the design of human-centered algorithms,”
Springer, 2019, pp. 200–214,ISBN: 3030052966.

[43] M. Soare, M. Ammad-Ud-Din, and S. Kaski, “Regression with n→1 by expert knowledge
elicitation,” pp. 734–739, Feb. 2017.DOI:10.1109/ICMLA.2016.0131.

[44] I. Sundin, T. Peltola, L. Micallef,et al., “Improving genomics-based predictions for precision
medicine through active elicitation of expert knowledge,”
Bioinformatics, vol. 34, pp. i395–i403, 13 Jul. 2018,ISSN: 1367-4803.
DOI:10.1093/bioinformatics/bty257. [Online]. Available:
https://doi.org/10.1093/bioinformatics/bty257.


[45] B. Ustun, L. A. Adler, C. Rudin,et al., “The world health organization adult
attention-deficit/hyperactivity disorder self-report screening scale for dsm-5,”
Jama psychiatry, vol. 74, pp. 520–526, 5 2017,ISSN: 2168-622X.

[46] B. Ustun and C. Rudin, “Learning optimized risk scores.,”
J. Mach. Learn. Res., vol. 20, pp. 1–75, 150 2019.

[47] S. Amershi, B. Lee, A. Kapoor, R. Mahajan, and B. Christian,
“Cuet: Human-guided fast and accurate network alarm triage,” 2011, pp. 157–166.

[48] H. Xiao-xuan, W. Hui, and W. Shuo, “Using expert’s knowledge to build bayesian networks,”
2007, pp. 220–223.DOI:10.1109/CISW.2007.4425484.

[49] B. Yet, Z. B. Perkins, T. E. Rasmussen, N. R. M. Tai, and D. W. R. Marsh, “Combining data and
meta-analysis to build bayesian networks for clinical decision support,”
Journal of biomedical informatics, vol. 52, pp. 373–385, 2014,ISSN: 1532-0464.

[50] G. W. Ashdown, M. Dimon, M. Fan,et al., “A machine learning approach to define antimalarial
drug action from heterogeneous cell-based screens,”
Science Advances, vol. 6, eaba9338, 39 2020,ISSN: 2375-2548.

[51] K. H. Bowles, S. Potashnik, S. J. Ratcliffe,et al., “Conducting research using the electronic health
record across multi-hospital systems: Semantic harmonization implications for administrators,”
The Journal of nursing administration, vol. 43, p. 355, 6 2013.

[52] K. H. Bowles, S. Ratcliffe, S. Potashnik,et al., “Using electronic case summaries to elicit
multi-disciplinary expert knowledge about referrals to post-acute care,”
Applied Clinical Informatics, vol. 7, pp. 368–379, 02 2016,ISSN: 1869-0327.

[53] E. T. Brown, J. Liu, C. E. Brodley, and R. Chang, “Dis-function: Learning distance functions
interactively,”IEEE Conference on Visual Analytics Science and Technology 2012, VAST 2012 -
Proceedings, pp. 83–92, 2012.DOI:10.1109/VAST.2012.6400486.

[54] C. J. Cai, E. Reif, N. Hegde,et al.,
“Human-centered tools for coping with imperfect algorithms during medical decision-making,”
2019, pp. 1–14.

[55] T. O. Ayodele, “Types of machine learning algorithms,”
New advances in machine learning, vol. 3, pp. 19–48, 2010.

[56] T. J. Loftus, P. J. Tighe, A. C. Filiberto,et al., “Artificial intelligence and surgical
decision-making,”JAMA surgery, vol. 155, no. 2, pp. 148–158, 2020.

[57] D. Heckerman, D. Geiger, and D. M. Chickering, “Learning bayesian networks: The combination
of knowledge and statistical data,”Machine learning, vol. 20, pp. 197–243, 1995,
ISSN: 0885-6125.

[58] A. Nikitin and S. Kaski, “Decision rule elicitation for domain adaptation,”
in26th International Conference on Intelligent User Interfaces, 2021, pp. 244–248.

[59] A. O’Hagan, “Expert knowledge elicitation: Subjective but scientific,”
The American Statistician, vol. 73, pp. 69–81, sup1 2019,ISSN: 0003-1305.

[60] W. P. Wagner, “Trends in expert system development: A longitudinal content analysis of over
thirty years of expert system case studies,”
Expert Systems with Applications, vol. 76, pp. 85–96, Jun. 2017,ISSN: 0957-4174.
DOI:10.1016/J.ESWA.2017.01.028.

[61] E. E. Altendorf, A. C. Restificar, and T. G. Dietterich, “Learning from sparse data by exploiting
monotonicity constraints,”arXiv preprint arXiv:1207.1364, 2012.


[62] A. J. Myles, R. N. Feudale, Y. Liu, N. A. Woody, and S. D. Brown, “An introduction to decision
tree modeling,”
Journal of Chemometrics: A Journal of the Chemometrics Society, vol. 18, pp. 275–285, 6 2004,
ISSN: 0886-9383.

[[RAW FILES]]

