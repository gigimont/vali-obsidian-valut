---
title: "Informed Machine Learning – Learning from data and prior knowledge » Lamarr-Blog"
source: "https://lamarr-institute.org/blog/informed-machine-learning/"
author:
  - "Gabriella Moreira"
published: 2021-02-17
created: 2026-05-20
description: "Informed Machine Learning makes existing knowledge sources usable. This enables companies to profitably integrate specialist knowledge into ML models."
tags:
  - "clippings"
---
© CNStock/stock.adobe.com

Artificial Intelligence holds enormous potential, but it also presents some challenges. One major requirement for training Machine Learning models is the availability of very large amounts of data. Additionally, the learned models must be trustworthy to make reliable decisions. The means to address these challenges often already exist in the form of prior knowledge. The concept of Informed Machine Learning aims to make such existing knowledge sources usable for Machine Learning. This makes it possible to train models even with smaller amounts of data or to reinforce learned models with prior knowledge.

## Making existing knowledge sources usable

Many companies or institutions possess extensive domain knowledge, often presented in the form of analytical models, simulations, or knowledge graphs. These forms of knowledge are utilized in various application areas, as illustrated by the following examples: in climatology, physical formulas are used to describe the thermodynamic properties of air and water. In autonomous driving, traffic scenarios can be recreated using simulations. In text processing, semantic and syntactic rules can be represented in knowledge graphs. All these diverse knowledge sources can be made usable through Informed Machine Learning.

In our research, we have observed that the prior knowledge used in Informed Machine Learning comes from three overarching categories and is represented differently depending on the context. Knowledge often originates from natural or engineering sciences and may be represented, for instance, in equations or simulation results. Another category is world knowledge, which describes language and visual concepts and may be represented in the form of logical rules or knowledge graphs. Additionally, more intuitive expert knowledge can be utilized and may be represented, for example, through direct human feedback or probabilistic relations.

## Informed ML learns models from data and prior knowledge

These knowledge sources can be incorporated into Machine Learning in addition to the actual training data. With such a hybrid information source, the strengths of both data-driven and knowledge-driven modeling can be combined: data can reveal new, unknown patterns, and prior knowledge can incorporate already validated statements, reducing the amount of data needed.

For the technical integration of prior knowledge into Machine Learning processes, there are various strategies depending on the representation and the ultimate goal of knowledge integration. Generally, there are four stages in which prior knowledge can be integrated: in the training data, in the model space, in the learning algorithm, or in the final model (see Figure 1).

![Pipeline EN - Lamarr Institute for Machine Learning (ML) and Artificial Intelligence (AI)](https://lamarr-institute.org/wp-content/uploads/Pipeline_EN.png)

© Lamarr Institute Illustration of the Informed Machine Learning process: In addition to data, prior knowledge is integrated into the Machine Learning process.

If one wants to train models with originally small amounts of data and has access to simulations, it makes sense to use them to generate additional synthetic data. Conversely, if one aims to secure models, validating a trained model using, for instance, knowledge graphs is an option. A strategy for incorporating prior knowledge suitable for both objectives is the incorporation into the learning algorithm through knowledge-based regularization terms, which can originate from scientific equations or logical rules.

## Learning trustworthy models and compensating for small data sets

Informed Machine Learning makes existing knowledge sources usable and integrates them into Machine Learning processes. This enables the training of models based on both data and prior knowledge. The advantages include compensating for originally small amounts of data and securing the learning process against existing knowledge.

For autonomous driving, this means, for example, that in addition to existing data, additional traffic scenes can be simulated and used as extra training data. Moreover, they can be used to validate already learned models. Both contribute to making the learned models more robust, thereby increasing safety in autonomous driving.

While the application of Informed Machine Learning is still in its early stages, the benefits, together with the various application areas and integration methods, promise significant potential. The ML2R competence center (now the Lamarr Institute) is playing a key role in advancing the research on knowledge-integrating Machine Learning approaches.

For more information, refer to the accompanying papers:

**Informed Machine Learning – A Taxonomy and Survey of Integrating Knowledge into Learning Systems** Laura von Rueden, Sebastian Mayer, Katharina Beckh, Bogdan Georgiev, Sven Giesselbach, Raoul Heese, Birgit Kirsch, Julius Pfrommer, Annika Pick, Rajkumar Ramamurthy, Michał Walczak, Jochen Garcke, Christian Bauckhage, Jannis Schuecker. ArXiv, 2019, [PDF](https://arxiv.org/pdf/1903.12394.pdf).

**Combining Machine Learning and Simulation to a Hybrid Modelling Approach: Current and Future Directions** Laura von Rueden, Sebastian Mayer, Rafet Sifa, Christian Bauckhage, Jochen Garcke. IDA, 2020, [PDF](https://www.springerprofessional.de/en/combining-machine-learning-and-simulation-to-a-hybrid-modelling-/17916102).

[[RAW FILES]]