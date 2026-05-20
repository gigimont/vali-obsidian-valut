```
Journal of Strategic Information Systems 33 (2024) 101848
```
Available online 13 July 2024
0963-8687/© 2024 The Author(s). Published by Elsevier B.V. This is an open access article under the CC BY license
(http://creativecommons.org/licenses/by/4.0/).


## Leif Sundberg

```
*
```
## , Jonny Holmstr ̈om

_Umeå University, Swedish Center for Digital Innovation (SCDI), Department of Informatics. Universitetstorget 4, 901 87 Umeå, Sweden_

ARTICLE INFO

_Keywords:_
Knowledge production
Artificial Intelligence
Machine Learning
Natural Language Processing
Public Sector

```
ABSTRACT
```
```
Machine learning (ML) offers widely-recognized, but complex, opportunities for both public and
private sector organizations to generate value from data. A key requirement is that organizations
must find ways to develop new knowledge by merging crucial ‘domain knowledge’ of experts in
relevant fields with ‘machine knowledge’, i.e., data that can be used to inform predictive models.
In this paper, we argue that understanding the process of generating such knowledge is essential
to strategically develop ML. In efforts to contribute to such understanding, we examine the
generation of new knowledge from domain knowledge through ML via an exploratory study of
two cases in the Swedish public sector. The findings reveal the roles of three mechanisms –
dubbed consolidation, algorithmic mediation, and naturalization – in tying domain knowledge to
machine knowledge. The study contributes a theory of knowledge production related to orga-
nizational use of ML, with important implications for its strategic governance, particularly in the
public sector.
```
**Introduction**

With advances in machine learning (ML) (Jordan and Mitchell, 2015), artificial intelligence (AI) is considered a key strategic
component for leveraging value from organizational data and creating new knowledge (Shollo et al., 2022). However, despite long-
standing optimistic narratives regarding the use of (big) data, it remains an underutilized asset, particularly in public sector organi-
sations (Cho and Lee, 2022; van Ooijen et al., 2019; Shastri and Deshpande, 2020). Many AI initiatives fail to generate value (Borges
et al., 2021; Brynjolfsson et al., 2017: Davenport and Bean, 2023). Therefore, investigating ways to exploit data as a strategic resource
is an important element of contemporary information systems (IS) research (Günther et al., 2022).
As noted by the European Commission (2022), “High quality datasets are essential for the development and deployment of AI
systems”, and researchers are currently engaged in finding ways of identifying datasets of high value (Nikiforova et al., 2023).
However, the processes involved in converting datasets into valuable information within organizations are complex, and key foci of
contemporary IS research (Ashrafi et al., 2024). The features and qualities of datasets are highly dependent on numerous contextual
factors that influence their creation and use (Vial, 2019; Smith, 2020). Consequently, both their meanings and representations must be
continuously managed to use them effectively as strategic resources to generate new knowledge in organizations (Aaltonen et al.,
2021; Alaimo et al., 2020: Østerlie and Monteiro, 2020).
It is well-documented that creating organizational knowledge is never a straightforward process (Boland & Tenkasi, 1995; Choo,

```
* Corresponding author.
E-mail addresses: leif.sundberg@umu.se (L. Sundberg), jonny.holmstrom@umu.se (J. Holmstrom). ̈
```
```
Contents lists available at ScienceDirect
```
# Journal of Strategic Information Systems

```
journal homepage: http://www.elsevier.com/locate/jsis
```
https://doi.org/10.1016/j.jsis.2024.


1998; Cook & Brown, 1999; Marabelli and Newell; 2012; Tsoukas, 2009). Recent empirical studies show that this is particularly true
for AI and ML initiatives (Pachidi et al., 2021; Lebovitz et al., 2021; van den Broek et al., 2021), which involve new practices, such as
data labelling (Mackenzie, 2017). The increasing adoption of algorithms in organizations is also spurring the emergence of new forms
of work and occupations (Kellogg et al., 2020; Waardenburg et al., 2022), calling for examination of the mechanisms through which
organizational knowledge is created, processed, and applied. Hence, there are recognized needs for more research on effective stra-
tegies for applying ML to facilitate the acquisition and development of organizational knowledge (Sturm et al., 2021) beyond narrow
attention to technical aspects (Meijer et al., 2021).
In this paper, we address these needs by investigating the processes involved in the use of ML in organizational knowledge creation.
The public sector is a particularly relevant setting for this as it involves diverse stakeholders that must align the use of emerging
technologies with the public ethos of the welfare state, governance of fiscal funds, and ideals related to accountability and trans-
parency (Gualdi and Cordella, 2024). Research on the use of AI in the public sector has also been characterized as undertheorized
(Zuiderwijk et al., 2021) and in need of more robust empirical investigations (Sun and Medaglia, 2019). According to Selten and
Klievink (2024), public sector organizations have rigid, formal structures, while AI development is promoted in flexible environments
that facilitate experimentation and innovation. However, as shown by Bechmann and Bowker (2019), technologies such as ML also
have inherent rigidity, including requirements for datasets with formal structures. Thus, there is a need to elucidate the processes
involved in aligning these structures to enhance understanding of effective strategies to create valuable knowledge through application
of ML in public sector organizations (Neumann et al., 2024).
Against this backdrop, the purpose of this paper is to analyze the mechanisms involved in the utilization of domain-specific
knowledge to generate organizational insights via ML. By examining the interplay between involved processes, we seek to illumi-
nate the various stages and factors involved in the process of knowledge creation. We specifically address the following research
question (RQ):
_How is organizational knowledge generated in machine learning initiatives?_
To do so, we present an exploratory case study of two ML initiatives in the Swedish public sector, rooted in stories of actors involved
in training predictive systems. The stories contribute to the literature theoretically, by informing a novel process model that illustrates
the mechanisms involved in knowledge creation with ML. Our findings also have empirical and practical implications for strategic AI
governance in the public sector.
This paper proceeds as follows. Section 2 provides background information. The methods applied in the empirical study are
described in Section 3. Findings are presented in Section 4 and discussed in Section 5. Finally, conclusions are presented in Section 6.

**Background: domain knowledge & machine knowledge**

Integrating domain knowledge with ML presents a crucial challenge in leveraging data effectively within organizations. The fusion
of these two elements requires a deep understanding of the professional landscapes that shape data characteristics as well as ML model
behaviors (Lebovitz et al., 2022). The data and ML models used in organizations are informed by _domain knowledge_ with properties that
depend on the structures and practices of the professional communities that populate the associated institutions (Bowker and Star,
1999; Wenger, 1999). In these contexts, datasets are key strategic assets (Aaltonen et al., 2021) that direct the structure of information
as a form of _machine knowledge_ , which can be defined as the process “...where knowledge is created out of data through the application
of ML techniques” (van den Broek et al., 2021, p. 1557). Most ML systems deployed today are based on supervised approaches in which
algorithms learn to recognize patterns in data via ‘ground truth’ labels, but creating ground truths is not straightforward, partly
because of disagreements among the experts involved in labeling (Lebovitz et al., 2021). However, while classifications may become
sources of conflicts and tensions due to differences in representations, they can also foster cooperation between communities (Bowker
and Star, 1999). Thus, there is a need to extend studies on the role of domain experts in ML development (Lebovitz et al., 2021; van den
Broek et al., 2021) with empirical investigations of how these experts use their professional knowledge to inform predictive ML
systems. In this paper, we focus our theorizing on the processes whereby organizational knowledge was created in two public sector ML
initiatives. To build a conceptual framework for this purpose, we define and differentiate domain knowledge and machine knowledge
in the following sections.

_Domain knowledge: categories and practices_

Knowledge production in organizations often involves multiple communities of people with expertise in diverse ‘domains’ or fields
and the generation of innovative outcomes depends on these experts’ abilities not only to use their own skills, but also to take other
groups’ knowledge into account (Boland and Tenkasi, 1995). We define this as ‘domain knowledge’, which is under continuous
development and has strongly social characteristics (Orlikowski, 2002). To characterize it more fully, we draw on multiple literature
streams. An important feature of such knowledge is the ‘categorization’ that stems from classification systems used by modern or-
ganizations (Bowker and Star, 1999). Examples range from classification of diseases to support medical practices, through
technology-induced differentiations such as ‘hand wash’ versus ‘machine wash’ to distinguish between appropriate practices for
cleaning clothes, to identification of ‘races’ to inform discriminatory systems. Thus, classifications constitute information structures
that can have both positive and negative effects on our lives (Bowker and Star, 1999).
Classification is an important element of human reasoning to make sense of the world around us (Foucault, 2005) and the resulting
classes can be applied in tools and systems used by multiple communities of practice within single or multiple organizations (Wenger,
1999). The creation of knowledge in organizations depends on individuals’ abilities to engage in self-reflection on their customary


practices and intersubjectivity with other members (Tsoukas, 2009). As noted by Kravˇcenko (2023), the boundaries between the
knowledge of different experts are in a constant state of evolution, and various types of interests, practical concerns, work tools, and
artifacts play important roles in processes of alignment and misalignment.
Classification is also an important practice in ML development as algorithms are trained on labeled data sorted into categories in the
form of ground truths to distinguish between elements (MacKenzie, 2017). Classifications are infrastructural, with both organizational
and informational elements, always embedded in practice (Keller and Keller, 1996), and the infrastructures may serve single or
multiple organizations to meet both the separate and combined needs of professionals in communities of practice. For example, a
hospital information system needs to serve doctors, nurses, administrators, government agencies, patients, and other relevant groups
of actors (Bowker and Star, 1999; Keller and Keller, 1996). They are often taken for granted, and ‘invisible’ to a degree, until they break
down (Bowker et al., 2010; Heidegger, 2008) or fail to meet particular groups’ needs.
Classifications are performed throughout ML development in activities such as defining task and outcome variables, selecting and
labeling data, selection of algorithms, and model evaluation and deployment (Bechmann and Bowker, 2019). In this sense techno-
logical classifications are powerful artifacts that may link several communities and form highly complex boundaries, which must be
considered in AI development and deployment. A common process to facilitate and harmonize the movement of information and
categories between contexts in technological systems is standardization. However, as noted by Pachidi et al. (2021), referring to
“regimes of knowing”, such efforts also delimit the information that can be transferred, thus clearly flagging what is worth knowing,
and the individuals or groups that have decision-making authority during processes such as technology implementation. An associated
issue is that deficiencies in governance mechanisms when implementing ML systems may lead to severe accountability issues in the
public sector due to these systems’ opacity (Keen et al., 2021; K ̈onig and Wenzelburger, 2020; Medaglia et al., 2021; Janssen et al.,
2020; Zuiderwijk et al., 2021; Asatiani et al., 2021). Hence, there are clear needs for greater understanding of the processes involved:
“the ways in which algorithmic systems are made actionable in organizations; how agency and subjectivities, roles, and relations are
reconfigured” in the creation of ML systems (Jarke and Heuer, 2024, p. 119).
As noted by Asatiani et al. (2021), the trajectory of AI implementation in government depends on the interactions between social
and technical actors. As ML provides a means to use data in knowledge production, there is a need to analyze these interactions more
closely. Tensions often arise due to views of datasets as objective representations (‘truths’) of focal phenomena (Bechmann and
Bowker, 2019; Lebovitz et al., 2021; Vial, 2019). This is because such truths in the form of categories are not constructed _a priori_ , but
sensitive to context and the cultural disposition(s) of the person(s) involved in the classification (Bowker and Star, 1999; Bechmann
and Bowker, 2019). These people are not necessarily data scientists, but knowledge workers who use their expertise to inform ML
models (Jarke and Büchner, 2024). As noted by Alaimo and Kallinikos (2022), the roles of data and algorithms are no longer concerns
of specific experts in administrative and managerial work: they are increasingly becoming pervasive resources and means through
which organizations develop knowledge. This emerging notion is used to define ‘machine knowledge’ in the following section.

_Machine knowledge: Data and algorithms_

Machine knowledge stems from the interplay between data and algorithms as they are used to create predictive ML systems (van
den Broek et al., 2021). According to Jones (2019, p. 3), “data are partial and contingent and are brought into being through situated
practices of conceptualization, recording and use”. Hence, data have a highly situated and contextualized nature (Vial, 2019), rather
than being neutral, raw material (Smith, 2020), and statistical representations of ‘facts’ (Drucker, 2011; see also, Langefors, 1980).
They are not merely important assets, but key pivots that organizational processes revolve and evolve around. In addition to viewing
data as a resource, it can also be considered an important medium for driving organizations’ strategizing (Alaimo and Aaltonen, 2023).
Due to this mediating role, organizations are becoming increasingly immersed in management of, and by, data (Alaimo and Kallinikos,
2021). In a broader perspective, data form epistemic architectures that enable and constrain information flows and related behavior
(Flyverbom and Murray, 2018, p. 10) as they are imbued with norms and values (Akrich, 1992; Latour, 2002; Denton et al., 2021).
To gain value from data, organizations must continuously align their work practices, and account for shifts in stakeholder interests
(Günther et al., 2017). In such processes, organizational categories are built around data, and once accepted they increasingly
reconfigure their environment (May and Finch, 2009; Alaimo and Kallinikos, 2021; Grønsund and Aanestad, 2020). Hence, ‘ground
truth’ creation is not only a key component of ML development, but also constituent in the sense that it directs and may re-configure
knowledge that is included during the development (Henriksen and Bechmann, 2020). Several previous researchers have addressed
the role of domain knowledge in ML development (van den Broek et al., 2021; Sturm et al., 2021; Shollo et al., 2022). However,
extension of their contributions is needed to theoretically account for such re-configurations of knowledge in relation to data and ML
algorithms (Mergel et al., 2024).
Data are made sense of and woven into work and knowledge practices through algorithmic work (Mikalsen and Monteiro, 2021).
Hence, algorithms and data are intertwined in a co-evolutionary process, mutually influencing each other (Dourish, 2016). Algorithms
should not be regarded merely as computational entities, as they increasingly shape and alter conditions for work and organizational
realities (Faraj et al., 2018; Aaltonen and Stelmaszak, 2023). Instead, to faciliate empirical analysis of their roles, they should be
regarded as parts of our culture where they are given meaning and included in certain practices (Seaver, 2017, see also, Dourish,
2016). An important element of such analysis is recognition that the use of algorithmic systems strongly depends on the interpretations
of the professionals using them (Abdel-Karim et al., 2023; Waardenburg et al., 2022). This is consistent with a previous more general
understanding of technology as a social phenomenon that may alter organizational and professional processes (Barley, 1986; 2015;
Dougherty and Dunne, 2011). When algorithms reach beyond the technical domain in which they are created, they cannot be
considered mere computational formulas, but as assemblages entangled in networks of people and practices (Glaser et al., 2021).


Drawing on the cited literature, we identify a need to explore the relation between domain knowledge and machine knowledge
more deeply, to understand how domain experts use their knowledge to inform predictive ML models. While opportunities and
challenges associated with AI and ML in the public sector have received considerable attention (Toll et al., 2020; Pi, 2021; Wirtz et al.,
2019; Wirtz et al., 2020), there is a need for deeper empirical investigations of shifts towards ‘algorithmic bureaucracy’ following the
increasing use of such technologies (Vogl et al., 2020). Echoing Straub et al. (2023), there is a need for more research on epistemic
alignment, i.e., if (and if so how) use of AI/ML in the public sector aligns with current practices of knowledge sharing. Exploration of
how this use may conflict with institutional standards and perceptions of what is considered acceptable behavior is also needed. As
noted by Wirtz et al. (2021, p. 1103), “Studies to date focus in detail on changes to existing government structures, while the creation of
entirely new structures due to new AI technologies is given less consideration.”
In sum, previous research on how professional knowledge is developed and used (which we refer to as domain knowledge) and
becomes institutionalized in organizations, as well as emerging studies on data and algorithms (which we refer to as machine
knowledge) both highlight the situational and contextual nature of the focal phenomena of this paper. However, several important
aspects of organizational knowledge production in ML initiatives require further exploration to deepen our understanding of the
relation between these two types of knowledge (domain knowledge and machine knowledge). First, more illumination of the processes
whereby the rich practices (Lebovitz et al., 2021) of domain experts are used to generate knowledge by informing predictive ML
systems is needed. Second, as data and algorithms are becoming increasingly pervasive and forming epistemic infrastructures, there
are needs to elucidate not only how they become means to discover new knowledge, but also how these infrastructures become
embedded in established knowledge regimes and institutions (Pachidi et al., 2021). To address these needs, we delve into “the
intersection of social and material phenomena” (Leonardi and Barley, 2008, p. 160) where actors create and engage with artifacts that
entail both constraints and affordances. In the following section, we describe our efforts to disentangle these engagements via an
explorative case study.

**Methods**

To investigate how ML contributes to knowledge production in organizations, particularly the use of ML and natural language
processing (NLP) in public organizations, we adopted an exploratory theory-building case study approach (Gehman et al., 2018). The
reasons for this methodological choice were the novelty and rapid development of the focal phenomena, and consequent paucity of
relevant prior theory. Empirically, this paper is based on a study of two cases set in the Swedish public sector, and data collected from
largely semi-structured interviews.

_Case descriptions_

Knowledge production during ML development is initiated when tasks are defined (e.g., what type of problem ML should solve via
predictions), target variables are determined, and training data created. Then a model is selected, trained, evaluated, and eventually
deployed (MacKenzie, 2017; Bechmann and Bowker, 2019). Thus, when selecting case(s) to address our RQ, it was important to ensure
that they could provide insights into this process. An initial challenge was that while ML’s adoption is increasing, many initiatives are
experimental, and difficult to translate into operational practices. To obtain rich empirical information, we also needed access to
people who had been heavily engaged with the data processing to train ML systems in order to hear first-hand accounts of their ex-
periences. Public and private sector organizations profoundly differ in many important respects, including values, stakeholders, ethos,
cultures, accountability, and responsibilities (see, e.g., Rose et al., 2015). These differences could all potentially influence the
development, implementation, and use of ML in organizations. These processes have received much more attention in the private than
in the public sector. Therefore, following calls for more empirically grounded studies in the latter (Sun and Medaglia, 2019; van Noordt
and Misuraca, 2022; Neumann et al., 2024), we focus particularly here on the processes in public sector organizations.
As access was crucial, we identified and obtained access to two relevant settings in the Swedish public sector – a small municipality
and a large national agency (the Tax Agency) – both of which were initiating use of NLP, a form of AI that is expected to play important
roles in both IS generally and digital government specifically (Li, Thomas and Liu, 2021). These two case studies also included in-
terviews with expert participants from a data readiness network facilitated by the ‘AI Sweden’ interest organization (hereafter the ‘AI
ecosystem’), to obtain additional contextual information.
Thus, we chose the two cases (and actors in the AI ecosystem) because of the apparent likelihood that they would provide valuable
insights for theorization on an emerging phenomenon: the use of ML and NLP in organizations (particularly public sector organiza-
tions). The first case, hereafter Case A, concerns a ML project initiated by the Social Services Department of a Swedish municipality
with about 40,000 citizens to provide operational support for social workers. The department receives approximately 2000 reports of
concerns for the welfare of children per year. It is important to process these reports quickly and accurately, then identify urgent risks
of harm to the affected children. To do so, the municipality trained a ML model using NLP techniques to detect signs of harm in text
with the aim to enable faster responses.
As we analyzed the case data to address our RQ, we discovered several interesting issues related to the interviewees’ descriptions of
the relation between their domain knowledge and the use of categories and labels to train ML models. However, at this time we were
not sure if this case was idiosyncratic, or the interviewees’ descriptions could inform the more general theorization required to answer
the RQ. Therefore, we recognized a need to add another case of ML development to explore the extent to which aspects of the processes
identified in Case A manifested in another public sector organizational context. So, we sought another case with similar features (i.e.,
an initiative to use ML/NLP in a public sector organization).


By attending events arranged in the mentioned AI ecosystem, we identified and obtained access to a second case, designated Case B,
set in a large national government agency (the Swedish Tax Agency) with more than 10 000 employees. This agency has strongly
engaged in digital transformation during the last two decades and developed AI/ML solutions for various tasks. This case also involves
NLP-mediated classification, to automatically sort emails based on elements of their content, such as topics, and forward them to
appropriate recipients in the agency. For this, a model was trained using data drawn from previous emails sent to the agency, and
labeled by a group of employees.

_Data collection_

The main sources of the data considered in this paper were 24 semi-structured interviews with 25 interviewees: ten involved in Case
A (I1-I10), eight involved in Case B (I11-I18), and seven experts (I19-I25). The interviews were conducted via Zoom between October
2021 and December 2023, recorded, and fully transcribed.
The interviewees were contacted through snowball sampling (Biernacki and Waldorf, 1981) after interviewing key members
involved in the cases. This method is advantageous for reaching members of a specific, relatively small, and fragmented population
(Lewis-Beck et al., 2003). Positions of the interviewees are listed in Appendix A1, and they are referred to with numbers (I1 to I25) in
the results section. All interviews except one were conducted in Swedish, and exemplary quotations in the results section have been
translated into English (see also Appendix B).
As we were exploring a sociotechnical phenomenon that has received little previous research attention, our first encounters with
the interviewees were based on an interview guide with open-ended questions about the project. It also covered interviewees’ ex-
periences of challenges and potential benefits of both the initiative and more general use of ML in organizations. As the study pro-
gressed, we focused more on this process and the interplay between domain knowledge and machine knowledge, asking the
interviewees to be as specific as possible regarding the mechanisms involved in the conversion of domain knowledge to data and ML
models. Key questions included the following: “What types of knowledge were used to inform the creation and labeling of training
data?”; “Were there any changes in the knowledge during model training?”; “What were the main challenges you encountered during
data labeling?”; “Were there any obstacles to deployment of the model(s) in your organization?”; and “Were there any changes to
[processes / practices / knowledge] when the ML system was created and deployed?”
As mentioned, the data labeling process in both cases was conducted by relatively small groups of individuals with experience of the
relevant domain, who collaborated with people with knowledge of data/ML. For example, I1 and I3 in Case A had previous experience
of work in the social services domain before playing more strategic roles, and collaborating with developers from a private company
(I6, I8) to iteratively create relevant ML models. Similarly, in Case B, data analysts of the Tax Agency (I11, I12, I13) collaborated with
individuals with experience of handling cases (e.g., I14) to label incoming.
The interviews with experts from the external AI ecosystem (which provided a common forum where both cases were presented and
discussed) clearly showed that AI development is not undertaken in isolation by individual agencies. Instead, it is influenced by the
surrounding ecosystem and rapid technological development. Thus, these interviews were beneficial for triangulation as they provided
rich insights into both the development of ML and NLP generally as well as helped validation of the themes that emerged during data
analysis.
The interviews were complemented with data from various secondary sources (Appendix A2): including documents, reports and
PowerPoint presentations from the organizations, screenshots of performance indicators of trained ML models (such as confusion
matrixes and receiving operating characteristic (ROC) curves), and NLP seminars (which we attended both online and on premises).
We also followed the progression of the cases by examining the participants’ and data scientists’ posts on social media channels such as
LinkedIn as well as press releases. The combination and triangulation of these types of data helped to increase the level of knowledge
and gain a better understanding of the focal phenomena (Lewis-Beck et al., 2003).

_Data analysis_

In line with our exploratory investigation of a novel phenomenon, we conducted several iterations between data collection and
analysis, to enable flexible responses to emerging themes. The empirical richness of case studies entails many open-ended ‘sampling’
decisions regarding the main foci of attention and analytical approaches. As cases unfold and their boundaries expand, choices must
inevitably be made from the increasingly numerous aspects that could be addressed. Therefore, we iterated between data analysis and
revisiting the literature to build theoretical foundations for our analysis in this phase. In line with Timmermans and Tavory (2012), we
applied an abductive approach, accompanying and justifying (or cultivating) empirical discoveries with consideration and refinement
of existing theories. Thus, while we see our cases as opportunities to generate theory based on rich insights from empirical phenomena,
we also acknowledge the interrelatedness of the various elements during research work (Dubois and Gadde, 2002). This includes going
“back and forth” between empirical observations and previous literature. As this exploration proceeded, the theoretical concepts of
domain knowledge and machine knowledge were refined by evaluating them against the empirical observations (Suddaby, 2006;
Timmermans and Tavory, 2012).
The interview transcripts were imported into the Atlas.ti software, and the interview guide was slightly updated during the
interview cycle to account for findings from previous interviews. All interviews were transcribed, and secondary data were used to
augment and triangulate the interview data. During this stage (which led to the identification of more than 500 first-order codes), we
focused on constructing a coherent theory by aggregating the varied empirical evidence into constructs, followed by outlining the
relationships between the constructs. Our analytical strategy consisted of the following three main steps.


First, case narratives were constructed, describing how the cases unfolded over time and facilitating the presentation of contextual
details to outline the richness of the qualitative data (Langley, 1999; Pettigrew, 1990). For this, the raw data and first-order codes
informed a chronological overview of the cases, while initial themes in these data started to emerge. The narratives were constructed
with the aid of references to the interviewees’ quotations (translated from Swedish to English) to outline detailed stories of the cases,
enriched with findings from the secondary materials.
In the second step, as data collection and analysis progressed, we engaged in axial coding using the Gioia methodology (Gioia et al.,
2013), to construct more theory-centered second order themes and aggregated constructs from the first order codes. Gioia method-
ology allows for the construction of rich knowledge from qualitative data and adds both rigor and a systematic approach to theory
construction. It also resonates well with our abductive approach as it allows the “systematic combining” of emerging data with existing
theory (Magnani and Gioia, 2023, p. 3; see also Dubois and Gadde, 2002). It has been presented as particularly useful in case studies as
“Compared to unstructured single or multiple case study designs with no methodical data-coding and data-analysis techniques, the GM
provides greater rigor, because it employs a more systematic research approach” (Magnani and Gioia, 2023; p. 2).
While we initially relied on inductive coding of the data, we also became increasingly sensitized by the literature summarized in
Section 2. For example, conceptualizing domain knowledge as ‘categories’ by operationalization of the literature summarized in
Section 2.1 (e.g., Bowker and Star 1999; Bechmann and Bowker, 2019) greatly improved our understanding of the trajectories in both
cases, as the knowledge production process during ML involves choosing, creating, and (as we experienced) eventually changing or
replacing these categories when predictive systems are developed and deployed.
In the third step, as our RQ is of a processual nature, we adopted a process research approach (Langley, 1999) to track events in the
cases and understand why they unfolded in a particular way. This involved creation of a process model from the themes and constructs
generated in the second step, by revisiting the case narratives to construct a graphical model as we incorporated elements of the
process illustrating the themes, constructs, and their relations. During this stage, there were constant iterations between literature and
data. This data analysis process was facilitated by the use of tables and matrices to refine the identified concepts, and the development
of tentative conclusions to capture the identified phenomena (Miles and Huberman, 1994). In this stage, we also structured the
findings in line with the aggregated constructs, which are presented together with an overview of the coding in Fig. 1. Additional
quotations from the interviews and secondary data sources are presented in Appendix B.

**Results**

The main findings of this study concern three key mechanisms: consolidation, algorithmic mediation, and naturalization. These
mechanisms are discussed in more detail (along with the codes and second-order themes that inform them) in Subsections 4.1 to 4.3,
and a summary of how they were manifested in both cases is provided in Table 1.

```
Fig. 1. Results of the coding.
```

_Consolidation_

The municipality in Case A had previously engaged in robotic process automation projects and regarded ML as a natural addition to
these technologies. The purpose of the ML project was not to automate decision-making, but to augment task handlers’ daily work, by
supplying them with predictions based on textual data. There were two main types of desired predictions according to the participants
in Case A: single-label binary classification of whether a text indicates the presence of urgent risks of harm to children or not, and multi-
label classification of the ‘type’ of harm involved. The domain knowledge used to inform the work stemmed from the everyday
practices of social workers and child welfare officers. These professionals work in a local government environment subject to national
regulations issued by the Swedish National Board of Health and Welfare (2022) in formal documents that provide classifications
reflecting the knowledge and practices of the domain. Since the textual data had to be manually labeled by the project participants to
use for supervised learning, this process was described as highly iterative, as the domain experts heavily engaged with the data and
created labels. The project members reported that they spent most of the project time labeling data. The final dataset consisted of 540
paragraphs of text, with a maximum of 220 words per paragraph, divided into seven categories in addition to the binary yes/no
category.

```
“We entered the project with a human logic that we needed to translate into a semantic model.”  Digital strategist, Case A (I2).
```
In contrast, in Case B, the purpose was to train a ML model based on email data, to automatically classify incoming emails and
forward them to the correct recipients within the Tax Agency. By automating the classification of emails, the aim was to acquire a
higher rate of correct email classification than in the current practices, involving citizens using a drop-down list in a web form. The case
was part of a larger strategic effort to use AI tools for data analytics. The domain knowledge stemmed from a dataset consisting of 1.
million The project members soon realized that the data was of poor quality and the existing labels were not suitable for training a
high-performing model. To generate a higher quality dataset and enable its use to train a classifier several changes were made. First, a
smaller sample with 7000 emails was selected. Then the emails were manually labeled by a group of people with good overviews of the
organization. The project members in Case B described a similar process of change in mindset as those in Case A when working with
ML:

```
“We switched from a task-based structure where the texts [in a category] are unrelated to another logic that departs from the text
content: topic and intention.”  Data analyst, Case B, (I13).
```
In this phase the interviewees highlighted needs to engage in dialogue with a small, motivated group of people in the organization
to enable _knowledge composition_ , and avoid fragmentation with too many diverging opinions during what we refer to as _label alignment_ ,
as domain experts seek consensus during data annotation.

_It [the data labeling] requires the people who work with the data to have the same mental image when they perform the annotation.
Otherwise, training the model will become chaotic._  Data Analyst, Case B (I11).
To reach consensus regarding ground truths, the group members all annotated the same set of exemplary texts, and then compared
their labels in Excel worksheets. As noted by I24, it was challenging to include new people in these types of processes as they had not
participated in the consolidation process and thus needed to align with the current consensus.

_Algorithmic mediation_

The proposed solution in Case A was to train a model using supervised learning by manually labeling the data, then applying these
classifications in transfer learning (via a Swedish version of the pretrained XLM-RoBERTa model) in a no-code platform supplied by a
vendor specializing in deep learning (I6, I8). The project participants soon realized that to use the mentioned categories, the text data
(and on some occasions the categories) had to be altered.

**Table 1**
Summary of case narratives in relation to the aggregated constructs.

```
Mechanism Case A: Identifying signs of harm in text data Case B: Classifying e-mail destinations
Consolidation Knowledge was composed of text data based on reported concerns
about child safety in the Social Service department. These reports
were split into paragraphs and labeled based on categories provided
by the National Board of Health and Welfare. Interviewees described
a switch from a ‘human’ logic to a semantic logic.
```
```
Knowledge was composed from a sample of mails. Interviewees
described a switch from a task-oriented structure to a logic-oriented
structure based on topic and intention during the data labeling, to
create common ‘mental images’ among the data annotators.
```
```
Algorithmic
mediation
```
```
Two types of models were trained: one identifying indications of risks
of imminent harm, and one identifying types of harm. Data
annotators altered existing categories by merging and removing
poor-performing categories, based on model evaluations.
```
```
Models were trained to distinguish between different email
recipients. They performed well but reportedly had low sensitivity to
contextual changes.
```
```
Naturalization The ML project, intended to augment case handlers’ work, was
difficult to integrate with current practices. The project was not
aligned with overall strategic goals and other digital transformation
efforts of the organization. It also diverged from legal, ethical, and
accountability perspectives.
```
```
The ML project’s purpose was to automate distribution of emails
coming into the agency. The initiative was attuned to the
organization’s core values and other strategic data analytics efforts.
The original practices used to categorize email destinations were
entirely omitted.
```

_“For example, we have this text with 200 words and we want to categorize it based on seven categories...Sometimes this categorization is
very simple, but sometimes maybe you’re more unsure. How should we categorize this text? Then I marked it, and when we met in our
annotation group, I said: ‘I reasoned like this, would you do that?’ ‘Oh, wait, said [I1], I have a similar case here, and I reasoned like
this.’”_  Organizational developer, Case A (I3).
As annotated training data were uploaded and used to train a model in the platform, the domain experts evaluated the output in
terms of ROC curves and confusion matrices (which are commonly used to assess ML models’ performance). The binary classification
model performed well, providing “a level of 86 % accuracy in predictions” (illustrated by screenshots of performance measures in the
secondary materials). The domain experts also identified categories that the model failed to generate any meaningful predictions from
by examining instances of wrongly classified texts. The informants described the need to structure the texts used to train the model to
conform to the algorithmic output, as the texts had to be as similar to each other as possible in terms of shape and structure, but also
display enough variance to be distinguishable for a model. Consequently, some categories related to practices that models had dif-
ficulties separating were omitted. Examples included some routines based on locations of (for example) harmful incidents, such as in a
household or school. As types of locations were not always explicitly stated in a text, they were not used to label any data. Moreover,
while ROC curves and confusion matrices indicated the models’ performance, the domain experts also explained that they had to
manage a trade-off between prediction performance and meaningful results, entailing a loss of nuances as indicated by the mentioned
example of locations. Regarding the ML model’s iterative enhancement, the project members described in detail how the domain
knowledge was transformed through implementation of the predictive systems, in an interesting process involving the alteration of
categories in data labeling.

```
“We changed the whole structure of the [domain knowledge] used by 95 % of all municipalities.”  Organizational developer, Case A
(I1).
```
This quotation reflects how _model evaluations_ led to changes in the domain knowledge, manifested in the form of _alterations of data_
and categories. In addition to removing certain categories as explained above, as some categories resulted in better model performance
than others and some inputs that were semantically similar had mixed effects on the output, the group experimented with merging
them.
The interviewees associated with Case B provided similar accounts regarding the use of algorithmic outputs as feedback for
iteratively altering the data:

_“The confusion matrix enables us to see limitations in individual categories. That indicates whether we need to change certain categories.
Maybe we need to split one category into two?... ...that’s how we work with the algorithmic output.”_  Data scientist, Case B (I12).
While the knowledge base used in Case B was more static than in Case A, the interviewees also reported a slowness in the process of
getting the model to classify new email topics, such as applications for tax relief during the Covid-19 pandemic.

```
“...in three weeks, the model had to be capable of handling topics about Covid-19 tax relief, but we had no data about that.”  Data
analyst, Case B (I13).
```
Thus, the models were sensitive to new forms of categories and changes in the external environment. Nevertheless, the Tax Agency
had mature data governance structures with a tradition of analytics and data warehousing, and, as part of their overall AI work, they
assembled new structures to facilitate data sharing and access. To monitor data relevance and prevent decay, the agency also had an
established AI council – with tasks such as monitoring the organization’s data legacy, including records of how, when and why data
were created (mentioned by I15 and I16).

_Naturalization_

Interviewees from both cases described efforts to deploy the ML models in their organizations and the tensions involved when
integrating the newly created knowledge with current strategies and practices. Many of these tensions were directly related to the
introduction of probabilistic ML models, which diverged from established knowledge bases.
The trained models in Case A performed relatively well, but deploying them in the organization raised several challenges. As the
output of the trained ML models was black-boxed, concerns about accountability in their use were raised by the project members.
While they argued that ML-mediated identification of signs of harm in the text data would augment the work rather than automate it
and replace social workers, leading NLP experts from the ecosystem expressed concerns regarding rapid upscaling of the solution in
other municipalities, and that it might be necessary to re-consider its application:

```
I’m not convinced that this particular area is suitable for the use of AI at the moment... If multiple municipalities are developing models
for this...we suddenly have machines that make decisions in very sensitive areas.  Head of research (I20).
```
Interviewees in both cases also mentioned a problematic lack of AI competence within the organization, particularly among
managers. Thus, they highlighted the importance of participating in the overall AI ecosystem (including external experts and interest
groups, a data readiness network, and central government actors) to facilitate acquisition of knowledge and increase general
competence. This ecosystem also functioned as a showcase where the latest NLP developments were demonstrated – such as large
language models based on the Swedish language – as these techniques spread rapidly during 2023. For example, I23 and I24 described
how several Swedish language models were currently being developed in collaboration with national government agencies. Thus, in


addition to contributing knowledge and expertise, the AI ecosystem also served as a forum not only to showcase new technology, but
also to legitimize and promote its responsible use.
Meanwhile, some interviewees claimed that the project in Case A enhanced knowledge of requirements to develop AI and ML, but
others were more skeptical and highlighted the lack of structures for knowledge management and low overall AI competence in the
organization. As noted by a project member in one of the secondary data sources, this raised problems when results were being
prepared for use by the organization.

_“How should the results be presented to the staff? Where in the process and where in the system? ‘0.275’ is not a good input for an
administrator.”_  post on social media_._
An internal report from the municipality in Case A highlighted a lack of strategic alignment of the AI project with other initiatives of
the organization, which hampered potential synergism. The project was criticized for its modest scale and dependence on external
resources, which detached the ML project from other initiatives involving digital transformation.

```
“The absence of governance mechanisms for projects with strategic and innovative characteristics seems to be a contributing factor to
difficulties in the AI project in navigating between feasibility, resource management, risks, and effects.”  Internal report, Case A.
```
Meanwhile, although the project in Case A was often described as highly innovative, it also raised questions about the role of
welfare organizations in relation to AI development.

```
“AI requires more strategical decisions.... Should we, as a small municipality be an actor that works with this type of pioneering
technology where there are no standard solutions? Should we invest money, time and resources? It is definitely an appropriate question.
What is our responsibility and role?” – Head of IT and digitalization, Case A (I4).
```
Legal challenges associated with the European Union’s General Data Protection Regulation (GDPR) and the USA’s Clarifying
Lawful Overseas Use of Data (CLOUD) were also frequently mentioned by the participants in Case A. Since the text-based training set
contained potentially sensitive personal data about individuals, the project members spent much effort on manually anonymizing the
content.

```
“We referred to ‘the French man’ [one of the project members] living in the city center when we discussed anonymization. As we act in a
small municipality, everybody would know this phrase refers to [the project member], but it would be difficult for an automatic tool to
understand this.”  Organizational developer, Case A (I3).
```
While the ML models trained in Case A displayed several signs of _divergence_ that posed legal and ethical challenges for their
deployment, in Case B these issues were less pronounced as the aim was to automate a non-sensitive process. The agency relies on the
trust of the population in their tax collection operations and developed frameworks for sustainable and responsible AI to _attune_ the
initiative to their commitment to their public service ethos, and the agency’s overall strategies (as mentioned by I15 and I16, and
expressed in strategic documents).

_“The Tax Agency has a history of a very high trust among the population, and we’re always very thorough to have trust permeate our
strategies. It’s a success factor for us.”_  AI Strategist, Case B (I15).
The use of ML to sort emails led to a reduction in the agency’s number of inboxes, as described by I16: “One inbox instead of 15”. A
downside of the previous, manual approach was that citizens needed to know what certain predefined categories meant. They mis-
classified the topic about 50 % of the times they used the previous system, and in worst-case scenarios an inappropriately qualified
administrator would give incorrect responses to mails. These statistics were cited in favor of the use of predictive systems, provided
they are more accurate, but employees tended to have lower tolerance of automated errors than human errors according to the in-
terviewees. For example, I17 described tensions between how things that used to be classified by humans were now represented by
probabilities generated by ML:

_It [previous practices] used to be black and white. Now, there is a moving grey scale. We’re presented with a probability... ...a sort of
guesswork: we “think” this is [this type] of category...However, the general perception is that we still say things with 100 % certainty._ 
Systems Architect, Case B (I17).
The classifiers were implemented throughout the organization and became the primary sorters in the agency’s management of
incoming messages. The agency also had a strong tradition of data analytics, and the exploration of AI technology became routinely
attuned to their current practices and organizational operations. Nevertheless, although the Tax Agency had a core group with
technical and analytical competence, the associated interviewees reported a lack of AI/ML competence among other employees and
managers, similar to the deficiencies noted in Case A.

```
“When we requested potential AI use cases from the organization, we received either very general statements about automation, or
suggestions that AI could act like some sort of magic wand – automagic!”  AI strategist, Case B (I15).
```
Accordingly, interviewees associated with both cases highlighted the adoption of user-friendly AI tools (e.g., “no-code AI plat-
forms” in Case A, and “analytics as a service” in Case B) during training and deployment of ML models.
While governance issues were less pronounced in Case B, an internal audit report raised concerns about translating the mentioned
AI policies to an operational level. Here, the importance of educating top managers about the fundamental capabilities and limitations
of AI to ‘demystify’ (I16) it was emphasized by the interviewees. Measures to address such issues included outlining strategies for


information and data sharing. As the Tax Agency started to use ML and NLP, they also developed strategies to coordinate the work with
other initiatives of the organization, so the AI work would not be conducted in silos.

```
“It’s easy to happily start doing POCs [proof of concepts] with a few initial AI solutions, but pretty soon you encounter issues of scaling,
data reuse and quality etc. Then you need to organize data management and this is something that many [organizations] need, but it’s a
giant hill to climb.”  Organizational developer, Case B (I16).
```
Hence, while both cases gave insights into a similar process of knowledge production with the switch to predictive ML systems,
differences in their scopes and trajectories facilitated discovery of factors that enabled the attunement to, or divergence of, this
knowledge in relation to organizational operations and practices.

**Discussion**

The selected cases and methodological approach proved suitable for eliciting informative narratives, identifying key themes in
them, and generating constructs that provide deeper understanding of the focal processes and answer the RQ, “ _How is organizational
knowledge generated in machine learning initiatives?”_.
We build on and extend prior research focused on the fusing of domain knowledge with ML, highlighting how this remains a crucial
challenge in leveraging data effectively within organizations (Waardenburg et al., 2022). Specifically, our cases demonstrate how the
creation of organizational knowledge in ML initiatives is an intricate process that involves interplay between domain knowledge and
machine knowledge. Over time, this cyclical exchange leads to the evolution of a new breed of knowledge that is deeply rooted in data
but informed by human understanding and expertise. The findings from our studied cases, particularly the observed impact of ML on
organizational knowledge, resonate strongly with emerging literature on how data and algorithms are increasingly challenging and re-
configuring established bases for domain knowledge (van den Broek et al., 2021; Henriksen and Bechmann, 2020). In addition to
validating existing studies, we also extend them by providing a novel processual view involving three mechanisms (consolidation,
algorithmic mediation, and naturalization) illustrated in Fig. 2 and further outlined below.
_Consolidation_ entails the formalization of appropriate knowledge as it must be suitably structured for labeling using classification
systems drawn from the domain where an ML system will be trained and applied. In associated practices, actors strive to align their
labeling consensually. Identification of this process significantly extends the previously recognized role of domain experts in data work
(e.g., van den Broek et al., 2021) and observations that divergence in their judgements during ground truth construction can hinder the
efficient training of ML systems (Lebovitz et al., 2021). In this phase, data requirements direct the knowledge creation process by
providing the epistemic structures required for training ML models. The process includes a transition of logics from those embedded in
the setting and conditions that influenced the domain knowledge’s creation to the formal logic required to use the knowledge to train
algorithms (e.g., a semantic logic in NLP cases). This process goes deeper than simply reflecting the current domain knowledge, as
ultimately it is a datafication of suitable categories (Bowker and Star, 1999; Bowker et al., 2010; Bechmann and Bowker, 2019).
_Algorithmic mediation_ refers to the performative role of ML models, as manifested during their evaluation. When domain knowledge
is referred to as ‘data’, it is subject to further alterations to improve the ML models’ predictive performance. The domain knowledge
has then acquired ‘machine’ form, in which it is subject to changes by iterations between performance measures and data alterations.
Here, categories in the form of data are altered (e.g., by removing or merging certain categories) to improve models’ predictive

```
Fig. 2. Illustration of the knowledge-creation process when developing ML in organizations.
```

performance. As noted by Akrich (1992, p. 221), “Once technical objects are stabilized, they become instruments of knowledge.” Then
datasets and algorithms are clearly not mere passive communicators of established knowledge: they actively shape the knowledge used
to create or inform them (Barley, 2015). In these processes, altered categories enable persistent patterns of change and action, facilitate
the organization of knowledge, and manifest as epistemic architectures (Flyverbom and Murray, 2018) that constitute “infrastructures
of knowing” (Monteiro, 2022). Thus, our findings extend understanding of how “material practices are implemented and routinely
embedded in everyday life” (May and Finch, 2009, p. 550).
Finally, when ML models are deemed to provide sufficient performance, they can be _naturalized_ by attuning the new knowledge to a
milieu through the replacement, complementation, augmentation, or enablement of new categories and practices. Thus, the models
become naturalized in a community’s environment and start to play established roles in their working routines. In addition to the rise
of data annotator professions in organizations, those whose tasks are to be augmented by predictive algorithms must now be prepared
to work with ML. However, the newly-created knowledge may be rejected in a process we call ‘divergence’ Examples of causes of such
divergence reported from our cases involved legal, ethical, and accountability issues (“normative divergence” as per Straub et al.,
2023), but also a lack of attunement of ML to current practices and operations. Echoing Aaltonen et al. (2021), we show how data are
generated and edited as domain knowledge is consolidated into machine knowledge, and gain relevance when they are attuned and
naturalized in a domain where they form organizational realities (see also, Østerlie and Monteiro, 2020). Here, we extend previous
research by showing how ML not only generates knowledge as outcomes (cf. Shollo et al., 2022), but also becomes the vessel in which
these outcomes manifest and hence must be considered as part of them (Latour, 2002).

_Theoretical contributions_

The main contribution of this study is a processual theory that explains how organizational knowledge is created in ML initiatives
via three mechanisms that we call consolidation, algorithmic mediation, and naturalization. Recognition of these mechanisms, which
have not been clearly distinguished in previous discourse, marks a significant theoretical advance by tying together notions of
knowledge as categories and practices (Bowker and Star, 1999; Bowker et al., 2010; Wenger, 1999) with emergent literature on the
social and situated character of data and algorithms (Vial, 2019; Smith, 2020; Alaimo and Aaltonen, 2023; Alaimo and Kallinikos,
2021; Flyverbom and Murray, 2018; Mikalsen and Monteiro, 2021).
Our findings partially align with previous literature, summarized in the Background section, highlighting challenges in labelling
domain experts’ knowledge based on rich practices for algorithmic processing (Lebovitz et al., 2021). We extend these studies by
introducing the notion of consolidation practices that explain how these experts form consensus regarding the content of their data,
although knowledge is always situated and contextually bounded. We show how ML development is highly dependent on negotiation
and consensus-building practices involving the composition of knowledge, and aligning labeling efforts. Thus, to paraphrase Langefors
(1980), data alone cannot carry information; knowledge generation is dependent on people sharing common world-views.
In addition, our processual view extends previous research on the knowledge creation process associated with ML development (e.
g., Shollo et al., 2022; Grønsund and Aanestad, 2020) with insights into the co-constituent relationship between domain knowledge
and machine knowledge in the public sector. By doing so, our study addresses recognized needs for empirical investigations of how
new structures in government are created as use of AI technologies increases (Wirtz et al., 2021). Following the changes in categories
that domain experts use during ML development, as recommended by Bechmann and Bowker (2019), we show how certain features are
included and others excluded during the ML workflow, partly due to the rigid requirements for ML algorithms to generate relevant
predictions. In this manner, we illustrate how algorithmic mediation directs knowledge production (Henriksen and Bechmann, 2020,
p. 805; Aaltonen and Stelmaszak, 2023) and stimulates the replacement, change and/or emergence of new practices.

_Implications for strategic AI governance in the public sector_

Public sector organizations constitute the backbone of the welfare state through the delivery of essential services and maintenance
of social safety nets. Thus, they play crucial roles in upholding social equity, public health, education, infrastructure, and societal well-
being. As these organizations are increasingly using AI techniques such as ML to support their operations, there are urgent needs to
elucidate the implications of their use. This study contributes new empirical insights into the use of ML in government as requested by
several scholars (e.g. Sun and Medaglia, 2019; van Noordt and Misuraca, 2022; Neumann et al., 2024). Our study provides insights into
tensions that occur when the formal structures of public sector organizations (Selten and Klievink, 2024) meet the performative nature
of ML algorithms. Concerns have been expressed about the scarcity of research on, and theoretical understanding of, AI and data
governance research in the public sector (Zuiderwijk et al., 2021). By unpacking and theorizing the process through which new
knowledge is created through the fusion of these worlds, our study addresses these gaps in the literature. In addition, it provides
practical implications for policymakers aiming to harness ML’s potential while navigating the complexities of the associated
transformations.
As data increasingly become the means through which organizations create knowledge via algorithmic practices (Alaimo and
Kallinikos, 2022), our findings highlight the importance of attuning these practices to overall strategies and the public service ethos.
This includes accounting for the contextual character of organizational data in strategic knowledge management efforts, in contrast to
treating data as objective phenomena (Vial, 2019; Smith, 2020). However, it also includes development of human-centric ML systems
that allow for the continuous involvement of domain experts during training and deployment of predictive models. Such attunement is
becoming increasingly important as diverse actors in both the private and public sectors are developing and implementing large
language models in emerging AI ecosystems. Echoing Pachidi et al. (2021), the outcome of such implementations ultimately depends


on if, and if so how, relevant actors conform to the knowledge regimes that emerge following sociotechnical transformations, and the
organizational structures that influence ML implementation. In the politically governed public sector, this raises questions about the
institutional configurations required to align these knowledge infrastructures to build sufficient capacity to use data-driven, predictive
systems, in effective, responsible, and resilient ways. There are opportunities to attune these systems with ideals of the welfare state by
institutionalizing appropriate governance mechanisms (K ̈onig and Wenzelburger, 2020), but also causes for concern about the po-
tential associated disruptions to its foundations.

_Limitations and further research_

As our results are based on a study of two cases in Swedish public sector settings, their direct applicability is inevitably limited by
these settings’ contextual conditions. While the case study approach is not intended to provide broad generalizations, the cases
provided substantial insights of both theoretical and potentially practical interest. Moreover, as AI and ML systems are not developed
in isolation, the results were enriched by interviews with additional actors from the surrounding AI ecosystem. We believe this
broadened both the empirical base of the study and its relevance to literature on AI in IS and digital government.
While our main theoretical contribution here consists of a process framework explaining the research phenomenon, we
acknowledge the temporal boundaries of such studies, as explained by Dubois and Gadde (2002, p. 557): “Studies focused on processes
have to come to an end, whereas the processes in the real world continue.” As AI and ML techniques rapidly evolve, we encourage
further study of our proposed mechanisms in other settings. We emphasize the need to follow the technology and conceptualize its
‘material biography’ (Leonardi and Barley, 2008, p. 167) in institutional settings in future analyses of the intersections and interactions
between domain knowledge and machine knowledge. We also particularly welcome studies that extend our findings related to the
characteristics and functions of AI ecosystems to additional settings, and the emerging strategic uses of generative AI systems, which
are much less dependent on structured data.

**Conclusion**

The purpose of this study was to enhance understanding of the processes involved in generation of new domain knowledge via ML.
To do so we addressed the RQ _How is organizational knowledge generated in machine learning initiatives?_ through an exploratory study of
two cases of ML development in Swedish public sector settings. This resulted in the identification of three mechanisms (consolidation,
algorithmic mediation and naturalization) that extend our theoretical understanding of how ML systems contribute to knowledge-
creation in organizational settings and the tensions involved. These theoretical contributions pinpoint the dynamics between expert
consensus and the performative nature of data and algorithms, while underscoring the need for legitimacy when this knowledge is to
be adopted in the public sector.

**CRediT authorship contribution statement**

**Leif Sundberg:** Writing – review & editing, Writing – original draft, Validation, Methodology, Investigation, Conceptualization,
Data curation, Formal analysis, Visualization. **Jonny Holmstr** ̈ **om:** Writing – review & editing, Writing – original draft, Methodology,
Conceptualization.

**Declaration of competing interest**

The authors declare that they have no known competing financial interests or personal relationships that could have appeared to
influence the work reported in this paper.

**Appendix**

_Appendix A. 1: Interviews_

```
Positions of the 25 interviewees in the 24 interviews.
```
```
Position(s)
Case A
Organizational developer no. 1 I1, digital strategist I2, organizational developer no. 2 I3*
Digital strategist I
Organizational developer I
Head of IT and digitalization I
Organizational developer I
( continued on next page )
```

```
( continued )
Position(s)
Organizational developer no. 3 I
Data scientist I
Digital innovation specialist I
AI solution engineer I
Solutions architect I
Health Care Manager I
Case B
Data analyst no. 1 I11, and Data scientist I12*
Data analyst no. 2 I
Task handler I
AI strategist I
Organizational developer I
Systems architect I
Product owner and AI trainer I
AI ecosystem
Head of strategic initiatives I
Head of research I
Digitalization strategist I
Statistician I
NLP lab leader I23 and Researcher I24*
Product owner, AI hub I
*indicates that more than one interviewee participated.
```
**Appendix A2. : Secondary data**

```
Secondary data Description
Social media and web data Content from LinkedIn, MyAI.se, websites, etc.
ML models Snapshots of ROC curves and confusion matrices of the trained models.
Documents Power point presentations of the cases by project members. Internal government reports. Documents of work practice routines.
NLP meetings Seminars and talks where participants from the cases presented and discussed their projects.
```
_Appendix B:. Quotations and second order themes_

```
Quotations Second order themes
“[The framework from the National Board of Health and Welfare] contains about 140 categories... ... We quickly realized that annotating
[140 categories] would take tremendous effort.” I
```
```
Knowledge
composition
“We have a lot of data associated with individual cases. So, we’ve had discussions with our legal councilor. What type of data are we
allowed to use, and how?” – I
“Data is said to be the new gold, but it can be really boring to work with. So, it is far from glamorous, but it pays off.” – I
“A lot of our [data scientists] work was focused on trying to understand what they [domain experts] wanted to teach the model. At the end
of the day, it is a classification problem.” I
“They [the domain experts] realized that when selecting categories, it is important that they are mutually exclusive.” I
“We started with 30 categories associated with inboxes with historical” I
“Initially there was a drop list where the citizen chooses the area their question belonged to. But that was hopeless as it was based on an
internal perspective.” I
“It [the data] needs to be as similar as possible when it comes to structure and form, to achieve as good results as possible.” – I1 Label alignment
“95 % of the Swedish municipalities use the same framework to classify harm. We needed to change this framework from a human to a
semantic logic, so a language model could make predictions. Hopefully additional municipalities think this is a good thing, and that it
could be further improved.” – I
“Human logic and semantic logic are two different things. For example, it is difficult for a machine to distinguish between harm at home,
in the school, or wherever. But it can differentiate between different types of harm.” I
“We started with a joint workshop to create a common point of reference. We annotated some cases together to create a basis for the data
labeling.” I
“After making a first schematic of the categories, we sit in groups of three or four people, and annotate the same example[s]. Then we can
immediately see what examples people annotate differently.” I
“In a way it [data labeling] is a form of ontology modelling.” I
“If we are to choose from two [labels] that are indifferent in relation to the algorithm the main point is to reach consensus.” I
“It [the model] should send a signal to the employees. Not that ‘this is right’, but a hint that it may be something there. And then it is better
that a hint is sent a few times too often than too few. At the same time, it cannot be too fine-meshed. We use thresholds [a method to
adjust a model’s sensitivity] to adjust this.” – I
```
```
Model evaluation
```
```
“We thought we were going to work with a variant of BERT, but they [the data scientists] explained that the XLMR-variant was better for a
reason I forgot, but it made sense, so we shifted to XLMR.” – I
“When we were looking at the evaluation results from the first models, they [the domain experts] understood directly like, this threshold is
not good because we’re going to have false positives in this category.” I
( continued on next page )
```

```
( continued )
Quotations Second order themes
“By looking at precision and recall, we can see if there are any insights in the data, or if we need to intervene and adjust certain categories.”
I
“We have the model in the loop [during data labeling].” I
“It became very slow to change the model when we needed new categories.” I
“The reason why our [Swedish Royal Library’s] models are used is because we have superior data.” I
“We needed to feed the model with data of a high quality. So sometimes we said, ‘No, let’s remove this text, it’s too complex and will
confuse the model.’ I
```
```
Data alteration
```
```
“In some classes with a lot of data, there was some signal, but some categories had very little data. And then you have to ask the question:
should you just ignore them?” I
“And then they [the domain experts] looked at the model results... ...We will just join these two categories and try another experiment.” 
I
“When you focus on one [category] you may lose track of another. These are communicating vessels, and there’s always a risk for
suboptimization.” I
“What we’ll do is to stop using these categories, start from scratch and think in different dimensions.... We’ll focus a little more on what
the algorithms want.” I
“It was better to use greater algorithms and reduce the amount of data.” I
“The AI model makes systematic rights, and systematic errors. The advantage is the systematization, as we get a quantification of the
errors, in contrast to manual handling. We get new tools to look at, analyze, and identify errors. Then we can have a clear dialogue
with the organization: can you accept an accuracy of 80 % here?” I
```
```
Attunement
```
```
“You get forced to use data as a point of departure when you build an AI-model, then that knowledge is used to shape your organizational
processes.” I
“One aspect when you work with historical data is the context where this data was created, and how. There’s an expert group with the
specific task to examine the context where our text data were created.” I
“Data governance includes creation of conditions to work with AI. [Descriptions of established structures for data, information,
architectures]” I
“Our whole strategy revolves around trust for the agency and for society at large in relation to democratic aspects.” I
“We have a project named the data readiness workshop, with the ambition to raise the data readiness in the public sector. It consists of
[references to numerous actors in the AI ecosystem].” I
“The AI platform used [in case A] enabled the creation of models without coding.” I
“Reaching a point where data labeling is an everyday task of a social worker is quite far away.” I3 Divergence
“We need to see data as a strategic resource, and put it on our agenda, and thereby make strategic decisions about how we want to push
forward in our development projects... ...It [a strategic approach] is not there today.” I
“[The municipal board] thought it was a good idea to participate in [AI education], but the learning curve was quite high for them. ...
Many tried to participate but they got a bit put off due to the high complexity.” – I
“An important part of innovation management is knowledge management. How do we create that knowledge... ...and turn it into an
organizational capability?” I
“Even if our data reside in the EU ... the [data storage provider] is an American company covered by the Cloud Act.” I
“When you receive a prediction, you need to present it in a good way for the user.... We need to build some sort of interface.” I
“[The project] is really interesting but it is not strategically relevant.... The use case is not strategically important for the social service
department’s overall digitalization.” II
“AI is good at many things, but to use it when kids are involved in very serious situations... ...I would prefer humans to make these
judgments rather than a machine.“ I
```
**References**

Aaltonen, A., Alaimo, C., Kallinikos, J., 2021. The making of data commodities: Data analytics as an embedded process. J. Manag. Inf. Syst.
Aaltonen, A., Stelmaszak, M., 2023. The performative production of trace data in knowledge work. Inf. Syst. Res.
Abdel-Karim, B.M., Pfeuffer, N., Carl, K.V., Hinz, O., 2023. How AI-based systems can induce reflections: The case of AI-augmented diagnostic work. MIS Q. 47 (4).
Akrich, M., 1992. The de-scription of technical objects. In: Wiebe, J. (Ed.), Shaping Technology / Building Society: Studies in Sociotechnical Change. Bijker and Trever
Pinch.
Alaimo, C., Aaltonen, A., 2023. Strategizing with data: data-based innovations and complementarities. In: Research Handbook on Digital Strategy. Edward Elgar
Publishing, pp. 239–254.
Alaimo, C., Kallinikos, J., 2021. Managing by data: Algorithmic categories and organizing. Organ. Stud. 42 (9), 1385–1407.
Alaimo, C., Kallinikos, J., 2022. Organizations Decentered: Data Objects, Technology, and Knowledge. Organ. Sci.
Alaimo, C., Kallinikos, J., Aaltonen, A., 2020. Data and value. Handbook of Digital Innovation. Edward Elgar Publishing.
Asatiani, A., Malo, P., Nagbøl, P.R., Penttinen, E., Rinta-Kahila, T., Salovaara, A., 2021. Sociotechnical envelopment of artificial intelligence: An approach to
organizational deployment of inscrutable artificial intelligence systems. J. Assoc. Inf. Syst. 22 (2), 325–352.
Ashrafi, A., Constantinides, P., Mehandjiev, N., Thatcher, J.B., 2024. Mobilising new frontiers in digital transformation research: A problematization review. Inform.
Syst. J.
Barley, S.R., 1986. Technology as an occasion for structuring: Evidence from observations of CT scanners and the social order of radiology departments. Adm. Sci. Q.
78 – 108.
Barley, W.C., 2015. Anticipatory work: How the need to represent knowledge across boundaries shapes work practices within them. Organ. Sci. 26 (6), 1612–1628.
Bechmann, A., Bowker, G.C., 2019. Unsupervised by any other name: Hidden layers of knowledge production in artificial intelligence on social media. Big Data Soc. 6
(1).
Biernacki, P., Waldorf, D., 1981. Snowball sampling: Problems and techniques of chain referral sampling. Sociol. Methods Res. 10 (2), 141–163.
Boland, Tenkasi, R.V., 1995. Perspective making and perspective taking in communities of knowing. Organ. Sci. 6 (4), 350–372.
Borges, A.F., Laurindo, F.J., Spínola, M.M., Gonçalves, R.F., Mattos, C.A., 2021. The strategic use of artificial intelligence in the digital era: Systematic literature
review and future research directions. Int. J. Inf. Manag. 57, 102225.


Bowker, G.C., Baker, K., Millerand, F., Ribes, D., 2010. Toward information infrastructure studies: Ways of knowing in a networked environment. Internat. Handbk.
Internet Res. 97–117.
Bowker, G., Star, S.L., 1999. Sorting things out. Class. Conseq. 4.
Brynjolfsson, E., Rock, D., Syverson, C., 2017. Artificial Intelligence and the Modern Productivity Paradox: A Clash of Expectations and Statistics (NBER Working
Paper 24001 No. w24001; p. w24001). National Bureau of Economic Research. https://doi.org/10.3386/w24001.
Davenport T.H and Bean R. (2023). Action and Inaction on Data, Analytics, and AI https://sloanreview.mit.edu/article/action-and-inaction-on-data-analytics-and-ai/.
Cho, J.Y., Lee, B.G., 2022. Creating value using public big data: Comparison of driving factors from the provider’s perspective. Inf. Technol. People 35 (2), 467–493.
Choo, W.C., 1998. The Knowing Organization: How Organizations Use Information To Construct Meaning, Create Knowledge, and Make Decisions, 2nd edn. Oxford
University Press, New York.
Cook, S.N., Brown, S.J., 1999. Bridging epistemologies: the generative dance between organizational knowledge and organizational knowing. Organ. Sci. 10,
382 – 400.
Denton, E., Hanna, A., Amironesei, R., Smart, A., Nicole, H., 2021. On the genealogy of machine learning datasets: A critical history of ImageNet. Big Data Soc. 8 (2),
20539517211035955.
Dougherty, D., Dunne, D.D., 2011. Digital science and knowledge boundaries in complex innovation. Organ. Sci. 23 (5), 1467–1484.
Dourish, P., 2016. Algorithms and their others: Algorithmic culture in context. Big Data Soc. 3 (2), 2053951716665128.
Drucker, J., 2011. Humanities approaches to graphical display. Digital Hum. Quarterly 5 (1), 1–21.
Dubois, A., Gadde, L.E., 2002. Systematic combining: an abductive approach to case research. J. Bus. Res. 55 (7), 553–560.
European Commission (2022). https://digital-strategy.ec.europa.eu/en/policies/enabling-ai.
Faraj, S., Pachidi, S., Sayegh, K., 2018. Working and organizing in the age of the learning algorithm. Inf. Organ. 28 (1), 62–70.
Flyverbom, M., Murray, J., 2018. Datastructuring—Organizing and curating digital traces into action. Big Data Soc. 5 (2), 2053951718799114.
Foucault, M., 2005. The order of things. Routledge.
Gehman, J., Glaser, V.L., Eisenhardt, K.M., Gioia, D., Langley, A., Corley, K.G., 2018. Finding theory–method fit: A comparison of three qualitative approaches to
theory building. J. Manag. Inq. 27 (3), 284–300.
Gioia, D.A., Corley, K.G., Hamilton, A.L., 2013. Seeking qualitative rigor in inductive research: Notes on the Gioia methodology. Organ. Res. Methods 16 (1), 15–31.
Glaser, V.L., Pollock, N., D’Adderio, L., 2021. The biography of an algorithm: Performing algorithmic technologies in organizations. Organization Theory 2 (2),
26317877211004609.
Grønsund, T., Aanestad, M., 2020. Augmenting the algorithm: Emerging human-in-the-loop work configurations. J. Strateg. Inf. Syst. 29 (2), 101614.
Günther, W.A., Mehrizi, M.H.R., Huysman, M., Feldberg, F., 2017. Debating big data: A literature review on realizing value from big data. J. Strateg. Inf. Syst. 26 (3),
191 – 209.
Gualdi, F., Cordella, A., 2024. Artificial intelligence to support public sector decision-making: the emergence of entangled accountability. In: Research Handbook on
Artificial Intelligence and Decision Making in Organizations. Edward Elgar Publishing, pp. 266–281.
Günther, W.A., Mehrizi, M.H.R., Huysman, M., Deken, F., Feldberg, F., 2022. Resourcing with data: Unpacking the process of creating data-driven value propositions.
J. Strateg. Inf. Syst. 31 (4), 101744.
Heidegger, M., 2008. reprint). Being and time, Harper Perennial.
Henriksen, A., Bechmann, A., 2020. Building truths in AI: Making predictive algorithms doable in healthcare. Inf. Commun. Soc. 23 (6), 802–816.
Janssen, M., Brous, P., Estevez, E., Barbosa, L.S., Janowski, T., 2020. Data governance: Organizing data for trustworthy Artificial Intelligence. Gov. Inf. Q. 37 (3),
101493.
Jarke, J., Büchner, S., 2024. Who cares about data? Data care arrangements in everyday organisational practice. Inf. Commun. Soc. 1–17.
Jarke, J., Heuer, H., 2024. Reassembling the black box of Machine Learning: Of monsters and the reversibility of foldings. Methods, Interactions, and Politics, p. 103.
Jones, M., 2019. What we talk about when we talk about (big) data. J. Strateg. Inf. Syst. 28 (1), 3–16.
Jordan, M.I., Mitchell, T.M., 2015. Machine learning: Trends, perspectives, and prospects. Science 349 (6245), 255 – 260.
Keen, J., Ruddle, R., Palczewski, J., Aivaliotis, G., Palczewska, A., Megone, C., Macnish, K., 2021. Machine learning, materiality and governance: A health and social
care case study. Inform. Polity 1–13.
Keller, C.M., Keller, J.D., 1996. Cognition and Tool Use: The Blacksmith at Work. Cambridge University Press, Cambridge.
Kellogg, K.C., Valentine, M.A., Christin, A., 2020. Algorithms at work: The new contested terrain of control. Acad. Manag. Ann. 14 (1), 366–410.
K ̈onig, P.D., Wenzelburger, G., 2020. Opportunity for renewal or disruptive force? How artificial intelligence alters democratic politics. Gov. Inf. Q. 37 (3), 101489.
Kravˇcenko, D., 2023. Towards processual understanding of knowledge boundaries: an ethnographic examination of how professionals (mis-) align, compete, and
collaborate. J. Work. Learn. 35 (3), 265–287.
Langefors, B., 1980. Infological models and information user views. Inf. Syst. 5 (1), 17–32.
Langley, A., 1999. Strategies for theorizing from process data. Acad. Manag. Rev. 24 (4), 691–710.
Latour, B., 2002. Morality and technology: The end of the means. Theory Cult. Soc. 19 (5/6), 247 – 260.
Lebovitz, S., Levina, N., Lifshitz-Assaf, H., 2021. Is AI ground truth really “true”? The dangers of training and evaluating AI tools based on experts’ know-what. Manag.
Inf. Syst. Q.
Lebovitz, S., Lifshitz-Assaf, H., Levina, N., 2022. To engage or not to engage with AI for critical judgments: How professionals deal with opacity when using AI for
medical diagnosis. Organ. Sci. 33 (1), 126–148.
Leonardi, P.M., Barley, S.R., 2008. Materiality and change: Challenges to building better theory about technology and organizing. Inf. Organ. 18 (3), 159–176.
Lewis-Beck, M., Bryman, A.E., Liao, T.F., 2003. The Sage Encyclopedia of Social Science Research methods. SAGE Publications.
Li, Y., Thomas, M.A., Liu, D., 2021. From semantics to pragmatics: where IS can lead in Natural Language Processing (NLP) research. Eur. J. Inf. Syst. 30 (5), 569–590.
Mackenzie, A., 2017. Machine learners: Archaeology of a data practice. MIT Press.
Magnani, G., Gioia, D., 2023. Using the Gioia Methodology in international business and entrepreneurship research. Int. Bus. Rev. 32 (2), 102097.
Marabelli, M., Newell, S., 2012. Knowledge risks in organizational networks: The practice perspective. J. Strateg. Inf. Syst. 21 (1), 18–30.
May, C., Finch, T., 2009. Implementing, embedding, and integrating practices: An outline of normalization process theory. Sociology 43 (3), 535–554.
Medaglia, R., Gil-Garcia, J.R., Pardo, T.A., 2021. Artificial Intelligence in Government: Taking Stock and Moving Forward, 08944393211034087 Soc. Sci. Comput.
Rev.
Meijer, A., Lorenz, L., Wessels, M., 2021. Algorithmization of bureaucratic organizations: Using a practice lens to study how context shapes predictive policing
systems. Public Adm. Rev. 81 (5), 837–846.
Mergel, I., Dickinson, H., Stenvall, J., Gasco, M., 2024. Implementing AI in the public sector. Public Manag. Rev. 1–14.
Mikalsen, M., Monteiro, E., 2021. Acting with inherently uncertain data: Practices of data-centric knowing. J. Assoc. Inf. Syst. 22 (6), 1715–1735.
Miles, M.B., Huberman, A.M., 1994. Qualitative Data Analysis: An Expanded Sourcebook. SAGE.
Monteiro, E., 2022. Digital Oil: Machineries of Knowing. MIT Press.
Neumann, O., Guirguis, K., Steiner, R., 2024. Exploring artificial intelligence adoption in public organizations: a comparative case study. Public Manag. Rev. 26 (1),
114 – 141.
Nikiforova, A., Rizun, N., Ciesielska, M., Alexopoulos, C., Mileti ́c, A., 2023. Towards high-value datasets determination for data-driven development: a systematic
literature review. In: International Conference on Electronic Government. Springer Nature Switzerland, Cham, pp. 211–229.
Orlikowski, W.J., 2002. Knowing in practice: Enacting a collective capability in distributed organizing. Organ. Sci. 13 (3), 249–273.
Østerlie, T., Monteiro, E., 2020. Digital sand: The becoming of digital representations. Inf. Organ. 30 (1), 100275.
Pachidi, S., Berends, H., Faraj, S., Huysman, M., 2021. Make way for the algorithms: Symbolic actions and change in a regime of knowing. Organ. Sci. 32 (1), 18–41.
Pettigrew, A.M., 1990. Longitudinal field research on change: Theory and practice. Organ. Sci. 1 (3), 267–292.
Pi, Y., 2021. Machine learning in governments: benefits, challenges and future directions. JeDEM-eJ. eDem. Open Gov. 13 (1), 203–219.


Rose, J., Persson, J.S., Heeager, L.T., Irani, Z., 2015. Managing e-Government: value positions and relationships. Inf. Syst. J. 25 (5), 531–571.
Seaver, N., 2017. Algorithms as culture: Some tactics for the ethnography of algorithmic systems. Big Data Soc. 4 (2), 2053951717738104.
Selten, F., Klievink, B., 2024. Organizing public sector AI adoption: Navigating between separation and integration. Gov. Inf. Q. 41 (1), 101885.
Shastri, A., Deshpande, M., 2020. A review of big data and its applications in healthcare and public sector. Big Data Anal. Healthcare 55 – 66.
Shollo, A., Hopf, K., Thiess, T., Müller, O., 2022. Shifting ML value creation mechanisms: A process model of ML value creation. J. Strateg. Inf. Syst. 31 (3), 101734.
Smith, G., 2020. Data mining fool’s gold. J. Inf. Technol. 35 (3), 182–194.
Straub, V.J., Morgan, D., Bright, J., Margetts, H., 2023. Artificial intelligence in government: Concepts, standards, and a unified framework. Gov. Inf. Q. 40 (4),
101881.
Sturm, T., Gerlach, J.P., Pumplun, L., Mesbah, N., Peters, F., Tauchert, C., Buxmann, P., 2021. Coordinating human and machine learning for effective organizational
learning. MIS Q. 45 (3).
Sun, T.Q., Medaglia, R., 2019. Mapping the challenges of Artificial Intelligence in the public sector: Evidence from public healthcare. Gov. Inf. Q. 36 (2), 368–383.
The Swedish National Board of Health and Welfare (2022). https://www.socialstyrelsen.se/kunskapsstod-och-regler/omraden/barn-och-unga/barn-och-unga-i-
socialtjansten/barns-behov-i-centrum/material/ Last accessed, June 2024.
Timmermans, S., Tavory, I., 2012. Theory construction in qualitative research: From grounded theory to abductive analysis. Sociol Theory 30 (3), 167–186.
Toll, D., Lindgren, I., Melin, U., Madsen, C.Ø., 2020. Values, benefits, considerations and risks of AI in government: A study of AI policies in Sweden. JeDEM-eJ. eDem.
Open Gov. 12 (1), 40–60.
Tsoukas, H., 2009. A dialogical approach to the creation of new knowledge in organizations. Organ. Sci. 20 (6), 941–957.
van den Broek, E., Sergeeva, A., Huysman, M., 2021. When the machine meets the expert: An ethnography of developing AI for hiring. MIS Q.
van Noordt, C., Misuraca, G., 2022. Artificial intelligence for the public sector: Results of landscaping the use of AI in government across the. European Union.
Government Information Quarterly.
van Ooijen, C., Ubaldi, B., Welby, B., 2019. A data-driven public sector: Enabling the strategic use of data for productive, inclusive and trustworthy governance.
OECD.
Vial, G., 2019. Reflections on quality requirements for digital trace data in IS research. Decis. Support Syst. 126, 113133.
Vogl, T.M., Seidelin, C., Ganesh, B., Bright, J., 2020. Smart technology and the emergence of algorithmic bureaucracy: Artificial intelligence in UK local authorities.
Public Adm. Rev. 80 (6), 946–961.
Waardenburg, L., Huysman, M., Sergeeva, A.V., 2022. In the land of the blind, the one-eyed man is king: Knowledge brokerage in the age of learning algorithms.
Organ. Sci. 33 (1), 59–82.
Wenger, E., 1999. Communities of practice. Cambridge University Press, Learning, Meaning and Identity.
Wirtz, B.W., Weyerer, J.C., Geyer, C., 2019. Artificial intelligence and the public sector—applications and challenges. Int. J. Public Adm. 42 (7), 596–615.
Wirtz, B.W., Weyerer, J.C., Sturm, B.J., 2020. The dark sides of artificial intelligence: An integrated AI governance framework for public administration. Int. J. Public
Adm. 43 (9), 818–829.
Wirtz, B.W., Langer, P.F., Fenner, C., 2021. Artificial Intelligence in the public sector-a research agenda. Int. J. Public Adm. 44 (13), 1103–1128.
Zuiderwijk, A., Chen, Y.C., Salem, F., 2021. Implications of the use of artificial intelligence in public governance: A systematic literature review and a research agenda.
Gov. Inf. Q. 101577.


[[RAW FILES]]