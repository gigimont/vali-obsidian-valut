---
title: Using Knowledge Elicitation Techniques To Infuse Deep Expertise And Best Practices Into Generative AI
source: https://www.forbes.com/sites/lanceeliot/2025/11/09/using-knowledge-elicitation-techniques-to-infuse-deep-expertise-and-best-practices-into-generative-ai/
author:
  -  Lance Eliot
published: 2025-11-09
created: 2026-05-16
description: How can we get AI and LLMs to be domain experts? The prior era of AI devised knowledge elicitation techniques. Those are still good in the LLM era. An AI Insider scoop.
tags:
  - clippings
---
Contributor.

Forbes contributors publish independent expert analyses and insights.

Dr. Lance B. Eliot is a world-renowned AI scientist and consultant.

![Male computer programmers discussing over laptop on desk while sitting in office](https://imageio.forbes.com/specials-images/imageserve/69081d2357aad872e71f643d/Male-computer-programmers-discussing-over-laptop-on-desk-while-sitting-in-office/0x0.jpg?crop=1382%2C1035%2Cx172%2Cy0%2Csafe&width=960&dpr=1)

Male computer programmers discussing over laptop on desk while sitting in office

In today’s column, I address how you can discover hidden best practices that underlie deep expertise and then codify that secret sauce of domain knowledge into modern-day generative AI and large language models (LLMs).

The crux of this vexing matter is that we can lean into the precepts of knowledge elicitation that were well-formulated during the rules-based expert systems era. I realize that some who are steeped in LLMs might balk at using the “dated” approaches from an earlier era of AI. Despite whatever adverse opinion someone has about so-called GOFAI (good old-fashioned AI), there is absolutely crucial value in leveraging tried-and-true techniques of eliciting deep domain knowledge. It can aid in turning generative AI and LLM into a bastion of best practices and deep expertise for a chosen domain.

Let’s talk about it.

This analysis of AI breakthroughs is part of my ongoing Forbes column coverage on the latest in AI, including identifying and explaining various impactful AI complexities (see [the link here](https://www.forbes.com/sites/lanceeliot/)).

Suppose that you want to turn an LLM into an expert within a particular domain.

Perhaps you want to devise an LLM that has deep medical expertise and is especially proficient in urology or maybe neurology. Another possibility might be to shape generative AI to be on par with a fully qualified lawyer in real estate law or be a mental health therapist that is deeply versed in CBT (cognitive behavioral therapy).

What can you do to shift a general-purpose LLM into being steeped in a specific domain?

The usual approach consists of gathering as many documents as you can find that encompass the domain of interest. You digitize the contents and then feed the materials into generative AI. A commonly used infusion technique is retrieval-augmented generation (RAG), whereby you have the AI pattern-match on the added data at run-time rather than when initially doing data training of the AI at the get-go. For more about RAG and other similar techniques, see my discussion at [the link here](https://www.forbes.com/sites/lanceeliot/2025/01/27/heres-how-big-llms-teach-smaller-ai-models-via-leveraging-knowledge-distillation/).

This is all well and good when you can get your hands on codified domain knowledge that happens to be written down somewhere. The problem is that an area of deep expertise doesn’t necessarily have everything written out to the nth degree. In the heads of experts in that domain are all sorts of human-devised rules of thumb.

You might say that the secret sauce of best practices in a domain is often locked away in the brains of those steeped in that domain. The question arises as to how to surface that hidden knowledge that contains best practices and make it tangible and visible so that you can get it into an LLM that is supposed to be superb in the domain at hand.

<video aria-label="Connatix video player" role="application" title="" src="blob:https://www.forbes.com/4eb0310f-04b8-412b-af20-617fdbb310e1" controls=""></video>1/1

You might be aware that during the AI era of knowledge-based systems, there was a great deal of research and practical implementation of domain knowledge elicitation techniques. To develop an expert system, you had to get experts to divulge what they knew. They would have mentally devised numerous tricks of their trade over the course of many years of trial-and-error.

Stepwise, you would work closely with the experts and get them to reveal their seasoned rules of thumb. Elicitation required getting them to talk about their expertise. Another avenue was to present them with problems to be solved and have them write down the rules they used to tackle the problems. Various clever means were crafted to surface the deep domain knowledge that wasn’t found in books and articles.

For those of you who remember the time period just before generative AI took off as a popular technology, there was a good deal of work on advancing machine learning (ML). It was during this focus on ML that researchers began to realize that knowledge elicitation still deserved to be at the forefront of AI advancements.

Indeed, a research paper undertook a helpful macroscopic look at the intertwining of ML and knowledge elicitation, doing so in an article entitled “A Survey of Domain Knowledge Elicitation in Applied Machine Learning” by Daniel Kerrigan, Jessica Hullman, and Enrico Bertini, *Journal of Multimodal Technologies and Interaction*, 2021, as per these salient remarks (excerpts):

- “Eliciting knowledge from domain experts can play an important role throughout the machine learning process, from correctly specifying the task to evaluating model results.”
- “Imbuing modeling with domain knowledge -- declarative, procedural, and conditional information that a person possesses related to a particular domain -- is a common goal.”
- “Our survey coded 73 elicitation paths found across 28 papers and analyzed the trends that emerged in these paths when comparing the paths where elicitation was performed for problem specification, feature engineering, model development, and model evaluation.

I will highlight how you can readily use knowledge elicitation in combination with getting generative AI and LLM up to speed in a desired domain.

In conferring with a successful stock trader, suppose you decided that it would be useful to tune an LLM toward being a deep expert in picking stocks.

The first step would be to choose an LLM and see what the AI has already been data-trained in regarding stock trading. There is no sense in reinventing the wheel if the AI is already fully loaded about the domain and ready to be used as is. I went ahead and opted to do this case study with OpenAI’s immensely popular ChatGPT. I could have selected some other LLM, but I just thought it would be a suitable choice for my readers overall.

Upon doing various prompts and conversations with ChatGPT, I was able to determine that a lot of the conventional materials about stock picking had obviously been data-scanned at the initial development of the LLM. This was useful to see. I say that because otherwise, you would have to bring the LLM entirely on board with whatever domain you are working with.

Doing so from scratch can be time-consuming and onerous. There is, though, an upside to using an LLM that isn’t versed in the domain of choice.

You see, once you start to elicit the hidden knowledge of best practices and then ingest that into the AI, there is a sizable chance that conflicts will arise. The LLM will already have some predetermined patterns about the domain, and you will have to potentially lock horns with those aspects. It’s a tradeoff as to whether a less-versed LLM is a better or worse choice than going with a highly versed LLM, and you’ll need to make that decision based on the domain you’ve chosen and which AI you wish to use.

After doing a deep dive into what ChatGPT seemed to have about picking stocks, I realized that the secret sauce of the stock trader was not already in the AI. That is not a surprise. This particular stock trader has crafted his own set of rules about picking stocks. No one else necessarily knows or abides by the rules he has come up with.

I am not saying that his rules are unique and unheard of. I am only noting that the AI didn’t have the rules I am about to show you, and it is not surprising that the LLM wouldn’t already have them in hand. I will only show you a few of the rules, due to space limitations for this discussion.

I manually went through many of his stock picks with him. We jointly explored his historical performance. I asked direct questions about what made him pick a stock, along with why he didn’t pick some other stock. This is a verbalization or “speaking aloud” protocol of performing knowledge elicitation. It has its ins and outs and strengths and weaknesses.

For example, when you get an expert to verbalize what they do, they might be on their guard about saying what they really do. If they are performing their tasks by guesswork, that would look bad if others knew what they were doing; they don’t want to be embarrassed or called out. In that sense, the expert might make up fake rationalizations and tell you that’s how they do their work. You are then going to falsely or mistakenly rely upon something that isn’t the true state of the matter.

This is often why poorly performed knowledge elicitation led to expert systems that couldn’t function on par with the domain experts. The expertise or rules elicited were rationalizations and not what the experts truly did. Be cautious and do not fall into that kind of trap.

Here are two example rules that I was able to surface and then double-checked as being the actual rules being utilized by the stock trader.

- **Earnings Momentum Rule** -- If a company has shown at least three consecutive quarters of earnings growth and the growth rate is accelerating, then consider it a buy candidate, unless the price-to-earnings ratio (P/E) exceeds 30.
- **Sector Rotation Rule** -- If capital inflows are shifting into a particular sector (e.g., tech, energy) and that sector has outperformed the market for two consecutive months, then favor stocks within that sector unless macroeconomic indicators (e.g., interest rates, inflation) signal an upcoming contraction.

I was able to identify lots of rules akin to those two rules.

The next step entailed getting these rules into the LLM.

This is a prompt that I used:

- **My prompt:** “You are going to be a stock trader with your own special rules about the picking of stocks. I am going to provide you with those special rules. Once I enter the rules, provide a response showcasing that you have the rules and are ready to make use of them.”

You can enter the devised rules as prompts, or put them into a document and use RAG, or you can even encode them into a structured, machine-interpretable format such as JSON or YAML.

The earning momentum rule would look something like this in JSON:

- { "name": "Earnings Momentum Rule", "if": \[ "Company has >= 3 consecutive quarters of earnings growth", "Growth rate is accelerating" \], "then": "Consider as buy candidate", "unless": "Price-to-earnings ratio > 30"}

Let’s take a big picture perspective for a moment.

I could have begun the entire knowledge elicitation process by first having the AI confer with the stock trader and identifying the initial round of rules. Generally, I prefer to start the process on a human-to-human basis. This usually gets the domain expert into a suitable mood and mode of being involved in knowledge elicitation.

The icing on the cake then happens when the domain expert does the follow-up work with the AI. The experts are usually pleased to see how their rules have been codified and echoed back to them. Furthermore, they typically relish verifying the rules, along with the AI often stirring them to think of additional rules.

Thus, yes, I like to do the upfront bootstrapping on a human basis, but, if needed, the approach can be done on human-to-AI first and then followed by human-to-human. One thing is to make sure that you do both paths. I realize it might be tempting to do just one path. The odds of getting this done wisely and completely are better if you proceed with both pathways.

If the domain includes the use of data by the expert, another useful step consists of collecting the data and having the LLM try to do pattern detection on the data. The idea is that you want the AI to inspect the relevant data, figure out patterns, and attempt to devise rules according to those patterns.

I went ahead and collected data that included factors such as Trade ID, Date of Trade, Stock Ticker, Trade Action, Price, EPS Growth, P/E, Sector Trend, Sentiment, Insider Activity, Market Index, and so on.

Here’s what I told the AI to do with the data:

- **My prompt:** “You are to inspect the following data and look for patterns associated with the stocks and the trading of the stocks. First, try to identify the potential rules underlying why a stock is being traded. Second, compare the rules to those that you already have as a result of the knowledge elicitation effort. Third, indicate if the already articulated rules seem to explain the trades. Fourth, identify any additional rules that might further explain the trades.”

An interesting new rule that the AI came up with was this:

- **New Rule: Stop-Loss Discipline Rule** -- If a stock drops more than 8% below the purchase price, then sell automatically, regardless of future outlook.

I discussed the rule with the stock trader. It was somewhat surprising at first glance and not a rule that the stock trader said they personally used. After mulling over the rule and drinking a glass of fine wine, the stock trader indicated that it is a worthy rule and can be added to the set.

I trust that you can see how knowledge elicitation of human experts can be undertaken in a chosen domain in an effort to inform an LLM on human-held deep expertise.

In a subsequent discussion, I will go over the ways to test the derived rules and decide whether the AI is ready as a presumed expert in the domain.

I’ll mention a bit of a twist on this topic. There is a great deal of debate about using LLMs as an expert, often referred to as a *synthetic expert*, to distinguish the notion of expertise embodied by a person versus by AI. One viewpoint is that no matter what you do, until we reach artificial general intelligence (AGI), which I discuss at [the link here](https://www.forbes.com/sites/lanceeliot/2025/10/29/the-haunting-story-of-ai-thats-been-dumped-into-the-agi-graveyard-but-might-get-remarkably-resurrected/), you aren’t going to have an AI that is on par with a human expert.

This brings up the classic question about narrow intelligence, namely, whether you can have a narrow form of “intelligence” in an AI that performs satisfactorily or whether you must also have general intelligence too.

An argument is often made that contemporary LLMs do have a semblance of general intelligence; therefore, they are a good place to infuse deep domain expertise. But you might disagree that current AI has enough general intelligence and be insistent that only once we arrive at AGI will this precondition be properly met. It is a contentious twist.

Meanwhile, AI developers are proceeding to use knowledge elicitation and aim to infuse LLMs with surfaced best practices and gold nuggets within chosen domains. The work continues while the debate heatedly ensues.

As the great American writer and philosopher Elbert Hubbard once remarked: “The best preparation for good work tomorrow is to do good work today.” Go ahead and do good work with AI today, and it will hopefully dovetail into even better work in the tomorrows to come.

FORBES’ FEATURED Video

[[RAW FILES]]