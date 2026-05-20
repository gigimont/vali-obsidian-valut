```
Phytopathology®  2025  115:1245-1259  https://doi.org/10.1094/PHYTO-06-25-0220-FI
```

### Jacobo Robledo,1,2,3,4,† Aaron I. Plex Sulá,1,2,3,4 Lauren G. Jaworski,1,2,3,4 Romaric A. Mouafo-Tchinda,1,2,3,4,

### Kelsey F. Andersen Onofre,^6 Sara Thomas-Sharma,^7 and Karen A. Garrett1,2,3,4,†

(^1) Plant Pathology Department, University of Florida, Gainesville, FL, U.S.A.
(^2) Institute of Food and Agricultural Sciences, University of Florida, Gainesville, FL, U.S.A.
(^3) Global Food Systems Institute, University of Florida, Gainesville, FL, U.S.A.
(^4) Emerging Pathogens Institute, University of Florida, Gainesville, FL, U.S.A.
(^5) Biopterre - Bioproducts Development Center, La Pocatière, Canada
(^6) Department of Plant Pathology, Kansas State University, Manhattan, KS, U.S.A.
(^7) Department of Plant Pathology & Crop Physiology, Louisiana State University Agricultural Center, Baton Rouge, LA, U.S.A.

#### Accepted for publication 9 September 2025.

### Abstract

```
A vast amount of expert knowledge currently remains inaccessible to digital information systems. Expert knowledge elicitation is a systematic
approach to accessing and synthesizing the insights of subject matter experts, especially when available objective data are incomplete. In plant pathology,
expert knowledge elicitation is valuable for addressing urgent, uncertain, and/or future challenges, such as emerging disease threats, complex epidemi-
ological systems, knowledge gaps when resources are limited, and future scenarios. This perspective explores when expert knowledge elicitation is
most effective for addressing plant health challenges, emphasizing its role in informing timely, expert-based decisions. We discuss lessons learned from
real-world implementations across diverse regions and pathosystems, highlighting strategies for eliciting, structuring, and interpreting expert-derived
data, as well as associated caveats. We frame expert knowledge as a form of big data and outline how existing big-data streams (e.g., remote sensing,
crowdsourced reports, and digital surveillance) can inform expert judgements. Outputs from expert knowledge elicitation can be captured as scalable
datasets (text, tabular, audio, and video) that enable artificial intelligence-supported synthesis. We illustrate how expert knowledge can be integrated
in Bayesian analyses, providing a transparent and rigorous approach to understanding uncertainty and improving inference. Finally, we outline future
opportunities, including integration with artificial intelligence, to scale and strengthen expert knowledge elicitation in support of global plant health.
```
```
Keywords : artificial intelligence, Bayesian update, big data, decision support, epidemic modeling, expert elicitation, expert opinion, future scenarios,
knowledge gaps, natural language processing, prior knowledge
```
†Corresponding authors: J. Robledo; jacoborobledobur@ufl.edu, and

K. A. Garrett; karengarrett@ufl.edu

J. Robledo and A. I. Plex Sulá made equivalent contributions.

Current address of L. G. Jaworski: Department of Entomology and Plant Pathology,
North Carolina State University, Raleigh, NC, U.S.A.

The opinions expressed in this article are those of the authors and do not necessarily
reflect the views of USAID or USDA.

**Funding:** Support was provided by the CGIAR Trust Fund (www.cgiar.org/funders/)
and CGIAR Seed Equal Initiative; Animal and Plant Health Inspection Service
(AP21PPQS&T00C195, AP22PPQS&T00C133); National Institute of Food and
Agriculture (2020-51181-32198, 2022-51181-38242, 2024-51181-43302); and the
United States Agency for International Development (720BHA22IO00136).

### e - X tra:Supplementary material is available online.

The author(s) declare no conflict of interest.

```
Copyright © 2025 The Author(s). This is an open access article
distributed under the CC BY 4.0 International license.
```
## Expert Knowledge Elicitation: Transforming

## Expert Insight into Data

#### In plant pathology, not all knowledge is accessible in digital

#### information systems, such as peer-reviewed publications or pub-

#### lic databases. Experts in plant pathology who, for example, work

#### with growers and perform experiments throughout a region ac-

#### quire extensive knowledge from their field experience and informal

#### observations that often remains unpublished (Fig. 1). The file drawer

#### problem is a common issue across disciplines, where lower prior-

#### ity results are filed away and known only to collaborators (Scherm

#### et al. 2014). Expert knowledge can be thought of as big data based

#### on common “3V” definitions (Kitchin and McArdle 2016; McAfee

#### and Brynjolfsson 2012; Table 1) due to its high volume, velocity

#### of acquisition and updating, and variety of topics (Bargmann and

#### Marder 2013; Bazinet et al. 2023).

#### Big data in plant pathology spans genetic sequence reposi-

#### tories, unstructured text in scientific articles, readings from re-

#### mote sensors (satellites, drones, smartphones), and high-resolution

```
Vol. 115, No. 10, 2025 1245
```

#### meteorological data (e.g., forecasting). Disease-forecasting tools

#### illustrate velocity by processing near-real-time information to sup-

#### port day-to-day decisions (Mueller et al. 2025). Advances in data

#### collection and artificial intelligence can facilitate processing of ex-

#### pert knowledge into structured information for integration with

#### other data types to address key problems in plant pathology. When

#### objective data are scarce, costly, or not readily available in digital

#### form, expert knowledge elicitation is a pathway to access expert

#### knowledge.

#### Considering expert knowledge as big data emphasizes the scale,

#### richness, and rapid updating of human information processing.

#### Humans have substantial long-term visual memory capacity, with

#### experiments reporting storage of detailed representations of thou-

#### sands of images (Brady et al. 2008; Wang et al. 2003). Experts can

#### process visual information rapidly (e.g., plant disease images) and

#### base their opinions on patterns they have observed. In practice, ex-

#### pert knowledge may be updated almost in real time and at regional

#### scales, for example, through scouting and consultations. Thus, ex-

#### perts are aware of a wide range of unpublished information about

#### plant disease accumulated over years of experience.

#### Expert knowledge elicitation (Table 1) is a systematic process for

#### gathering expert knowledge and opinions and synthesizing these

#### perspectives (Hadjigeorgiou et al. 2022). It may address specific

#### system traits, such as yield loss and management adoption rates (po-

#### tentially as model parameters for epidemiological studies), or more

#### strongly subjective judgements, such as preferences and opinions

#### about future scenarios (EFSA Panel on Plant Health (PLH) et al.

#### 2018; Hadjigeorgiou et al. 2022). Expert knowledge is particularly

#### useful when objective data from field, lab, or greenhouse experi-

#### ments are limited (Costa et al. 2017; EFSA Panel on Plant Health

#### (PLH) et al. 2018). As we discuss below, one important aspect of

#### expert knowledge elicitation is incorporation of methods to min-

#### imize the effects of bias and address other challenges inherent to

#### expert judgements.

#### Existing big-data streams inform expert judgments, and better

#### integration can improve elicitation design. For example, satellite

#### or drone imagery could help contextualize expert-estimated rates

#### of pathogen dispersal. Leveraging crowdsourced disease reports

#### and social-media signals can be complementary to expert percep-

#### tions about disease occurrence (Bock et al. 2020; Mahlein 2016).

#### Conversely, expert-elicited information may be transformed into

#### tangible big data, such as audio or video from interviews or text from

#### narrative responses and surveys. This information can be captured

#### using standards currently applied on platforms such as REDCap or

#### Qualtrics and archived for reuse, enabling replication, sensitivity

#### analysis, and meta-analyses (Patridge and Bardyn 2018).

#### The first objective of this Perspective is to synthesize how ex-

#### pert knowledge elicitation has been used in plant pathology and its

#### potential for new applications. The second objective is to review

#### methods in expert knowledge elicitation that provide structured

#### and scalable information while considering the limitations associ-

#### ated with interpreting these data. Third, we illustrate how expert

#### knowledge can be integrated as informative priors (Table 1) or

#### data in a Bayesian update and how updating these priors, as new

#### data become available, supports evidence-based practices. Finally,

#### we consider the future potential for expert knowledge elicitation,

#### including integration with artificial intelligence.

## Expert Knowledge Elicitation in Plant Pathology

## and Other Fields: Uses and Impact

#### Expert knowledge elicitation is an emerging tool in plant pathol-

#### ogy, providing valuable information for decision-making to address

#### plant health issues. Collective expert knowledge is often a primary

#### source of unpublished information that is used for pathogen prior-

#### itization (McRoberts et al. 2016). Expert judgment is commonly

#### used to quantify the risk of the introduction of plant pathogens to

#### a new region (Arndt et al. 2022). In practice, determining priority

#### locations for pathogen surveillance across a region (e.g., a state or

#### province) often depends on the multi-criteria knowledge of experts

#### (Bouwmeester et al. 2023; Etherton et al. 2025; Hughes and Madden

#### 2002).

#### Some studies have highlighted the complementary value of expert

#### assessment in estimating key parameters in epidemiological models

#### (Chen et al. 2019; Hughes and Madden 2002). These applications

#### build on foundational epidemiological frameworks developed for

#### the study of plant disease epidemics (Jeger et al. 2018; Madden et al.

#### 2007). In other cases, decision-support systems for plant diseases

#### have been strengthened or validated through shared expert judgment

#### (Chen et al. 2019; Motisi et al. 2022). Expert knowledge elicitation

#### has helped characterize geographic risk factors that contribute to the

```
New plant health
information sources
```
```
Expert Knowledge
```
```
Plant health Artificial Intelligence (AI)
information sources
```
```
Unpublished information
```
- Unpublished
    observations
- Expert discussions

```
Published information
```
- Digitized experimental
    results
- Digitized opinions and
    syntheses
       **Expert-elicited data**

```
Digitized big data
(e.g., video and audio of
expert statements)
```
```
Expert-elicited
estimates to summarize
expert knowledge
```
```
Synthesis of big data
from experts using AI
```
```
Expert
knowledge
elicitation
```
#### FIGURE 1

Expert knowledge includes knowledge of unpublished observations and discussions that are not generally available as input to syntheses, such as
those from artificial intelligence (AI). Experts may also have valuable opinions about future scenarios. Expert knowledge elicitation is designed to
optimize the quality of data obtained from experts. Expert knowledge elicitation can generate statistical summaries of expert knowledge provided
directly by experts in direct elicitation or can generate video or audio of expert statements in indirect elicitation. AI can be used to synthesize the
results of expert knowledge elicitation and translate the results for different purposes. Expert knowledge can serve as a baseline for decision-making,
which can be improved with information from new experiments.

##### 1246 PHYTOPATHOLOGY®


##### TABLE 1

```
Operational definitions of key terms used in this perspective
```
Term Operational definition (for this paper) Primary role in this paper Related references

Anchoring &
adjustment bias

```
Tendency for estimates to be pulled toward initial
values or cues presented before elicitation
```
```
Instrument design and training Morgan 2014; Tversky
and Kahneman 1974
```
Availability bias Judgments influenced by easily recalled or recent
events rather than base rates

```
Instrument design and interpretation Morgan 2014; Tversky
and Kahneman 1974
```
Balanced expert
assessment

```
Use of diverse, balanced expert panels/procedures
in regulatory assessments
```
```
Policy examples (e.g., EPA guidelines) U.S. Environmental
Protection Agency
2004, 2009, 2024
```
Bayesian hierarchical
prior

```
Prior that shares information across
experts/groups while allowing for group- or
expert-specific parameters
```
```
Modeling heterogeneous experts McGlothlin and Viele
2018
```
Bayesian prior
(informative prior),
prior distribution

```
Probability distribution representing existing
knowledge about a parameter before current
data; “informative” when derived from
substantive knowledge (e.g., from EKE)
```
```
Prior for prevalence and other
parameters
```
```
Hartley and French
2021; O’Hagan 2019
```
Big data “Big data” often refers to datasets that contain a
large amount of data, are rapidly updated, and
potentially span a variety of data types and
topics.
Some big data sets are so large, fast, or complex
that traditional data processing methods are
inadequate.

```
Experts’ minds are an important,
potentially extensive source of diverse
and rapidly updated information.
```
```
Sagiroglu and Sinanc
2013
```
Delphi technique Iterative, anonymous rounds with feedback to
converge/clarify group judgments

```
Group processes and bias mitigation Linstone and Turoff
2011
```
Digital twins Virtual, updateable representations of real systems
that mirror key processes to test scenarios and
visualize implications of parameter choices

```
Communicate to experts how elicited
parameters affect epidemic
dynamics/decisions; support
interactive “what-if” exploration
```
```
Grieves and Vickers
2017; Tao et al. 2019
```
Direct elicitation Experts provide quantities directly used in analysis
(e.g., dates, probabilities).

```
Method option Martin et al. 2012
```
Effective sample size The amount of information a prior contributes,
expressed as the number of data points it is
roughly equivalent to

```
Cap prior influence from expert inputs
so elicited information cannot
dominate new data
```
```
Morita et al. 2008
```
Elicitation instrument Protocols, prompts, and procedures
(survey/interview/workshop) used to collect
expert judgments

```
Design/execution choices and
documentation
```
```
Hemming et al. 2018;
Martin et al. 2012
```
Epistemic uncertainty Uncertainty due to limited knowledge or model
structure; decreases with additional information

```
Rationale for using expert knowledge
elicitation
```
```
Der Kiureghian and
Ditlevsen 2009
```
Expert An individual with demonstrable, peer-recognized
expertise and knowledge relevant to the target
questions (e.g., years of practice, professional
role, regional familiarity), selected according to
prespecified criteria

```
Provides judgments/estimates in expert
knowledge elicitation
```
```
Hemming et al. 2018;
Knol et al. 2010
```
Expert knowledge
elicitation (EKE)

```
Structured process to obtain, quantify, and
synthesize expert judgments as data to inform
decisions under uncertainty
```
```
Data acquisition when empirical data are
sparse/difficult to obtain
```
```
Caley et al. 2014; EFSA
Panel on Plant Health
(PLH) et al. 2018;
Hemming et al. 2018
```
Global sensitivity
analysis

```
Exploring the output response to simultaneous
variation of multiple inputs over their joint ranges
(often variance-based)
```
```
Quantify joint uncertainty propagation
for priors/parameters; identify most
influential assumptions
```
```
Saltelli et al. 2008;
Sobol’ 2001
```
Hierarchical models Statistical models that share information (partial
pooling) across groups/experts while allowing
for group-specific parameters, improving
estimates when data are sparse or
heterogeneous

```
Encode expert-to-expert variability;
borrow strength across
experts/regions in Bayesian updates
```
```
Gelman and Hill 2007
```
IDEA protocol Investigate–Discuss–Estimate–Aggregate:
a structured elicitation workflow

```
Improving reliability of judgments Hemming et al. 2018
```
Indirect elicitation Experts provide judgments (e.g., rankings,
experiences) that analysts transform into
required quantities.

```
Method option Martin et al. 2012
```
Informal seed/planting
material exchange

```
Not formal, i.e., not exchange of certified seed
through registered outlets
```
```
Motivating expert knowledge elicitation
to characterize movement
```
```
McGuire and Sperling
2016; Andersen
Onofre et al. 2021
```
```
(Continued on next page)
```
```
Vol. 115, No. 10, 2025 1247
```

#### spread of plant pathogens (Andersen Onofre et al. 2021; Etherton

#### et al. 2025; Thomas-Sharma et al. 2017).

#### At larger geographic scales, expert knowledge has been used to

#### understand the impacts of plant pathogens on global ecosystems

#### (Acuña et al. 2023; Savary et al. 2019). In policy development,

#### the U.S. Environmental Protection Agency uses balanced expert

#### assessment (Table 1) when reviewing the impacts of insecticides,

#### fungicides, and rodenticides on human health and the environment

#### (U.S. Environmental Protection Agency 2004, 2009, 2024). Expert

#### knowledge elicitation has been applied to support decision analysis

#### across the science of plant health: for a range of plant pathogens,

#### across host plants, and in high-, middle-, and low-income countries

#### (Table 2).

#### Use of expert knowledge elicitation in other disciplines illus-

#### trates the potential for new applications in plant pathology. Many

#### areas of plant pathology can benefit from expert knowledge meth-

#### ods applied in pest biosecurity (EFSA Panel on Plant Health (PLH)

#### et al. 2018). Applications in plant pathology commonly require

#### more data for understanding pathways of transmission, uncertainty,

#### and how to address newly emerging problems. These applications

#### map onto complementary modeling approaches that have differ-

#### ent strengths and data needs (Supplementary Table S1A). Models

#### of human health have used expert knowledge to adjust the mod-

#### eling process for estimating the burden of communicable diseases

#### (Mangen et al. 2013). Conservation biology uses expert knowledge

#### elicitation to address the common need to make decisions with in-

#### complete objective information (Petracca et al. 2018; Runge et al.

#### 2011), an issue for many questions in plant pathology. Expert opin-

#### ions have also helped to characterize the effects of technologies on

#### progress toward the Sustainable Development Goals (Herrero et al.

#### 2021), illustrating the potential for using expert reasoning to eval-

#### uate future scenarios. In agricultural economics, Bayesian updates

#### have been used to integrate objective data with expert opinions and

#### survey data (Mkondiwa et al. 2024). Integrating these data types

#### can help bridge evidence gaps, improve uncertainty quantification,

#### and support more informed decisions.

## When to Use Expert Knowledge Elicitation

## in Plant Pathology

#### Types of uncertainty

#### In general, three key considerations can help plant pathologists

#### determine whether expert knowledge elicitation is useful to address

#### a problem in plant health science (Fig. 2). The first consideration

#### is the level of uncertainty associated with the plant health problem

#### in question. Uncertainty can arise from a relative lack of knowl-

#### edge (epistemic uncertainty; Table 1) or the inherent randomness

##### TABLE 1

```
(Continued from previous page)
```
```
Term Operational definition (for this paper) Primary role in this paper Related references
```
```
Objective data Direct measurements collected with documented,
standardized procedures whose numeric values
do not depend on the observer’s judgment;
independently verifiable and reproducible
```
```
Provides likelihoods and validation
targets (e.g., field-trial
incidence/severity/yield, diagnostic
assay results, surveillance detections,
meteorological records,
remote-sensing indices,
administrative/interception records)
```
```
EFSA Panel on Plant
Health (PLH) et al.
2018; Jeger et al.
2018; Madden et al.
2007
```
```
One-at-a-time
sensitivity analysis
```
```
Varying a single input while holding others fixed to
see its individual effect on outputs
```
```
Quick, interpretable checks of key
assumptions (e.g., prior effective
sample size alone)
```
```
Saltelli et al. 2008
```
```
Performance weighting
(Cooke’s method)
```
```
Weighting experts by calibration and
informativeness on calibration questions
```
```
Aggregation of expert inputs Colson and Cooke
2018; Cooke and
Goossens 2004
```
```
Posterior distribution Updated distribution of a parameter after
combining the prior with observed data
(likelihood)
```
```
Decision-relevant inference after
updating
```
```
Mila and Carriquiry
2004; O’Hagan 2019
```
```
Power prior weight A tuning parameter (0–1) that raises the likelihood
of historical/expert data to a powerδto control
how much those data inform the prior
```
```
Build a hybrid prior that transparently
dials the influence of expert
information; runδsensitivity
```
```
Ibrahim and Chen 2000
```
```
Prior-predictive checks Simulating plausible data from the prior (and
model) to assess whether assumptions could
have generated reasonable observations before
seeing the data
```
```
Screen/eliminate unrealistic priors
before updating with trial data
```
```
Gelman and Shalizi
2013; Gelman et al.
2020
```
```
SEIR model Compartmental epidemic model with
Susceptible–Exposed–Infectious–Removed
states
```
```
Example of stochastic modeling with
elicited inputs
```
```
Li and Muldowney
1995
```
```
Sensitivity analysis Systematically varying inputs/assumptions to
assess their impact on model outputs and
conclusions
```
```
Report robustness of inferences to prior
choices,δ, and model settings
```
```
Oakley and O’Hagan
2004; Saltelli et al.
2008
```
```
Stochastic/aleatoric
uncertainty
```
```
Inherent randomness of the system; not reducible
by more information
```
```
Interpreting variability and modeling Der Kiureghian and
Ditlevsen 2009
Value chain Network of actors and flows (materials/info)
moving planting material/products
```
```
Framing seed movement examples Andersen Onofre et al.
2021
```
```
WAMBS “When to worry and how to Avoid the Misuse of
Bayesian Statistics”— practical guidance and
reporting checklist for Bayesian analysis
```
```
Document modeling choices/diagnostics
and improve transparency/
reproducibility
```
```
van de Schoot et al.
2021
```
##### 1248 PHYTOPATHOLOGY®


##### TABLE 2

```
Where expert knowledge becomes data: representative plant health applications showing what was elicited (e.g., pathogen lists,
detection probabilities, adoption rates, network structures, efficacy and process parameters), why expert knowledge elicitation was
required (scarce/inaccessible objective data, time/budget constraints), at what scale (country to global), and with whom
(panel size/discipline mix), across crops and pathogensa
```
Topic addressed Information acquired

```
Rationale for use of
expert elicitation
```
```
Spatial
coverage
```
```
Experts
included
```
```
Targeted
crop(s)
```
```
Targeted
pathogen(s) Reference
```
Pathogen
categorization

1. A list of quarantine
    pests
2. A list of regulated
    nonquarantine pests

```
There is little published
information about
many new and
invasive pathogens.
```
```
European
Union
```
```
Many experts Many crops Many pathogens EFSA Panel on
Plant Health
(PLH) et al.
2018
```
Pathogen
prioritization

```
A list of select agents
in the United States
of America
```
```
Selecting among tens
of thousands of plant
pathogens is not an
easy task.
```
```
United
States of
America
```
```
Many experts Many crops 12 exotic plant
pathogens
```
```
McRoberts et al.
2016
```
Global plant
health
assessment

1. Plant health status
2. Plant health trends

```
Not specified Global 80 experts 16 plant
systems
```
```
Not pathogen
specific
```
```
Acuña et al. 2023
```
The global
impact of
plant
pathogens

```
Magnitude and
frequency of crop
losses for each
pathogen species
```
```
Accurate quantification
of pathogen impacts
is difficult at a global
scale.
```
##### 67

```
countries
```
```
219 experts 5 major
crops
```
```
137 pests and
pathogens
```
```
Savary et al.
2019
```
An integrated
seed health
strategy

1. Seed exchange
    between
    stakeholders
2. Adoption rates of
potato varieties
3. Estimates of disease
prevalence

```
Disease reports were
sporadic, and
pathogen distribution
remains
understudied.
```
```
Republic of
Georgia
```
```
15 experts Potato 6 diseases Andersen Onofre
et al. 2021
```
Seedborne
pathogen
movement
through seed
systems

1. Characterization of
    seed trade networks
2. Characterization of
farmer
communication
networks

```
There were no formal
reports on the
geographic exchange
of seed and
information.
```
```
Ethiopia 20 experts Potato Bacterial wilt
(Ralstonia
solanacearum
phylotype II
sequevar 1)
```
```
Etherton et al.
2025
```
Mapping
continental
risk of a
disease

```
Vulnerability scores for
```
1. DominantMusa
    genotype
2. Altitude
3. Temperature
    variability
4. Precipitation
5. Connectivity to
    infected areas
6. Distance to infected
    areas

```
The importance of each
risk factor was not
available on the
continental scale.
```
```
Africa Not specified Bananas Banana bunchy
top disease
```
```
Bouwmeester
et al. 2023
```
Cluster sampling
for disease
incidence

```
Estimation of sample
size
```
```
The anticipated value
of the targeted
parameter is usually
unknown.
```
```
Not
applicable
```
```
1 hypothetical
expert
```
```
Not
applicable
```
```
Not applicable Hughes and
Madden 2002
```
Advisory system
for fungicide
application

```
Estimates for the date
of initial symptom
appearance
```
```
Weekly scouting of
symptoms by every
farmer is
time-consuming.
```
```
France 29 experts Grapes Grape downy
mildew
(Plasmopara
viticola)
```
```
Chen et al. 2019
```
Validation of a
forecasting
tool
(ExpeRoya)

```
Estimates for the
efficacy of
```
1. Fungicides
2. Spore dispersal
3. Spore wash-off
4. Infection
5. Leaf emergence
6. Latent period

```
Scattered published
knowledge of a
complex
pathosystem
```
```
Central
America
```
```
17 experts Coffee Coffee leaf rust
(Hemileia
vastatrix)
```
```
Motisi et al. 2022
```
Early warning of
pathogen
incursions

```
Probability of disease
detection
```
```
Budget constraints:
Direct detection
experiments are
expensive for every
disease.
```
```
Australia
(Victoria)
```
```
157 experts 11 grain
crops
```
```
14 exotic pests
and diseases
```
```
Arndt et al. 2022
```
```
(Continued on next page)
```
```
Vol. 115, No. 10, 2025 1249
```

#### in a system or process (stochastic/aleatoric uncertainty; Table 1)

#### (Der Kiureghian and Ditlevsen 2009). Both types of uncertainty

#### are often an issue for questions in plant pathology. One source of

#### epistemic uncertainty is confounding factors. For example, when

#### assessing the use of a fungicide for disease management, it is diffi-

#### cult to have full knowledge about the trade-offs of economic risks

#### and environmental risks, such as fungicide resistance development

#### (U.S. Environmental Protection Agency 2004, 2009). Another key

#### example of epistemic uncertainty is limited information about the

#### informal trade of planting material in a region (informal planting

#### material exchange; Table 1; Andersen Onofre et al. 2021; Etherton

#### et al. 2025; Mouafo-Tchinda et al. 2024). Informal trade is currently

#### difficult to track through objective approaches in most countries.

#### Stochastic uncertainty is generated by system elements that are in-

#### herently difficult to predict. Examples include weather conditions

#### years in the future that will influence epidemics or yield losses at a

#### national or global scale (Savary et al. 2019).

#### Expert knowledge elicitation can support decision-making when

#### there is a substantial degree of uncertainty in the target problem.

#### If a problem is too uncertain, experts may lack sufficient relevant

#### information to address it (Morgan 2014). For example, accurately

#### anticipating the timing and geographic location for the introduction

##### TABLE 2

```
(Continued from previous page)
```
```
Topic addressed Information acquired
```
```
Rationale for use of
expert elicitation
```
```
Spatial
coverage
```
```
Experts
included
```
```
Targeted
crop(s)
```
```
Targeted
pathogen(s) Reference
```
```
Risk
assessment
of seed
degeneration
```
```
Estimated adoption
rates of
management options
```
```
Limited information
was available for
low-income countries
```
```
Africa and
India
```
```
25 experts Banana,
cassava
```
```
Not pathogen
specific
```
```
Thomas-Sharma
et al. 2017
```
```
National risk
assessment
```
```
Estimates for
```
1. Crop yield losses
2. Certified seed use
3. Informal seed
    movement
4. Information exchange

```
Nationwide estimates
of each factor were
not available from
formal reports.
```
```
Pakistan 28 experts Bread
wheat
```
```
33 diseases and
pests
```
```
Plex Sulá et al.
2025
```
```
Policy
effectiveness
assessment
```
```
Estimates for
```
1. Movement of
    planting material
2. Movement of
    personnel

```
Nationwide estimates
of each factor were
not available from
formal reports.
```
```
Colombia 127 experts Bananas Fusarium wilt
(Fusarium
oxysporumf.
sp.cubense
tropical race 4)
```
```
J. Robledo,
M. Betancourt,
and K. Garrett,
unpublished
data
aThese cases span categorization/prioritization, global burden estimation, seed-system epidemiology, risk mapping, sampling design, forecasting
tool calibration/validation, early warning, and national policy evaluation.
```
### How uncertain is the target

### problem in plant health science?

### Are there resource constraints

### that hinder new data

### collection through gold standard

### technologies?

### How limited is available objective

### data in time and spatial extent?

```
There is enough uncertainty to
motivate expert elicitation
```
```
Uncertainty is not so high that
experts lack useful knowledge
```
### Expert knowledge elicitation is

### appropriate for addressing this

### problem

#### Ye s

```
Objective data are incomplete
```
```
Experts can provide estimates
for the required information
```
```
The target problem is
either already well-
resolved or is too
uncertain
```
### Not suitable for

### expert elicitation

```
Objective data can be
accessed
```
### Existing data can be

### analyzed without the

### need for expert

### knowledge elicitation

#### No

### Suitable for

### conventional data-

### acquisition tools

```
Expert knowledge elicitation
can inform targeting of other
data collection
```
#### FIGURE 2

The greatest value of expert
knowledge elicitation in plant
pathology lies in situations in which an
uncertain problem has incomplete
objective data, and resource
constraints make it difficult to acquire
data through gold-standard
technologies as part of new field, lab,
or greenhouse studies.

##### 1250 PHYTOPATHOLOGY®


#### and establishment of a new pathogen species in a country is a par-

#### ticularly complex problem; the utility of expert opinion may be

#### limited in the face of such high uncertainty. However, biosecurity

#### experts might have unpublished information about geographic fac-

#### tors driving general introduction patterns of plant pathogens at a

#### particular location (a less uncertain problem) and good foundational

#### knowledge of pathogen biology. This expert knowledge could pro-

#### vide valuable information for addressing the problem. If solving

#### a problem depends on information that is already certain or read-

#### ily predictable, tools other than expert elicitation can address the

#### problem using available information.

#### Data availability

#### A second consideration is whether objective data are currently

#### lacking or digitally inaccessible (Fig. 2). For example, a practical

#### issue in plant pathology is the prioritization of pathogen species

#### in biosecurity programs to prevent introduction and establishment

#### in a country. How do policymakers effectively establish priori-

#### ties quickly if essential epidemiological information is typically

#### lacking for new pathogens? Similarly, when addressing large, com-

#### plex systems, such as value chains (Table 1) or landscape-scale

#### cropping systems, objective data may not exist, may be sparse,

#### and may be difficult to combine in models lacking interoperabil-

#### ity. Expert knowledge elicitation can serve as a quick approach to

#### acquiring this relevant information in a structured format, using

#### proven methodologies for data collection, calibration, and analysis

#### (Aspinall and Cooke 2013; Morgan 2014). Another useful out-

#### come from expert elicitation can be identifying which information

#### needs to be collected through objective data-acquisition tools in the

#### long term.

#### Cost-effectiveness

#### A third consideration is the cost-effectiveness of expert knowl-

#### edge elicitation given resource constraints. Plant pathologists have

#### used expert knowledge elicitation when acquiring data with gold-

#### standard technologies is challenging (e.g., when implementing new

#### field experiments is not practical). For example, expert elicita-

#### tion has been applied in African agricultural systems, where the

#### first quantitative comparisons of organic and conventional agricul-

#### ture performance were done using expert input (Andriamampianina

#### et al. 2018). Expert elicitation can serve as a relatively rapid data-

#### acquisition tool when these other technologies are too costly (Arndt

#### et al. 2022), time-consuming (Chen et al. 2019), or not feasible

#### (e.g., quickly documenting informal exchange of planting mate-

#### rial; Andersen Onofre et al. 2021). Expert elicitation methods may

#### be difficult to standardize, and field-specific protocols are scarce.

#### However, methodological adaptations based on time, budget, and

#### locational constraints are available (Hemming et al. 2018). Soft-

#### ware such as Elicitator (James et al. 2010) can make analyses more

#### straightforward. In general, open-source software can streamline

#### elicitation protocols, data collection, and processing, which are key

#### in time-sensitive situations (Aspinall and Cooke 2013; Knol et al.

#### 2010). However, expert knowledge elicitation alone is inappropri-

#### ate for providing definitive evidence to address a new biological

#### hypothesis, such as satisfying Koch’s postulates or confirming the

#### presence of a pathogen species in a new country.

#### Expert knowledge elicitation is generally cost-effective for ad-

#### dressing problems in plant pathology where substantial uncertainty,

#### lack of objective data, and resource constraints converge, especially

#### when information is needed quickly. Expert knowledge elicitation

#### offers additional benefits beyond data collection. When experts in-

#### teract directly, such as drawing experts together in meetings, expert

#### elicitation can facilitate interactions that may develop into future

#### projects, encourage the creation of collaboration networks, develop

#### innovative ideas, and foster knowledge transfer across domains.

#### There are opportunities to better integrate expert elicitation with

#### existing big-data resources (e.g., remote sensing layers or gridded

#### weather data), which may increase cost-effectiveness. Expert elic-

#### itation can also be integrated with epidemiological frameworks by

#### considering precision, scalability, interpretability, and data require-

#### ments; Supplementary Table S1A summarizes these trade-offs to

#### support method choice.

## How Expert Knowledge Is Collected and Translated

## into Usable Data

#### There are generally four steps to conducting expert knowledge

#### elicitation: (i) defining the project objectives and determining what

#### data to elicit to meet them, (ii) designing the elicitation process,

#### (iii) implementing the elicitation, and (iv) translating the data ob-

#### tained into quantitative information to inform decision-making

#### (Martin et al. 2012). The first step is to define the purpose of the

#### information gathered through elicitation. The kind of data to be ob-

#### tained, the nature of the models used, and decisions to be made will

#### determine whether a research question warrants the use of expert

#### knowledge elicitation. Information elicited from experts is most

#### useful when it improves the performance of the model or decision

#### being made (Bojke et al. 2021).

#### The second step is to determine the specific type of informa-

#### tion required, for example, by choosing models or parameters,

#### and approaches to quantifying uncertainty. At this stage, research

#### organizers formulate the questions experts will answer. It is impor-

#### tant to include in the organizational team an array of end users,

#### such as modelers and people knowledgeable about the system be-

#### ing targeted. This team will discuss the data format and use in

#### a model/decision, as well as alignment with the resources avail-

#### able for processing data and modeling. This team also selects and

#### invites experts to participate in the expert knowledge elicitation,

#### considering factors such as expert reputation, experience, publi-

#### cation record, and availability (Bojke et al. 2021). The European

#### Food Safety Authority (2014) describes an expert as being some-

#### one whose judgement is deemed worth eliciting. In expert knowl-

#### edge elicitation, supporting plant pathology, experts may come

#### from complementary fields such as crop breeding, economics, and

#### entomology.

#### The third step involves choosing or designing an elicitation instru-

#### ment, including methods for measuring uncertainty and processing

#### data. The European Food Safety Authority (2014) provides an in-

#### depth discussion of the design, implementation, and aggregation

#### of elicited information. There are two common approaches to data

#### collection. In direct elicitation (Table 1), experts are asked to com-

#### municate knowledge in terms of quantities that will be used by the

#### analyst. For example, experts directly provided estimates for the

#### onset date of initial symptoms of grape downy mildew in France

#### (Chen et al. 2019). In indirect elicitation (Table 1), experts pro-

#### vide personal opinions or describe experiences, which the analyst

#### processes to derive the needed quantities (Martin et al. 2012). For

#### example, experts characterized potato seed exchange networks in

#### Ethiopia, which were later used to simulate the potential spread of

#### seedborne pathogens (Etherton et al. 2025). Modeling the move-

#### ment of informal seed would often be impractical without expert

#### input (McGuire and Sperling 2016).

#### Elicitation methods exist on a spectrum of synchronicity and

#### expert engagement, from asynchronous email surveys of experts to

#### individual interviews to group discussions. More direct interactions

#### with experts, whether in person or by phone, are more resource-

#### intensive than emails or premade surveys. Protocols such as the

#### Delphi technique and Cooke’s model have the potential to provide

#### concise answers to time-sensitive or high-risk issues, such as in the

#### management of invasive pathogens and biosecurity decisions (Table

#### 1). The European Food Safety Authority (2014) and Soares et al.

#### (2024) provide a detailed comparison of the protocols discussed

#### below. Similar procedures with some additional steps to emphasize

```
Vol. 115, No. 10, 2025 1251
```

#### systematic preparation, customization to the problem, and trans-

#### parency of outcomes have been developed in environmental health

#### research (Knol et al. 2010). Facilitators and developers of elicitation

#### questions must have a clear idea of how the data they are collect-

#### ing will be encoded and analyzed, as this strongly influences the

#### choice of methodology, the software used, and the structure of the

#### questions (Martin et al. 2012).

#### The Delphi technique is often used to reach a group consen-

#### sus by pooling inputs after experts hear the anonymized opinions

#### of other experts and update their individual responses accordingly

#### (Linstone and Turoff 2011), without personal identifiers to influence

#### judgements. It is often applied with an equal-weighting aggregation

#### rule (European Food Safety Authority 2014; McBride et al. 2012).

#### The Delphi technique may be most useful for discussion of com-

#### plex questions, accentuating differing viewpoints while gathering

#### knowledge to generate a clearer answer than what individual experts

#### might provide alone (Linstone and Turoff 2011).

#### Cooke’s model is an individualistic approach that limits expert

#### interaction to training and briefing (European Food Safety Author-

#### ity 2014). Cooke’s model involves weighting experts’ judgements

#### based on the quality of answers to a set of calibration questions

#### (Cooke 1991). An important advantage of this model is that it al-

#### lows for validation (European Food Safety Authority 2014), because

#### the approach to mathematical aggregation is auditable and objec-

#### tive. This model is also supported by readily accessible software,

#### such as the Excalibur package (Boutry et al. 2023) and ANDURYL

#### Python-based code (Pieter’t Hart et al. 2019).

#### The IDEA (Investigate, Discuss, Estimate, and Aggregate) pro-

#### tocol is a variation of the Delphi technique to provide a reproducible

#### expert elicitation for estimating probabilities and quantities, orig-

#### inally intended to improve biosecurity decisions (Hemming et al.

#### 2018). The discussion portion of this protocol promotes linguistic

#### clarity, critical thinking, and evidence sharing, rather than empha-

#### sizing a group consensus (Hemming et al. 2018). Wittmann et al.

#### (2015) provide an example of the IDEA protocol used to forecast

#### carp invasions in Lake Erie based on expert judgments.

#### The Sheffield elicitation framework (SHELF) uses behavioral ag-

#### gregation to reach a consensus distribution (Gosling 2018; Williams

#### et al. 2021). SHELF focuses on variable and fixed interval methods

#### for expert elicitation and is compatible with Bayesian applications.

#### SHELF has a corresponding R package for fitting distributions

#### and illustrating expert judgements in real time during discussions

#### (Gosling 2018; Soares et al. 2024).

#### After implementing the elicitation, making sure all questions are

#### clear to the experts, the last step is the translation of the elicited

#### knowledge into quantitative information to inform decision-making

#### or modeling. A common goal of expert knowledge elicitation is

#### integration of data types. For example, expert-based parameter es-

#### timates can be combined with epidemiological models (Etherton

#### et al. 2025; Motisi et al. 2022). Supplementary Table S1A syn-

#### thesizes how expert-elicited information contributes to priors, pa-

#### rameters, constraints, and validation across Bayesian, mechanistic,

#### and machine-learning frameworks. Daee et al. (2017), Martin et al.

#### (2005), and Rose et al. (2023) exemplify key applications of these

#### frameworks when combined with expert elicitation, highlighting

#### more opportunities for plant pathology. Notably, artificial intel-

#### ligence (e.g., transformer-based sentence embeddings and large

#### language models [LLMs]) provides innovative ways of coding

#### narrative responses, clustering themes, and linking qualitative ra-

#### tionales to quantitative parameters (Bojanowski et al. 2017; Devlin

#### et al. 2019; Gemini Team Google 2025). Interactive machine learn-

#### ing offers additional opportunities to integrate expert feedback

#### loops with model refinement (Daee et al. 2017). Capturing expert

#### elicitation outputs as digital artifacts (audio or video of group dis-

#### cussions, verbatim transcripts, structured survey exports) is key to

#### accelerating this integration (Fig. 1). Digitization of expert knowl-

#### edge enhances replicability and audit trails, evaluation of variability

#### between responses and origin of disagreements, and identification

#### of systematic bias.

## Mitigating Bias and Assessing the Quality

## of Expert Knowledge

#### Expert-elicited knowledge may be subject to several cognitive

#### biases (Morgan 2014). For example, anchoring-adjustment bias oc-

#### curs when experts are shown potential answers to the questions

#### being asked, such as mentioning the potential yield loss levels before

#### experts respond. Experts’ estimates may be directly influenced by

#### these initial values (anchoring) (Tversky and Kahneman 1974). To

#### reduce this issue, questions can be structured in a non-leading way,

#### beginning by asking for values in terms of extremes or in relation to

#### one another, rather than the best value (Morgan 2014). Anchoring

#### is an important consideration in structuring expert knowledge elic-

#### itation, because experts will likely be influenced by the phrasing of

#### questions and influenced if they hear the responses of other experts

#### before formulating their own responses. Structured elicitation case

#### studies confirm that these biases are common in practice but can be

#### mitigated through formal design. The quality of expert information

#### may be improved when experts review each other’s estimates and

#### revise their judgments (McBride et al. 2012).

#### Availability bias occurs when experts provide a judgement or

#### probability based on how easily they can recall relevant occurrences

#### or information (Tversky and Kahneman 1974). More recent or im-

#### pactful events are relatively more available in experts’ memory,

#### which may influence experts’ answers in relation to timing, abun-

#### dance, or occurrence of certain pathogens. Availability bias should

#### be considered when developing instruments to avoid overlooking

#### relevant information (Tversky and Kahneman 1974).

#### In plant pathology, selection bias may emerge when experts

#### disproportionally represent specific geographic regions within a

#### country. For some topics, there might be overrepresentation of ex-

#### perts from temperate, high-income regions and underrepresentation

#### of the tropics (Kowal et al. 2022). Experts may be less familiar with

#### the early stages of an epidemic and its dynamics, resulting in incom-

#### plete observations of the system (Battiston et al. 2021; Glennon et al.

#### 2021). Selection bias can be partially mitigated using approaches

#### such as structured recruitment for stratified sampling with pre-set

#### quotas for experts in key subgroups and/or using weighting of ex-

#### pert responses so experts from groups that better match information

#### needs (or have lower error) carry more influence (Bird and King

#### 2018; O’Hagan 2019). Storing full elicitation traces (timestamps,

#### item order, rationales) and linking them to external big-data co-

#### variates (e.g., contemporaneous weather anomalies) can also help

#### diagnose availability.

#### Expert overconfidence is common across expert knowledge elic-

#### itation (McKenzie et al. 2008; Morgan 2014). Several potential

#### explanations include anchoring, experts’ perceived pressure to give

#### precise response ranges to fulfill their role as experts, and an instinc-

#### tive reliance on experts’ individual “short-cut” heuristics (O’Hagan

#### 2019).

#### Because experts vary in their level of knowledge, analysis of data

#### from expert knowledge elicitation can weight the responses of ex-

#### perts based on some measure of their knowledge. One approach to

#### this is to weight expert responses by each expert’s years of expe-

#### rience working on the topic being addressed. Another option is to

#### ask experts to rate their confidence in each response, though imple-

#### menting this effectively demands extra time from experts. A better

#### approach, when practical, may be to assign weights to responses

#### based on the expert’s performance on a set of calibration questions

#### in their area of expertise for which the answer is already known

#### (Cooke and Goossens 2004). However, finding appropriate calibra-

#### tion questions is challenging: the questions must be relevant enough

##### 1252 PHYTOPATHOLOGY®


#### to the topic targeted by the elicitation to indicate expert knowledge

#### yet different enough that they do not influence the elicited answers.

## Balancing Challenges and Opportunities

## for Expert Knowledge Elicitation

#### As discussed above, there are a number of challenges to im-

#### plementation of expert knowledge elicitation. In the worst-case

#### scenario, there may be no adequate experts who can provide the

#### information desired, so the results of expert knowledge elicitation

#### would be misleading if there are not adequate checks on data quality

#### (Morgan 2014; O’Hagan 2019). Distinguishing between stochastic

#### and deterministic components in a system can help address aleatoric

#### uncertainty (stochasticity, or inherent system variability), such as

#### in weather-driven epidemics or long-distance pathogen dispersal.

#### Examples include eliciting conditional probabilities (e.g., infection

#### rates given environmental conditions) or using elicited inputs in

#### stochastic models, such as weather-dependent SEIR (Susceptible–

#### Exposed–Infectious–Removed) frameworks (Table 1) (Xiao et al.

#### 2022). Reporting uncertainty intervals (e.g., 5th/50th/95th per-

#### centiles) instead of point estimates also helps to capture variability

#### (Rongen et al. 2024). Bayesian probabilistic sensitivity analysis

#### can systematically evaluate how uncertainty in elicited parameters

#### propagates through complex models (Oakley and O’Hagan 2004).

#### Expert knowledge elicitation can be resource-intensive, requiring

#### travel, coordination, and extensive data processing (Grigore et al.

#### 2017). Remote elicitation techniques, modular instruments, and

#### digital platforms can alleviate these constraints, in addition to sup-

#### porting reproducibility and streamlining data workflows (Grigore

#### et al. 2017). We provide a comparison of different frameworks that

#### can be combined with expert knowledge elicitation, considering

#### available data, desired interpretability, and computational capacity

#### (Supplementary Table S1A). To scale up expert knowledge into big

#### data, communities will need information systems with reproducible

#### protocols, role-targeted access, and sufficient storage for mixed data

#### types (audio, video, text, and tabular). General data-collection tools

#### (e.g., REDCap, Qualtrics, and SurveyMonkey) can be adapted to

#### capture expert group discussions, geospatial inputs, and uncertainty

#### quantiles. Exporting data in machine-readable formats (e.g., CSV,

#### JSON, and raster) will increase compatibility with Bayesian updates

#### and artificial intelligence models.

## A Bayesian Framework for Combining

## Expert-Elicited and Objective Data

#### Bayesian updating (Table 1) provides a structured and transpar-

#### ent framework for integrating expert knowledge with other forms of

#### data (Garrett et al. 2004; Ikorasaki and Akbar 2018; Kuhnert et al.

#### 2010; Mila and Carriquiry 2004; Yuen and Hughes 2002) (Fig. 3).

#### Bayesian updating is a useful option in several structured elicita-

#### tion approaches (Supplementary Table S1A and B), often applied

#### when decisions have significant economic implications or regula-

#### tory impact. A distinctive characteristic of Bayesian statistics is

#### that parameters are explicitly treated as having a probability distri-

#### bution. A Bayesian update starts with a prior probability distribution

#### (Bayesian prior; Table 1) for the parameter of interest that represents

#### existing information (such as expert knowledge and/or previous ob-

#### jective results). The prior distribution is updated when new data

#### become available, obtaining the posterior distribution (Supplemen-

#### tary Table S1A) (van de Schoot et al. 2021). New data may come

#### from objective measurements (e.g., a pilot trial) or from new expert-

#### elicited data. For example, experts may define the prior distribution

#### that is later updated by field data. Another example is when existing

#### maps or model outputs serve as the Bayesian prior that experts later

#### refine (Mkondiwa et al. 2024; Rosace et al. 2025).

#### Defining the parameter of interest is the starting point of this

#### workflow (Fig. 3). In the example below, field efficacy is a parameter

#### denoted asθand represents the probability that a farm using recom-

#### mended biosecurity methods remains uninfected during a 30-day

#### period. The posterior distribution combines the prior distribution of

#### θwith evidence from new observations.

#### Multiple approaches can be used to answer this type of research

#### question, but Bayesian updating provides key advantages to effi-

#### ciently integrate a mathematical framework with expert knowledge.

#### Bayesian statistics combines multiple information sources: expert

#### knowledge and objective data. It explicitly measures uncertainty in

#### terms of intervals, not just point estimates. It can adjust the influence

#### of expert input, which is useful when sample sizes are small or con-

#### ditions differ between regions. However, Bayesian updating may

#### have limitations when applied in risk analysis, and complementary

#### perspectives may be needed to adequately capture some broader

#### dimensions of uncertainty (Aven 2020). Bayesian approaches are

#### one option in a broader decision process.

#### As an example, when local field data are absent, expert judg-

#### ment can serve as data in the form of encoded structured responses,

#### and, where relevant, hierarchical models (Table 1) can account for

#### expert-to-expert differences. A simple cap for the effective sample

#### size (ESS; Table 1) keeps expert input from overpowering the anal-

#### ysis, managing how strongly expert data can influence the analysis.

#### Prior-predictive checks (Table 1) then simulate plausible trial re-

#### sults from the prior to assess whether the prior produces reasonable

#### outcomes (Fig. 3). These steps (encoding, ESS caps, and prior-

#### predictive checks) are illustrated in a supplementary notebook for

#### a hypothetical example simulation (https://github.com/jrobledob/

#### Expert_Elicitation_in_Plant_Pathology).

#### When new data become available, the same expert information

#### can be blended into the prior and then updated with the new ob-

#### servations. In this example, a power prior weight (Table 1),δ,a

#### dial ranging from 0 to 1, determines how much influence the expert

#### information has in the hybrid prior (δ=0 ignores experts;δ= 1

#### weights them fully). Varyingδin a sensitivity analysis (Table 1)

#### enables a transparent evaluation of the impact of expert assump-

#### tions while allowing for adjustments (Fig. 3). Thisδweighting and

#### the update steps are demonstrated inhttps://github.com/jrobledob/

#### Expert_Elicitation_in_Plant_Pathology.

#### When priors are neutral or well-calibrated and sample sizes are

#### modest, Bayesian intervals forθare expected to align with fre-

#### quentist intervals, allowing for comparison between these statistical

#### approaches (Bayarri and Berger 2004). The Bayesian route pro-

#### vides the ability to formally include expert information, quantify

#### its influence, and retain and update it as more data accumulate.

#### The example uses hierarchical structures when experts differ

#### (partial pooling rather than treating each expert as identical), runs

#### prior-predictive checks to avoid unrealistic priors, and conducts

#### both one-at-a-time (Table 1) and global (Table 1) sensitivity analy-

#### ses as good practices. It also follows WAMBS-style (When to worry

#### and how to Avoid the Misuse of Bayesian Statistics) guidance to

#### document choices and diagnostics. All technical details (formulas,

#### priors,θsummaries,δweights, and diagnostics) of this workflow

#### are provided inhttps://github.com/jrobledob/Expert_Elicitation_

#### in_Plant_Pathology. Similar workflows have been developed in re-

#### lated agricultural and ecological decision contexts (Kuhnert et al.

#### 2010; Mkondiwa et al. 2024).

#### Hypothetical example of Bayesian analysis

#### Consider the scenario of an invasive pathogen in a new region in

#### the tropics, where the national plant protection organization needs

#### to formulate a strategy, but objective data in the country are not

#### available yet. Expert knowledge elicitation provides a structured

#### way to capture informed expectations about the likely performance

#### of biosecurity measures, accounting for local conditions. For exam-

#### ple, local experts may evaluate the likely effectiveness of biosecurity

```
Vol. 115, No. 10, 2025 1253
```

#### practices in tropical areas by considering field results from temper-

#### ate regions in which the pathogen is already present, taking into

#### account local factors, such as climate or management constraints,

#### that could modify how biosecurity practices perform in the new

#### location in the tropics.

#### To formalize such expert judgments, they can be incorporated

#### into a Bayesian workflow designed to evolve as new evidence be-

#### comes available (Fig. 3). The process begins with an informative

#### and adaptable prior distribution for field efficacy (θ), defined here

#### as the probability that a farm implementing biosecurity procedures

#### remains uninfected over a given period. This prior distribution is

#### based on studies conducted in temperate regions and is represented

#### as a beta distribution with moderate strength. This prior nudges but

#### does not dominate; in the code, this influence is the prior ESS=

#### α+β, where a larger ESS produces a stronger nudge. We deliber-

#### ately build in extra uncertainty, keeping the prior flexible, because

#### transportability of the prior from temperate to tropical contexts is

#### imperfect.

#### In the absence of experimental trials in the tropical region, expert

#### judgments can be used as small pseudo-trials, in which the num-

#### ber of expert observations corresponds to confidence levels (low,

#### medium, or high). For example, 30 observations might represent

#### a high-confidence judgment, whereas 10 might correspond to low

#### confidence. To prevent expert opinion from over-influencing anal-

#### ysis outcomes, explicit caps can be placed on the total number of

#### pseudo-trials included in the model. Hierarchical modeling can also

#### be used to account for differences between individual experts, where

#### the influence of each expert’s estimate is set to the mean influence of

#### an expert group, so no single outlier drives the result. This approach

#### yields a posterior distribution for field efficacy (θ) that is informative

#### for decision-making and can be checked for plausibility using prior-

#### predictive simulations (simulating multiple trials from the prior to

#### Scenario B: Expert judgment as

#### prior and objecve data as

#### likelihood

- Expert only prior (or hybrid
    expert and transportable prior)
    + objecve data
- Power prior (δ) applied to EKE
- Update with y, n → posterior

#### Define θ and decision to be made

- Endpoint and me frame
- Success metric and context

#### Obtain transportable prior

#### (if available)

- P(θ) from analog evidence or literature
- Adjust prior strength and note assumpons

#### Expert knowledge elicitaon (EKE)

- Structured judgments become data
- Hierarchical expert input constrained by ESS cap

#### Scenario A: Transportable

#### prior and expert judgment

#### as likelihood

- EKE used to esmate
    posterior

#### Scenario C: Noninformave

#### prior and objecve data as

#### likelihood

- Bayes noninformave priors
- Frequenst confidence
    intervals (CIs)

```
Sensivity analysis
```
- Vary k, δ, ESS, model, etc.
- Check uncertainty
- PPC+ WAMBS checks

#### Iterate

- Update priors and hierarchy
- Plan new data collecon

#### FIGURE 3

Workflow illustrating scenarios for combining expert elicitation with Bayesian updating. **Step 1** defines the decision and endpoint (e.g., field efficacy
(θ) is the probability a treated farm remains uninfected during the assessment window). **Step 2** specifies a transportable prior P(θ) based on evidence
(i.e., a prior relevant across multiple contexts) and adjusts the strength of the prior (e.g.,kfor a beta prior beta(α,β), wherek=α+βreflects the
prior’s effective sample size [ESS]). **Step 3** elicits expert knowledge and models expert variability with a hierarchical model (e.g., partial pooling
across experts), including calibration and ESS safeguards (ESS reflects the informational weight assigned to the expert input). Three scenarios can
be considered depending on the availability of data. **Scenario A** updates the prior with expert knowledge treated as data (e.g., when no local trials
exist). **Scenario B** forms a hybrid prior by discounting expert information (e.g., with a power prior weightδ∈[0,1]: higherδ=more weight given
to expert input) and then updates with objective data (e.g.,ysuccesses out ofntreated units). **Scenario C** provides a data-only baseline (without
expert knowledge), using a Bayesian noninformative prior (e.g., beta(1,1)) and/or frequentist confidence intervals (CIs) (e.g., Wilson/exact). In **Step 4,**
uncertainty and robustness are evaluated via sensitivity analyses (e.g., sensitivity acrossk,δ, ESS, and modeling choices), prior-predictive checks
(PPCs) (simulating plausible data from the prior), and WAMBS (When to worry and how to Avoid the Misuse of Bayesian Statistics) considerations.
In **Step 5,** the cycle iterates as evidence is available, revising priors and the hierarchical structure.

##### 1254 PHYTOPATHOLOGY®


#### assess if the outcomes look reasonable before analyzing the new

#### data).

#### As data from the new location in the tropics become available, the

#### framework adapts (Fig. 3, moving from Scenario A to Scenario B).

#### A hybrid prior is created by combining the original prior, based on

#### experiments and results in temperate regions, with expert input and

#### adjusting the weight given to expert opinion through a parameterδ.

#### By varyingδin a sensitivity analysis, we can assess the influence

#### of expert judgment on the results. This hybrid prior is then up-

#### dated with experimental data from the tropical setting, producing a

#### posterior distribution that reflects both prior knowledge and new ev-

#### idence. Once the new objective data from the tropics are available,

#### the same experimental trial can also be analyzed using standard

#### frequentist methods. When priors are well calibrated and sample

#### sizes are modest, Bayesian and frequentist approaches tend to yield

#### similar conclusions (Bayarri and Berger 2004), meaning that ei-

#### ther approach can be used, depending on whether decision-makers

#### choose to include expert opinion.

#### This workflow is presented as an illustrative example rather

#### than a prescriptive recommendation. A complete technical expla-

#### nation, with a fully worked simulated example—including sim-

#### ulated data from expert knowledge elicitation, expert knowledge

#### elicitation formulated as a prior, prior-predictive checks, hierarchi-

#### cal expert modeling, sensitivity analyses, and a comparison with

#### frequentist intervals—is provided athttps://github.com/jrobledob/

#### Expert_Elicitation_in_Plant_Pathology, together with the code.

## Lessons Learned from Implementing Expert

## Knowledge Elicitation in Plant Pathology

#### We discuss lessons learned from experience using expert knowl-

#### edge elicitation to study questions in plant health in Cameroon,

#### Colombia, Ethiopia, India, Nepal, Pakistan, the Republic of Geor-

#### gia, Tanzania, and the United States (A. Adhikari, in preparation;

#### Andersen Onofre et al. 2021; Mouafo-Tchinda et al. 2024; Plex Sulá

#### et al. 2025; J. Robledo, M. Betancourt, and K. Garrett, unpublished

#### data ; Thomas-Sharma et al. 2017). Many of these analyses focused

#### on generating geographic data layers of estimated parameters such

#### as yield loss and networks of informal trade in planting materials as

#### a potential conduit for the spread of seedborne pathogens. A com-

#### mon goal was to provide baseline information about the geographic

#### distribution of pathogens and pests at a national level, as well as

#### the potential for invasive spread, as input for decision-making by

#### national plant protection organizations. These goals represent a dif-

#### ferent approach compared with the above example of Bayesian

#### analysis, which focused careful attention on understanding a sin-

#### gle important parameter. Focused attention in Bayesian analysis

#### could add another dimension to the national projects discussed in

#### this section, when stakeholders identify key parameters for detailed

#### consideration. Direct elicitation may be used for precise quanti-

#### ties and indirect elicitation when narratives/experiences must be

#### encoded before quantification (Martin et al. 2012).

#### Continuous instrument improvement

#### The design and adaptation of instruments were critical factors

#### influencing the success of expert knowledge elicitation. Adjusting

#### instruments to each country supported local relevance and expert en-

#### gagement. The approach involved review and adaptation of country-

#### and crop-specific questions with the organizing team, in terms of

#### points such as the relevant pathogen species and relevant yield loss

#### levels to consider, fostering expert engagement (Mouafo-Tchinda

#### et al. 2024). In Thomas-Sharma et al. (2017), experts were asked

#### to provide frequency distributions, such as the distribution of fre-

#### quencies of grower use of different types of management. However,

#### many experts were more comfortable providing means, especially

#### when questions involved intricate biotic interactions. This indicates

#### the need for a compromise between the information that researchers

#### would like to obtain and what experts can provide, especially given

#### time constraints. It also highlights the need for instruments that fa-

#### cilitate data acquisition, for example, by providing real-time and

#### interactive feedback to experts in a summary of their responses

#### (e.g., maps or graphs) and potentially figures indicating the impli-

#### cations of expert parameter estimates. The use of varied question

#### formats addressing the same information could increase confidence

#### and provide measures of uncertainty, if time allows. To reduce an-

#### choring and capture uncertainty, SHELF-style percentile prompts

#### with real-time plots and pre-specified EFSA aggregation could be

#### implemented, for example, using Elicitator, REDCap, or Qualtrics

#### (European Food Safety Authority 2014; Gosling 2018; Morgan

#### 2014; Patridge and Bardyn 2018).

#### Expert identification

#### For system-level studies, identifying the right mix of experts

#### with relevant and complementary knowledge is important (Thomas-

#### Sharma et al. 2017). In some cases, participants may have narrow

#### specialization, such as deep knowledge of a single pathosystem or

#### region, but limited awareness of others. This underscores the im-

#### portance of assembling diverse expert teams to ensure broad and

#### balanced insights for the pathosystems being studied. Confirm-

#### ing instrument content with in-country expert organizers prior to

#### expert knowledge elicitation is important when applying a study

#### across locations, given that pathogen species and other components

#### of pathosystems can vary widely. Expert knowledge elicitation in

#### plant pathology can benefit from incorporating experts in related

#### disciplines—e.g., entomology, horticulture, economics—to provide

#### a more holistic estimate of yield loss frequency distributions, for

#### example, and to avoid biases from single-discipline perspectives.

#### Selection bias could be mitigated with stratified recruitment and re-

#### sponse weighting and, when feasible, applying Cooke’s calibration

#### using, for example, Excalibur or ANDURYL for performance-

#### based weights (Bird and King 2018; Boutry et al. 2023; Cooke

#### 1991; O’Hagan 2019; Pieter’t Hart et al. 2019).

#### Participatory elicitation

#### Access to experts’ time may be a limiting factor. In Andersen

#### Onofre et al. (2021), expert knowledge elicitation consisted of a

#### 2-day facilitated workshop that included a broad spectrum of stake-

#### holders from the potato value chain. This project made clear the

#### importance of effective facilitators, note-takers, and translators.

#### Beyond the structured questions in the instrument, capturing spon-

#### taneous discussions among stakeholders can be a valuable source

#### of insights. In Mouafo-Tchinda et al. (2024), in-person workshops

#### enabled clarification of the instrument and allowed participants

#### to discuss complex issues before answering the questions. This

#### group dynamic significantly enhanced the consistency and clarity

#### of responses, demonstrating the benefit of collaborative, face-to-

#### face formats. In Thomas-Sharma et al. (2017), expert knowledge

#### elicitation was implemented through paper-based, in-person, and

#### phone interviews, allowing for some direct engagement. The for-

#### mat could have been strengthened with tools that helped experts

#### visualize answers and elicited uncertainty. Delphi or IDEA might

#### be used for anonymized iteration toward estimates and Cooke’s

#### method for auditable individual judgments after independent first

#### estimates (European Food Safety Authority 2014; Hemming et al.

#### 2018; Linstone and Turoff 2011; Morgan 2014).

#### Data analysis and interpretation

#### Interpreting and integrating elicited data also offered important

#### lessons. For example, if some experts perceive questions to be too

#### complicated (such as the case of asking for frequency distribu-

#### tions of yield losses), data analysis is less straightforward when

#### some experts estimate frequency distributions whereas other experts

#### only provide an estimated mean (Thomas-Sharma et al. 2017). One

```
Vol. 115, No. 10, 2025 1255
```

#### solution is to improve instruments for analyzing uncertainty and

#### expert confidence, potentially through synthesizing answers from

#### experts across fields. Integrating expert responses with other data

#### sources, such as analyses of cropland connectivity as a proxy for

#### potential epidemic networks (Xing et al. 2020), can help model

#### pathogen risk and prioritize phytosanitary actions (Andersen Onofre

#### et al. 2021). Finally, transparent documentation of the expert knowl-

#### edge elicitation process (roles of organizers and experts, assump-

#### tions about participation, reviews, and reflections after expert elic-

#### itation) is important for building the credibility and reproducibility

#### of expert knowledge elicitation findings. Data analysis and interpre-

#### tation can benefit from use of percentiles and hierarchical models

#### with ESS caps, prior-predictive checks, varyingδin hybrid priors,

#### linking to additional big data layers, and code narratives with LLMs

#### (Bayarri and Berger 2004; Bock et al. 2020; Bojanowski et al. 2017;

#### Devlin et al. 2019; Mahlein 2016; Mueller et al. 2025; Oakley and

#### O’Hagan 2004; van de Schoot et al. 2021).

#### Based on these experiences, an app to facilitate application of

#### expert knowledge elicitation in plant pathology is being developed

#### (Fontan et al. 2025), using a curated catalog of relevant questions

#### (PlantQuest). This catalog incorporates continuous feedback on

#### how best to formulate questions in instruments for expert elicitation

#### to avoid ambiguities and obtain high-quality data. Having easy-to-

#### use tools for expert knowledge elicitation can facilitate decision-

#### making and provide an opportunity for research teams to share a

#### baseline that is interoperable and reusable across applications.

## Potential for Plant Pathology, Future Applications,

## and New Interfaces with Artificial Intelligence

#### Expert knowledge elicitation has provided important research re-

#### sults in plant pathology over the past two decades, and there are new

#### opportunities in the coming decades. For example, expert elicitation

#### can be integrated with scenario analysis to address key problems in

#### complex systems in plant pathology (Savary et al. 2019), including

#### scenario analysis of global change (climate, land-use, or irrigation

#### change). Sensor technologies may be integrated with expert per-

#### ceptions in disease surveillance (Bock et al. 2020; Mahlein 2016).

#### Another important application of expert knowledge elicitation is in

#### the context of disaster plant pathology (Etherton et al. 2024). Be-

#### fore and after disasters such as droughts, floods, and civil conflicts,

#### there is a need for plant disease information, but rapid implemen-

#### tation of new objective studies is often challenging. Without expert

#### knowledge elicitation methods, information needed from experts

#### after disasters may often be obtained using rushed and casual ap-

#### proaches. Expert knowledge elicitation can improve elicitation of

#### high-quality information from experts using methods that account

#### for uncertainty in expert knowledge for timely, decision-relevant

#### inputs when conventional data collection is constrained.

#### Interfaces with artificial intelligence and data workflows

#### Expert knowledge elicitation presents valuable opportunities to

#### fill data gaps, promote cost-efficient forecasting, catalyze interdisci-

#### plinary collaboration, and support integration with natural language

#### processing and other artificial intelligence-driven models. Expert

#### knowledge elicitation may be especially useful when combined

#### with probabilistic frameworks, such as Bayesian updates, which

#### are well suited to quantify and appropriately propagate uncertainty

#### in a transparent and rigorous manner. Big data can both inform prior

#### acquisition and be generated by expert knowledge elicitation itself.

#### Capturing and analyzing data with modern artificial intelligence

#### enables more transparent uncertainty quantification and more ac-

#### tionable plant health decisions that can be revisited as new evidence

#### is available. New approaches that incorporate artificial intelligence-

#### driven analysis of elicitation outputs (text, audio, and video) may

#### make a range of new types of analyses possible, such as the poten-

#### tial to measure expert uncertainty based on analysis of nonverbal

#### cues in videos.

#### LLMs to support instrument design and data synthesis

#### There are many opportunities for ongoing improvement to meth-

#### ods in expert knowledge elicitation. LLMs may be used to provide

#### an initial summary of experts’ answers to open-ended questions and

#### discussion (Kaiyrbekov et al. 2025). Transformer-based models can

#### be used to identify latent themes and quantify agreement and uncer-

#### tainty. Because LLMs synthesize available literature, they can help

#### formulate questions for elicitation instruments and help identify

#### knowledge gaps. LLMs also have potential for identifying ques-

#### tions that could be used to weight expert responses based on how

#### accurate experts are, as this could synthesize pertinent knowledge

#### and help to identify relevant questions that are of a similar caliber

#### to those in the elicitation instrument. Integrating expert knowledge

#### elicitation methods with digital twins (Table 1) could clarify for

#### experts the implications of their parameter estimates. These ap-

#### proaches target two bottlenecks: efficient instrument preparation

#### and scalable synthesis of mixed-format elicitation traces.

#### A human–artificial intelligence pipeline vision

#### In the future, the most effective systems to support plant health

#### will likely integrate across new objective data and expert knowledge

#### input, with potential automated cycling between human and artifi-

#### cial intelligence in a streamlined pipeline (expanding on Fig. 1).

#### For example, there is the potential to use LLMs to facilitate elicit-

#### ing expert estimates of priors in Bayesian updates (Capstick et al.

#### 2025). There are exciting prospects to integrate the most valuable

#### input from each data acquisition component, such as in the con-

#### text of ongoing development of a national plant health risk analysis

#### (Mouafo-Tchinda et al. 2024). Effective systems will emphasize

#### reproducibility, transparent uncertainty, and the ability to update

#### decisions as soon as new data or judgments become available.

#### Capacity needs

#### Although advances in LLMs and machine learning may sup-

#### port more effective use of expert knowledge, there may be less

#### expert knowledge available in plant pathology in the future.

#### Underinvestment in research and extension programs may result

#### in fewer experts who have direct experience with plant disease

#### epidemics. Future public and private investments to maintain ex-

#### pertise in plant health would ensure that there is new and up-to-date

#### information for integration into human and artificial intelligence.

#### Expert knowledge elicitation can help to optimize data-driven deci-

#### sions when resources are limited, and maintaining expert capac-

#### ity remains a prerequisite for realizing the benefits of artificial

#### intelligence-enabled elicitation.

```
Acknowledgments
```
```
We t h a n k t h e Phytopathology reviewers for useful recommendations.
```
```
Literature Cited
```
```
Acuña, I., Andrade-Piedra, J., Andrivon, D., Armengol, J., Elizabeth Arnold, A.,
Avelino, J., Bandyopadhyay, R., Bihon Legesse, W., Bock, C. H., Bove, F.,
Brenes-Arguedas, T., Calonnec, A., Carmona, M., Carnegie, A. J., Castilla,
N. P., Chen, X., Coletta-Filho, H. D., Coley, P. D., Cox, K. D., Davey, T., Del
Ponte, E., Denman, S., Desprez-Loustau, M.-L., Dewdney, M. M., Djurle,
A., Drenth, A., Ducousso, A., Esker, P., Fiaboe, K. M., Hendrik Fourie, P.,
Frankel, S. J., Frey, P., Garcia-Figuera, S., Garrett, K. A., Guérin, M., Hardy,
G. E. S. J., Hausladen, H., Hu, X., Hüberli, D., Juzwik, J., Kang, Z., Kenyon,
L., Kreuze, J., Kromann, P., Kubiriba, J., Kuhnem, P., Kumar, J., Lava Kumar,
P., Lebrun, M.-H., Legg, J. P., Leon, A., Ma, Z., Mahuku, G., Makinson, R. O.,
Marzachi, C., McDonald, B. A., McRoberts, N., Menkir, A., Mikaberidze,
A., Munck, I. A., Nelson, A., Nguyen, N. T. T., O’Gara, E., Ojiambo, P.,
Ortega-Beltran, A., Paul, P., Pethybridge, S., Pinon, J., Ramsfield, T., Rizzo,
D. M., Rossi, V., Safni, I., Sah, S., Santini, A., Sautua, F., Savary, S.,
```
##### 1256 PHYTOPATHOLOGY®


Schreinemachers, P., Singh, M., Spear, E. R., Srinivasan, R., Tripathi, L.,
Vicent, A., Viljoen, A., Willocquet, L., Woods, A. J., Wu, B., Xia, X., Xu,
X., Yuen, J., Zalamea, P.-C., and Zhou, C. 2023. A global assessment of the
state of plant health. Plant Dis. 107:3649-3665.
Andersen Onofre, K. F., Forbes, G. A., Andrade-Piedra, J. L., Buddenhagen,
C. E., Fulton, J. C., Gatto, M., Khidesheli, Z., Mdivani, R., Xing, Y., and
Garrett, K. A. 2021. An integrated seed health strategy and phytosanitary
risk assessment: Potato in the Republic of Georgia. Agric. Syst. 191:103144.
Andriamampianina, L., Temple, L., de Bon, H., Malézieux, E., and Makowski, D.

2018. Évaluation pluri-critères de l’agriculture biologique en Afrique subsa-
harienne par élicitation probabiliste des connaissances d’experts. Cah. Agric.
27:45002.
Arndt, E., Rumpff, L., Lane, S., Bau, S., Mebalds, M., and Kompas, T. 2022. Esti-
mating probability of visual detection of exotic pests and diseases in the grains
industry—An expert elicitation approach. Front. Ecol. Evol. 10:968436.
Aspinall, W. P., and Cooke, R. M. 2013. Quantifying scientific uncertainty from
expert judgement elicitation. Pages 64-99 in: Risk and Uncertainty Assess-
ment for Natural Hazards. J. Rougier, S. Sparks, and L. J. Hill, eds. Cambridge
University Press, Cambridge, U.K.
Aven, T. 2020. Bayesian analysis: Critical issues related to its scope and bound-
aries in a risk context. Reliab. Eng. Syst. Saf. 204:107209.
Bargmann, C. I., and Marder, E. 2013. From the connectome to brain function.
Nat. Methods 10:483-490.
Battiston, P., Kashyap, R., and Rotondi, V. 2021. Reliance on scientists and
experts during an epidemic: Evidence from the COVID-19 outbreak in Italy.
SSM Popul. Health 13:100721.
Bayarri, M. J., and Berger, J. O. 2004. The interplay of Bayesian and frequentist
analysis. Stat. Sci. 19:58-80.
Bazinet, V., Hansen, J. Y., and Misic, B. 2023. Towards a biologically annotated
brain connectome. Nat. Rev. Neurosci. 24:747-760.
Bird, S. M., and King, R. 2018. Multiple systems estimation (or capture-
recapture estimation) to inform public policy. Annu. Rev. Stat. Appl. 5:95-
118.
Bock, C. H., Barbedo, J. G. A., Del Ponte, E. M., Bohnenkamp, D., and Mahlein,
A.-K. 2020. From visual estimates to fully automated sensor-based measure-
ments of plant disease severity: Status and challenges for improving accuracy.
Phytopathol. Res. 2:9.
Bojanowski, P., Grave, E., Joulin, A., and Mikolov, T. 2017. Enriching word
vectors with subword information. Trans. Assoc. Comput. Linguist. 5:135-
146.
Bojke, L., Soares, M., Claxton, K., Colson, A., Fox, A., Jackson, C., Jankovic,
D., Morton, A., Sharples, L., and Taylor, A. 2021. Good practice in struc-
tured expert elicitation: Learning from the available guidance. In Develop-
ing a Reference Protocol for Structured Expert Elicitation in Health-Care
Decision-Making: A Mixed-Methods Study. NIHR Journals Library. Health
Technology Assessment No. 25.37.
Boutry, S., Helaers, R., Lenaerts, T., and Vikkula, M. 2023. Excalibur: A new
ensemble method based on an optimal combination of aggregation tests for
rare-variant association testing for sequencing data. PLoS Comput. Biol.
19:e1011488.
Bouwmeester, H., Blomme, G., Omondi, A. B., and Ocimati, W. 2023. Banana
bunchy top disease in Africa—Predicting continent-wide disease risks by
combining survey data and expert knowledge. Plant Pathol. 72:1476-1490.
Brady, T. F., Konkle, T., Alvarez, G. A., and Oliva, A. 2008. Visual long-term
memory has a massive storage capacity for object details. Proc. Natl. Acad.
Sci. U.S.A. 105:14325-14329.
Caley, M. J., O’Leary, R. A., Fisher, R., Low-Choy, S., Johnson, S., and
Mengersen, K. 2014. What is an expert? A systems perspective on expertise.
Ecol. Evol. 4:231-242.
Capstick, A., Krishnan, R. G., and Barnaghi, P. 2025. AutoElicit: Using large
language models for expert prior elicitation in predictive modelling. arXiv
2411.17284v5.
Chen, M., Brun, F., Raynal, M., Debord, C., and Makowski, D. 2019. Use of
probabilistic expert elicitation for assessing risk of appearance of grape downy
mildew. Crop Prot. 126:104926.
Colson, A. R., and Cooke, R. M. 2018. Expert elicitation: Using the classical
model to validate experts’ judgments. Rev. Environ. Econ. Policy 12:113-132.
Cooke, R. M. 1991. Experts in Uncertainty: Opinion and Subjective Probability
in Science. Oxford University Press, New York.
Cooke, R. M., and Goossens, L. H. J. 2004. Expert judgement elicitation for risk
assessments of critical infrastructures. J. Risk Res. 7:643-656.
Costa, M. C., Goumperis, T., Andersson, W., Badiola, J., Ooms, W., Pongolini,
S., Saegerman, C., Jurkovic, M., Tuominen, P., Tsigarida, E., Steinwider, J.,
Hölzl, C., Mikushinska, N., Gross-Boškovi ́c, A., Kanari, P., Christodoulidou,
M., Babiˇcka, L., Korsgaard, H., Pesonen, S., Fillet, A. M., Foures, F., Lohman,
M., Luber, P., Szabó, M., Cseh, J., Noteborn, H. P. J. M., Færden, K., Fulke,
Å., Trnovec, T., Ilbäck, N. G., Andersson, T., Donohoe, T., Merten, C., and
Robinson, T. 2017. Risk identification in food safety: Strategy and outcomes

```
of the EFSA emerging risks exchange network (EREN), 2010–2014. Food
Control 73:255-264.
Daee, P., Peltola, T., Soare, M., and Kaski, S. 2017. Knowledge elicitation
via sequential probabilistic inference for high-dimensional prediction. Mach.
Learn. 106:1599-1620.
Der Kiureghian, A., and Ditlevsen, O. 2009. Aleatory or epistemic? Does it
matter? Struct. Saf. 31:105-112.
Devlin, J., Chang, M.-W., Lee, K., and Toutanova, K. 2019. BERT: Pre-training
of deep bidirectional transformers for language understanding. Pages 4171-
4186 in: Proceedings of the 2019 Conference of the North American Chapter
of the Association for Computational Linguistics: Human Language Tech-
nologies, Volume 1 (Long and Short Papers). J. Burstein, C. Doran, and T.
Solorio, eds. Association for Computational Linguistics, Minneapolis, MN.
EFSA Panel on Plant Health (PLH), Jeger, M., Bragard, C., Caffier, D.,
Candresse, T., Chatzivassiliou, E., Dehnen-Schmutz, K., Grégoire, J.-C.,
Jaques Miret, J. A., MacLeod, A., Navarro, M. N., Niere, B., Parnell, S.,
Potting, R., Rafoss, T., Rossi, V., Urek, G., Van Bruggen, A., Van Der Werf,
W., West, J., Winter, S., Almeida, R., Bosco, D., Jacques, M-A., Landa, B.,
Purcell, A., Saponari, M., Czwienczek, E., Delbianco, A., Stancanelli, G.,
and Bragard, C. 2018. Guidance on quantitative pest risk assessment. EFSA
J. 16:e05350.
Etherton, B. A., Choudhury, R. A., Alcalá Briseño, R. I., Mouafo-Tchinda, R. A.,
Plex Sulá, A. I., Choudhury, M., Adhikari, A., Lei, S. L., Kraisitudomsook,
N., Buritica, J. R., Cerbaro, V. A., Ogero, K., Cox, C. M., Walsh, S. P.,
Andrade-Piedra, J. L., Omondi, B. A., Navarrete, I., McEwan, M. A., and
Garrett, K. A. 2024. Disaster plant pathology: Smart solutions for threats to
global plant health from natural and human-driven disasters. Phytopathology
114:855-868.
Etherton, B. A., Plex Sulá, A. I., Mouafo-Tchinda, R. A., Kakuhenzire, R.,
Kassaye, H. A., Asfaw, F., Kosmakos, V. S., McCoy, R. W., Xing, Y., Yao,
J., Sharma, K., and Garrett, K. A. 2025. Translating Ethiopian potato seed
networks: Identifying strategic intervention points for managing bacterial wilt
and other diseases. Agric. Syst. 222:104167.
European Food Safety Authority. 2014. Guidance on expert knowledge elicita-
tion in food and feed safety risk assessment. EFSA J. 12:3734.
Fontan, R., Perez, C. M., Adhikari, A., Mouafo-Tchinda, R. A., Plex Sulá, A. I.,
Robledo, J., Etherton, B. A., Choudhary, M., Sarwar, M. A., Naveed, Z. A.,
and Garrett, K. A. 2025. MetaQuestion: A web application for expert knowl-
edge elicitation addressing plant health and applied plant ecology. arXiv
2509.19393.
Garrett, K. A., Madden, L. V., Hughes, G., and Pfender, W. F. 2004. New
applications of statistical tools in plant pathology. Phytopathology 94:999-
1003.
Gelman, A., and Hill, J. 2007. Data Analysis Using Regression and Multi-
level/Hierarchical Models. Cambridge University Press, Cambridge, U.K.
Gelman, A., and Shalizi, C. R. 2013. Philosophy and the practice of Bayesian
statistics. Br. J. Math. Stat. Psychol. 66:8-38.
Gelman, A., Vehtari, A., Simpson, D., Margossian, C. C., Carpenter, B., Yao,
Y., Kennedy, L., Gabry, J., Bürkner, P.-C., and Modrák, M. 2020. Bayesian
Workflow. arXiv 2011.01808.
Gemini Team Google. 2025. Gemini: A family of highly capable multimodal
models. arXiv 2312.11805v5.
Glennon, E. E., Bruijning, M., Lessler, J., Miller, I. F., Rice, B. L., Thompson,
R. N., Wells, K., and Metcalf, C. J. E. 2021. Challenges in modeling the
emergence of novel pathogens. Epidemics 37:100516.
Gosling, J. P. 2018. SHELF: The Sheffield Elicitation Framework. Pages 61-
in: Elicitation: The Science and Art of Structuring Judgement. L. C. Dias,
A. Morton, and J. Quigley, eds. Springer International Publishing, Cham,
Switzerland.
Grieves, M., and Vickers, J. 2017. Digital Twin: Mitigating unpredictable, un-
desirable emergent behavior in complex systems. Pages 85-113 in: Transdis-
ciplinary Perspectives on Complex Systems: New Findings and Approaches.
F.-J. Kahlen, S. Flumerfelt, and A. Alves, eds. Springer, Cham.
Grigore, B., Peters, J., Hyde, C., and Stein, K. 2017. EXPLICIT: A feasibility
study of remote expert elicitation in health technology assessment. BMC
Med. Inform. Decis. Mak. 17:131.
Hadjigeorgiou, E., Clark, B., Simpson, E., Coles, D., Comber, R., Fischer,
A. R. H., Meijer, N., Marvin, H. J. P., and Frewer, L. J. 2022. A system-
atic review into expert knowledge elicitation methods for emerging food and
feed risk identification. Food Control 136:108848.
Hartley, D., and French, S. 2021. Bayesian modelling of dependence between
experts: Some comparisons with Cooke’s classical model. Pages 115-146 in:
Expert Judgement in Risk and Decision Analysis. A. M. Hanea, G. F. Nane,
T. Bedford, and S. French, eds. Springer International Publishing, Cham,
Switzerland.
Hemming, V., Burgman, M. A., Hanea, A. M., McBride, M. F., and Wintle,
B. C. 2018. A practical guide to structured expert elicitation using the IDEA
protocol. Methods Ecol. Evol. 9:169-180.
```
```
Vol. 115, No. 10, 2025 1257
```

Herrero, M., Thornton, P. K., Mason-D’Croz, D., Palmer, J., Bodirsky, B. L.,
Pradhan, P., Barrett, C. B., Benton, T. G., Hall, A., Pikaar, I., Bogard, J. R.,
Bonnett, G. D., Bryan, B. A., Campbell, B. M., Christensen, S., Clark,
M., Fanzo, J., Godde, C. M., Jarvis, A., Loboguerrero, A. M., Mathys, A.,
McIntyre, C. L., Naylor, R. L., Nelson, R., Obersteiner, M., Parodi, A., Popp,
A., Ricketts, K., Smith, P., Valin, H., Vermeulen, S. J., Vervoort, J., van Wijk,
M., van Zanten, H. H., West, P. C., Wood, S. A., and Rockström, J. 2021. Artic-
ulating the effect of food systems innovation on the Sustainable Development
Goals. Lancet Planet Health 5:e50-e62.
Hughes, G., and Madden, L. V. 2002. Some methods for eliciting expert knowl-
edge of plant disease epidemics and their application in cluster sampling for
disease incidence. Crop Prot. 21:203-215.
Ibrahim, J. G., and Chen, M.-H. 2000. Power prior distributions for regression
models. Stat. Sci. 15:46-60.
Ikorasaki, F., and Akbar, M. B. 2018. Detecting corn plant disease with expert
system using Bayes theorem method. Pages 1-4 in: 2018 6th International
Conference on Cyber and IT Service Management (CITSM).
James, A., Choy, S. L., and Mengersen, K. 2010. Elicitator: An expert elic-
itation tool for regression in ecology. Environ. Modell. Software 25:129-
145.
Jeger, M. J., Madden, L. V., and van den Bosch, F. 2018. Plant virus epi-
demiology: Applications and prospects for mathematical modeling and anal-
ysis to improve understanding and disease control. Plant Dis. 102:837-
854.
Kaiyrbekov, K., Dobbins, N. J., and Mooney, S. D. 2025. Automated survey
collection with LLM-based conversational agents. arXiv 2504.02891.
Kitchin, R., and McArdle, G. 2016. What makes Big Data, Big Data?
Exploring the ontological characteristics of 26 datasets. Big Data Soc.
3:2053951716631130.
Knol, A. B., Slottje, P., van der Sluijs, J. P., and Lebret, E. 2010. The use of
expert elicitation in environmental health impact assessment: A seven step
procedure. Environ. Health 9:19.
Kowal, M., Sorokowski, P., Kulczycki, E., andZela ́ ̇ zniewicz, A. 2022. The
impact of geographical bias when judging scientific studies. Scientometrics
127:265-273.
Kuhnert, P. M., Martin, T. G., and Griffiths, S. P. 2010. A guide to eliciting and
using expert knowledge in Bayesian ecological models. Ecol. Lett. 13:900-
914.
Li, M. Y., and Muldowney, J. S. 1995. Global stability for the SEIR model in
epidemiology. Math. Biosci. 125:155-164.
Linstone, H. A., and Turoff, M. 2011. Delphi: A brief look backward and
forward. Technol. Forecast. Soc. Change 78:1712-1719.
Madden, L. V., Hughes, G., and van den Bosch, F. 2007. The Study of Plant
Disease Epidemics. American Phytopathological Society, St. Paul, MN.
Mahlein, A.-K. 2016. Plant disease detection by imaging sensors – Parallels and
specific demands for precision agriculture and plant phenotyping. Plant Dis.
100:241-251.
Mangen, M.-J. J., Plass, D., Havelaar, A. H., Gibbons, C. L., Cassini, A.,
Mühlberger, N., van Lier, A., Haagsma, J. A., Brooke, R. J., Lai, T., de Waure,
C., Kramarz, P., Kretzschmar, M. E. E., on behalf of the BCoDE Consortium.

2013. The pathogen- and incidence-based DALY approach: An appropriated
methodology for estimating the burden of infectious diseases. PLoS One
8:e79740.
Martin, T. G., Burgman, M. A., Fidler, F., Kuhnert, P. M., Low-Choy, S.,
McBride, M., and Mengersen, K. 2012. Eliciting expert knowledge in con-
servation science. Conserv. Biol. 26:29-38.
Martin, T. G., Kuhnert, P. M., Mengersen, K., and Possingham, H. P. 2005.
The power of expert opinion in ecological models using Bayesian methods:
Impact of grazing on birds. Ecol. Appl. 15:266-280.
McAfee, A., and Brynjolfsson, E. 2012. Big data: The management revolution.
Harv. Bus. Rev. 90:60-68.
McBride, M. F., Garnett, S. T., Szabo, J. K., Burbidge, A. H., Butchart, S. H. M.,
Christidis, L., Dutson, G., Ford, H. A., Loyn, R. H., Watson, D. M., and
Burgman, M. A. 2012. Structured elicitation of expert judgments for threat-
ened species assessment: A case study on a continental scale using email.
Methods Ecol. Evol. 3:906-920.
McGlothlin, A. E., and Viele, K. 2018. Bayesian hierarchical models. JAMA
320:2365-2366.
McGuire, S., and Sperling, L. 2016. Seed systems smallholder farmers use. Food
Sec. 8:179-195.
McKenzie, C. R. M., Liersch, M. J., and Yaniv, I. 2008. Overconfidence in
interval estimates: What does expertise buy you? Organ. Behav. Hum. Decis.
Process. 107:179-191.
McRoberts, N., Thomas, C. S., Brown, J. K., Nutter, F. W., Stack, J. P., and
Martyn, R. D. 2016. The evolution of a process for selecting and prioritizing
plant diseases for recovery plans. Plant Dis. 100:665-671.
Mila, A. L., and Carriquiry, A. L. 2004. Bayesian analysis in plant pathology.
Phytopathology 94:1027-1030.

```
Mkondiwa, M., Hurley, T. M., and Pardey, P. G. 2024. Closing the gaps in ex-
perimental and observational crop response estimates: A Bayesian approach.
Q Open 4:qoae017.
Morgan, M. G. 2014. Use (and abuse) of expert elicitation in support of de-
cision making for public policy. Proc. Natl. Acad. Sci. U.S.A. 111:7176-
7184.
Morita, S., Thall, P. F., and Müller, P. 2008. Determining the effective sample
size of a parametric prior. Biometrics 64:595-602.
Motisi, N., Bommel, P., Leclerc, G., Robin, M.-H., Aubertot, J.-N., Butron,
A. A., Merle, I., Treminio, E., and Avelino, J. 2022. Improved forecasting of
coffee leaf rust by qualitative modeling: Design and expert validation of the
ExpeRoya model. Agric. Syst. 197:103352.
Mouafo-Tchinda, R. A., Etherton, B. A., Plex Sulá, A. I., Andrade-Piedra, J.,
Ogero, K., Omondi, B. A., McEwan, M. A., Tayo, P. M. T., Harahagazwe, D.,
Cherinet, M., Gebeyehu, S., Sperling, L., and Garrett, K. A. 2024. Pathogen
and pest risks to vegetatively propagated crops in humanitarian contexts: To-
ward a national plant health risk analysis for Cameroon and Ethiopia. bioRxiv
580019.
Mueller, D. S., Iles, L. C., Pilcher, C. L., Sisson, A. J., Magarey, R., Adams,
R., Almodovar, W. I., Alston, D., Beauzay, P., Bessin, R., Bish, M., Burrows,
M., Calixto, A., Chandran, R., Colquhoun, J. B., Concklin, M., Dreves, A. J.,
Ellsworth, P. C., Esker, P. D., Farrar, J. J., Fournier, A., Frank, D., Hamby, K.,
Hamilton, G., Hanson, A., Hazelrigg, A., Hein-Ferris, N., Held, D., Jasinski,
J., Kelly, H. M., Kerns, D., Kersten, M., Kerzicnik, L., Knodel, J., Koehler,
G., Kratsch, H., Krupke, C. H., Leppla, N. C., Lizotte, E., Matney, C., Melan-
son, R. A., Miller, F., Murray, M., Owens, D., Plewa, D., Reay-Jones, F. P.
F., Rondon, S. I., Royer, T. A., Rozeboom, P. A., Sandler, H. A., Schell, S.
P., Schuh, M., Seipel, T., Carley, D. S., Sial, A., Singh, R., Smith, D. L.,
Stock, T., Studebaker, G., Szczepaniec, A., Tewksbury, L., Tooker, J., Varen-
horst, A. J., Vinchesi-Vahl, A., Walsh, D., Wickwar, D., Wright, R. J., and
Zebelo, S. 2025. Integrated pest management: State infrastructure status af-
ter 50 yr of federal support (1973 to 2023). J. Integr. Pest. Manag. 16(1):
30.
Oakley, J. E., and O’Hagan, A. 2004. Probabilistic sensitivity analysis of com-
plex models: A Bayesian approach. J. R. Stat. Soc. Ser. B Stat. Methodol.
66:751-769.
O’Hagan, A. 2019. Expert knowledge elicitation: Subjective but scientific. Am.
Stat. 73:69-81.
Patridge, E. F., and Bardyn, T. P. 2018. Research Electronic Data Capture
(REDCap). J. Med. Libr. Assoc. 106:142-144.
Pieter’t Hart, C. M., Leontaris, G., and Morales-Nápoles, O. 2019. Update
(1.1) to ANDURIL — A MATLAB toolbox for ANalysis and Decisions
with UnceRtaInty: Learning from expert judgments: ANDURYL. SoftwareX
10:100295.
Petracca, L. S., Frair, J. L., Cohen, J. B., Calderón, A. P., Carazo-Salazar, J.,
Castañeda, F., Corrales-Gutiérrez, D., Foster, R. J., Harmsen, B., Hernández-
Potosme, S., Herrera, L., Olmos, M., Pereira, S., Robinson, H. S., Robinson,
N., Salom-Pérez, R., Urbina, Y., Zeller, K. A., and Quigley, H. 2018. Robust
inference on large-scale species habitat use with interview data: The status
of jaguars outside protected areas in Central America. J. Appl. Ecol. 55:
723-734.
Plex Sulá, A. I., Sarwar, M. A., Ali, S., Qureshi, N., Maqbool, R., Saleem, K.,
Singh, P. K., Ali, Z., Garrett, K. A., and Naveed, Z. A. 2025. Wheat diseases
and pests in Pakistan: A nationwide assessment. agriRxiv 20250496487.
Rongen, G., Morales-Nápoles, O., and Kok, M. 2024. Using the classi-
cal model for structured expert judgment to estimate extremes: A case
study of discharges in the Meuse River. Hydrol. Earth Syst. Sci. 28:2831-
2848.
Rosace, M. C., Conesa, D. V., López-Quílez, A., Marini, L., Martinez-Beneito,
M. A., Nardi, D., Rossi, V., Vicent, A., and Cendoya, M. 2025. Hotspot map-
ping of pest introductions in the EU: A regional analysis of environmental,
anthropogenic and spatial effects. Biol. Invasions 27:18.
Rose, L. E., Hemming, V., Hanea, A. M., Wintle, B. A., and Chee, Y.
E. 2023. Linking species distribution models with structured expert elic-
itation for predicting management effectiveness. Conserv. Sci. Pract. 5:
e13038.
Runge, M. C., Converse, S. J., and Lyons, J. E. 2011. Which uncertainty? Using
expert elicitation and expected value of information to design an adaptive
program. Biol. Conserv. 144:1214-1223.
Sagiroglu, S., and Sinanc, D. 2013. Big data: A review. Pages 42-47 in: 2013
International Conference on Collaboration Technologies and Systems (CTS).
IEEE Xplore, San Diego, CA.
Saltelli, A., Ratto, M., Andres, T., Campolongo, F., Cariboni, J., Gatelli, D.,
Saisana, M., and Tarantola, S. 2008. Global Sensitivity Analysis: The Primer.
John Wiley & Sons, New York.
Savary, S., Willocquet, L., Pethybridge, S. J., Esker, P., McRoberts, N., and
Nelson, A. 2019. The global burden of pathogens and pests on major food
crops. Nat. Ecol. Evol. 3:430-439.
```
##### 1258 PHYTOPATHOLOGY®


Scherm, H., Thomas, C. S., Garrett, K. A., and Olsen, J. M. 2014. Meta-analysis
and other approaches for synthesizing structured and unstructured data in
plant pathology. Annu. Rev. Phytopathol. 52:453-476.
Soares, M., Colson, A., Bojke, L., Ghabri, S., Garay, O. U., Felli, J. K., Lee, K.,
Molsen-David, E., Morales-Napoles, O., Shaffer, V. A., and IJzerman, M. J.

2024. Recommendations on the use of structured expert elicitation protocols
for healthcare decision making: A good practices report of an ISPOR task
force. Value Health 27:1469-1478.
Sobol’, I. M. 2001. Global sensitivity indices for nonlinear mathematical models
and their Monte Carlo estimates. Math. Comput. Simul. 55:271-280.
Tao, F., Qi, Q., Wang, L., and Nee, A. Y. C. 2019. Digital twins and cyber–
physical systems toward smart manufacturing and industry 4.0: Correlation
and comparison. Engineering 5:653-661.
Thomas-Sharma, S., Andrade-Piedra, J., Carvajal Yepes, M., Hernandez Nopsa,
J. F., Jeger, M. J., Jones, R. A. C., Kromann, P., Legg, J. P., Yuen, J., Forbes,
G. A., and Garrett, K. A. 2017. A risk assessment framework for seed degener-
ation: Informing an integrated seed health strategy for vegetatively propagated
crops. Phytopathology 107:1123-1135.
Tversky, A., and Kahneman, D. 1974. Judgment under uncertainty: Heuristics
and biases. Science 185:1124-1131.
U.S. Environmental Protection Agency. 2004. Fumigant bystander exposure
model review: The Fumigant Exposure Modeling System (FEMS) using
metam sodium as a case study. U.S. EPA Archive Document.https://archive.
epa.gov/scipoly/sap/meetings/web/pdf/aug2004final.pdf(accessed 17 July
2025).
U.S. Environmental Protection Agency. 2009. USEPA: Expert Elicitation
Task Force White Paper. U.S. EPA Archive Document. https://archive.epa.
gov/osa/pdfs/web/pdf/expert_elicitation_white_paper-january_06_2009.pdf
(accessed 17 June 2025).

```
U.S. Environmental Protection Agency. 2024. US EPA - Framework for In-
teragency Collaboration to Review Potential Antibacterial and Antifun-
gal Resistance Risks Associated with Pesticide Use.https://www.epa.gov/
system/files/documents/2024-10/11370-05-fyi-framework.pdf(accessed 17
June 2025).
van de Schoot, R., Depaoli, S., King, R., Kramer, B., Märtens, K., Tadesse,
M. G., Vannucci, M., Gelman, A., Veen, D., Willemsen, J., and Yau, C. 2021.
Bayesian statistics and modelling. Nat. Rev. Methods Primers 1:1.
Wang, Y., Liu, D., and Wang, Y. 2003. Discovering the capacity of human
memory. Brain Mind 4:189-198.
Williams, C. J., Wilson, K. J., and Wilson, N. 2021. A comparison of prior
elicitation aggregation using the classical method and SHELF. J. R. Stat.
Soc. Ser. A Stat. Soc. 184:920-940.
Wittmann, M. E., Cooke, R. M., Rothlisberger, J. D., Rutherford, E. S., Zhang,
H., Mason, D. M., and Lodge, D. M. 2015. Use of structured expert judgment
to forecast invasions by bighead and silver carp in Lake Erie. Conserv. Biol.
29:187-197.
Xiao, Y., Dong, Y., Huang, W., and Liu, L. 2022. Regional prediction of
Fusarium head blight occurrence in wheat with remote sensing based
Susceptible-Exposed-Infectious-Removed model. Int. J. Appl. Earth Obs.
Geoinf. 114:103043.
Xing, Y., Hernandez Nopsa, J. F., Andersen, K. F., Andrade-Piedra, J. L.,
Beed, F. D., Blomme, G., Carvajal-Yepes, M., Coyne, D. L., Cuellar, W. J.,
Forbes, G. A., Kreuze, J. F., Kroschel, J., Kumar, P. L., Legg, J. P., Parker,
M., Schulte-Geldermann, E., Sharma, K., and Garrett, K. A. 2020. Global
cropland connectivity: A risk factor for invasion and saturation by emerging
pathogens and pests. BioScience 70:744-758.
Yuen, J. E., and Hughes, G. 2002. Bayesian analysis of plant disease prediction.
Plant Pathol. 51:407-412.
```
```
Vol. 115, No. 10, 2025 1259
```

[[RAW FILES]]