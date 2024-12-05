---
layout: post
title:  "Hands-on-LLM"
date:   2024-12-04
categories: daily log
---

### Hands-on-LLM
  - ch. 7 - Advanced text generation techniques and tools
    - [notebook](https://github.com/HandsOnLLM/Hands-On-Large-Language-Models/tree/main/chapter07)
    - Model I/O - loading quantized models with LangChain
    - Chains - extending the capabilities of LLMs
    - Memory - helping LLMs remember conversations
    - Agents - creating a system of LLMs
        - using tools and planning the actions autonomously
        - [ReAct](https://arxiv.org/abs/2210.03629)
            - combine Reasoning and Acting ie. Reason only (i.e. chain of thought) and Act only(ie. SayCan, WebGPT)
            - Thought, Action, Observation
            - example shown in LangChain to "check the price of macbook pro and convert it to Euro using calculator given the conversion rate from usd"
            - LLM - GPT 3.5 Turbo, DuckDuckGoSearchResults - search tool to find the price of macbook pro, calculator tool using llm-math from LangChain
