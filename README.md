# Prompt Engineering Techniques – Ready-to-Use Prompts

This repository contains **ready-to-use AI Studio prompts** for various prompt engineering techniques. Each prompt is crafted according to the specific technique outlined in the [Prompt and Context Engineering Tutorial](https://github.com/panaversity/learn-low-code-agentic-ai/blob/main/00_prompt_engineering/readme.md).

---

## Table of Contents

1. [Prompt Coach](#prompt-coach)
2. [Zero-Shot Prompting](#zero-shot-prompting)
3. [One-Shot Prompting](#one-shot-prompting)
4. [Few-Shot Prompting](#few-shot-prompting)
5. [System Prompting](#system-prompting)
6. [Role Prompting](#role-prompting)
7. [Contextual Prompting](#contextual-prompting)
8. [Chain-of-Thought (CoT) Prompting](#chain-of-thought-cot-prompting)
9. [Self-Consistency](#self-consistency)
10. [Step-Back Prompting](#step-back-prompting)
11. [ReAct (Reasoning + Acting)](#react-reasoning--acting)
12. [Tree of Thoughts (ToT)](#tree-of-thoughts-tot)
13. [MoE-Optimized Prompt Skeleton](#moe-optimized-prompt-skeleton)

---

## Prompt Coach

```
You are my Prompt Coach. I will give you a rough or unclear prompt. 
Your task is to:
1. Clarify it
2. Add missing context
3. Structure it for best results
4. Suggest 2–3 alternative versions (simple, detailed, structured)

Here’s my rough prompt: [INSERT YOUR PROMPT HERE]
```

---

## Zero-Shot Prompting

```
Classify this movie review as positive, negative, or neutral:
"The film was visually stunning but the plot felt rushed."
```

---

## One-Shot Prompting

```
Translate English to French:

English: "Hello, how are you?"
French: "Bonjour, comment allez-vous?"

English: "Where is the library?"
French:
```

---

## Few-Shot Prompting

```
Convert customer feedback to structured data:

Feedback: "Great service, but food was cold"
JSON: {"service": "positive", "food": "negative", "overall": "mixed"}

Feedback: "Amazing experience, will definitely return"
JSON: {"service": "positive", "food": "positive", "overall": "positive"}

Feedback: "Terrible food and rude staff"
JSON:
```

---

## System Prompting

```
You are a helpful travel guide. Provide practical, accurate information about destinations. Always include:
- Key attractions
- Local customs
- Budget considerations
- Best time to visit

User: Tell me about visiting Tokyo.
```

---

## Role Prompting

```
Act as an experienced software architect. I need help designing a scalable web application for 1 million users. What architecture patterns should I consider?
```

---

## Contextual Prompting

```
Context: You're writing for a tech blog aimed at beginners who have never coded before.

Write a 200-word explanation of what an API is, using simple language and practical examples.
```

---

## Chain-of-Thought (CoT) Prompting

```
Solve this step by step:
If I was 6 when my sister was half my age, how old is my sister when I'm 40?

Let me think through this step by step:
```

---

## Self-Consistency

```
Question: If a store offers a 20% discount on a $50 item, what is the final price?

Generate 3 different reasoning paths and select the most consistent answer.

Path 1: ...
Path 2: ...
Path 3: ...

Most common answer:
```

---

## Step-Back Prompting

```
Step 1: What are the key factors affecting website loading speed?

[Get response]

Step 2: Using these factors, provide specific recommendations to optimize loading speed of an e-commerce website with heavy images and multiple third-party plugins.
```

---

## ReAct (Reasoning + Acting)

```
Question: What is the current population of Tokyo, and how does it compare to New York City?

Thought: I need current population data for Tokyo and NYC.
Action: web_search <query="current population Tokyo 2025">
Observation: [result]
Thought: Now I need NYC population
Action: web_search <query="current population New York City 2025">
Observation: [result]

Final Answer: Tokyo ~37.4M, NYC ~23.6M
```

---

## Tree of Thoughts (ToT)

```
Question: What is the best marketing strategy for launching a new eco-friendly clothing brand targeting young adults?

Branch 1: Social Media Campaign
- Pros/Cons
- Score

Branch 2: Sustainable Pop-Up Events
- Pros/Cons
- Score

Branch 3: Collaborative Partnerships
- Pros/Cons
- Score

Synthesize final strategy combining the best approaches.
```

---

## MoE-Optimized Prompt Skeleton

```
You are a Multi-Expert LLM system. You have access to multiple expert agents with distinct specialties (e.g., coding, marketing, finance, legal, education). 

Task: [INSERT USER TASK HERE]

Process:
1. Analyze task type and determine relevant expert agents.
2. Split the task into sub-tasks for each expert if needed.
3. Query each expert for their solution or recommendation.
4. Aggregate answers into a final, coherent response.
5. Include reasoning or citations if applicable.

Constraints:
- Maintain clarity and structure
- Avoid conflicting recommendations
- Provide final answer along with key reasoning steps

User Input: [INSERT INPUT HERE]
```

---

This MoE skeleton allows you to **simulate multi-agent reasoning** in a single prompt, which is great for classroom demonstrations and advanced prompt engineering exercises.

-
