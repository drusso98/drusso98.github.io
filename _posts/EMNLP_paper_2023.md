---
layout: post
title: 🥃 VerMouth on the rocks, fake news on thin ice — ready for a cool conversation?
date: 2023-11-22 15:56:00
description: EMNLP 2023 paper announcement
tags: EMNLP2023 VerMouth
categories: paper-announcement
thumbnail: assets/img/EMNLP2023/vermouth_logo_no_bg.png
---

📢 Check our latest #EMNLP2023 paper **“Countering Misinformation via Emotional Response Generation”**!

Authors: Daniel Russo, Shane Peter Kaszefski-Yaschuk, Jacopo Staiano, Marco Guerini

https://arxiv.org/abs/2311.10587

{% include figure.liquid loading="eager" path="assets/img/EMNLP2023/vermouth_logo_no_bg.png" class="img-fluid rounded z-depth-1" %}

We introduce VerMouth, the first large-scale and general-domain dataset for the generation of counter-misinformation responses that mimic social media platform style (SMP). The dataset is grounded in trustworthy fact-checking articles and comprises ~12 thousand examples.

{% include figure.liquid loading="eager" path="assets/img/EMNLP2023/vermouth_examples.png" class="img-fluid rounded z-depth-1" %}

## 🥃 VerMouth recipe

### 🛒 Ingredients:

· A misleading claim, a response (the verdict), and a fact-checking article, written in a journalistic style
· An instruction-based LLM
· A dash of human wisdom

### 📋 Instructions:

· Prompt LLM to rewrite the journalistic claim in SMP style
· Ask humans to intervene
· Mix the new claim and the verdict using LLM for a fresh, social response
· Add the human post-editing touch

For a personalized twist, prompt the LLM to infuse Ekman emotions.

{% include figure.liquid loading="eager" path="assets/img/EMNLP2023/data_collection.png" class="img-fluid rounded z-depth-1" %}

We “tasted” VerMouth by casting response generation as a summarisation task, combining extractive and abstractive summarization into a unique pipeline (following our previous work). Both automatic and manual evaluation were used to assess the quality of the responses generated. 

More details in the paper. 

Data are publicly available on GitHub at: https://github.com/marcoguerini/VerMouth