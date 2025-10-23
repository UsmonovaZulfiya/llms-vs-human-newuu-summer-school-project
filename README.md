# Can LLMs replicate human opinion? Evaluating the ability of LLMs to mimic human answer to Real-World Questions
*A Progress Report on the Comparative Study of AI and Human Communication*  

**Team members:**  
Muhammadyusuf Hakimov, Malikaxon Musajonova, Husan Samandarov, Quyashbek Allanazarov, Akniet Kenzhegulov, and Mirzosharif Habibov  

**Academic Mentors:** 
Zulfiya Usmonova, Akmaljon Latifov  

**Date:** August 14, 2025  

---

## Abstract  

In the past 2-3 years, Large Language Models (LLMs) like **ChatGPT, Claude, and Gemini** have become increasingly intelligent by showing high results in different benchmarks, such as *“Humanity’s Last Exam”*[1]. As a result, the question about their ability to replicate human opinions and the relevance of their responses arose in different discussions.  

This research investigates whether LLM agents can simulate genuine human opinions by comparing their responses with those of humans across several open-ended and quite controversial questions.  

- Opinions with profiles (background information) of **100+ people** are collected with an online survey.  
- The same number of agents are created with the same persona profiles and characteristics on **8 different mainstream models**.  
- Through **multi-agent simulation**, agents are given the same open-ended questions from the survey, and their responses are recorded.  
- After all responses are collected, they are then compared with each other (human vs LLM) using **data analysis methods**, and infographics are created for better data visualization.  

By examining models’ responses, this study assesses the reliability of AI as a human opinion generation tool.  

**Keywords:** Large Language Models (LLM), LLM agents, data visualization, multi-agent simulation, human opinion generation  

---

## Introduction  

The aim of this research is to investigate the differences between **LLMs' responses** and **human responses** to certain questions. It will identify the key factors affecting the responses and determine how relevant the responses of generative AI models are.  

LLM agents are the most important tools needed in our simulation as we collect LLM-generated public opinions[2]. **Multi-agent systems (MAS)**, a group of LLM agents, are used in simulations to model scenarios where multiple autonomous entities interact, communicate, and make decisions[3].  

In our simulation, people or groups of different people are represented by agents. In these systems, each agent operates independently within the given environment. They have their own decision-making capabilities, logic, and perception[4].  

### Research Questions  

1. Can LLMs accurately replicate human survey responses when conditioned on persona data?  
2. How similar are LLM-generated responses to real human responses to the same set of questions?  
3. How relevant are AI chatbots’ (ChatGPT, Claude, Gemini) answers compared to humans? Is asking their personal opinions the right thing to do?  

By conducting this research, we aim to compare how well LLM-generated public opinion approximates real human responses on **5 controversial or socially relevant questions**. This research follows an approach combining human survey data collection with **LLM-based agent simulations**.  

---

## Methodology  

### Research Design  
This study employed a **comparative experimental design** to evaluate the accuracy of Large Language Models (LLMs) in simulating human opinions across different contextual conditions[5].  

The research was structured around three distinct experiments designed to assess:  

1. Personalized opinion prediction using a person’s background data.  
2. Cultural context modeling using regional personas.  
3. Baseline performance without contextual information.  

### Participants and Data Collection  
A total of **108 participants from Uzbekistan** were recruited for the study. Participants were selected to represent the local demographic and cultural context relevant to the research objectives (e.g., gender, area of residence, political views, profession)[6].  

All participants provided informed consent and completed a structured questionnaire containing **five opinion statements on socio-cultural topics** (see Appendix A).  

### Opinion Questions  
Five fixed opinion statements were developed covering diverse socio-cultural domains[7]:  

1. **Environmental responsibility** – "Every person should be directly responsible for protecting the environment in their daily life by reducing waste, recycling, and conserving resources."  
2. **Child development** – "Children need to spend more time at home in front of screens for activities such as learning, using technology, and doing homework. They should spend less time in the outdoor environment."  
3. **Social media impact** – "Social media causes more harm than benefit to society due to exposing personal life, spreading false information, and its impact on mental health."  
4. **Gender equality** – "Female athletes should receive equal pay to male athletes when their work, level, and performance in sports are the same."  
5. **Cultural practices** – "A daughter is ready for marriage when she reaches the age of 19."  

Participants responded using a **three-point scale**: *Agree, Disagree, or Neutral*.  

### Experimental Procedure  
The experiment involved evaluating each leading LLM model individually by giving them the same set of challenging and controversial questions as used in the human survey. Each model was asked to provide its response in the form of a vote (Agree, Disagree, or Neutral) along with an explanation of their reasoning.  

These responses were then compared with a dataset of human responses collected through an online survey.  

### LLM Testing Procedure  
For the **8 LLMs**, the following steps were taken[8]:  

- Choosing questions from the given storage of questions.  
- Passing the questions through the API to the correct model and getting the voting of agents and their reasoning.  
- For the collected responses, comparing aggregated agreements with human survey results.  
- Profiling the LLM models.  

### Models Used  
| Model | Params | Provider |
|-------|--------|----------|
| DeepSeek-R1-Distill-Llama | 70B | Groq |
| Gemini-2.5-flash | - | Google |
| Llama-4-scout | 17B | Groq |
| Llama-3.3-versatile | 70B | Groq |
| Gemma-3 | 4B | Ollama |
| GPT-4 | - | OpenAI |
| GPT-3.5-Turbo | - | OpenAI |
| GPT-4.1-mini-2025-04-14 | - | OpenAI |
| Allam-2 | 7B | Groq |  

### Caching and Randomness  
- For **Experiments 2 and 3**, temperature was set to **0** to exclude randomness[9].  
- For **Experiment 1**, temperature was set to **0.3** to allow some creativity in imitating human opinion[9].  
- A new API call was initiated for each agent response.  
- Documentation from model providers was carefully reviewed to ensure no unintended caching occurred.  

### Reproducibility Provisions  
We will share the materials, the report, and source codes (without API keys) in a **GitHub repository** to make reproducibility possible and accurate.  

References
1.Phan, L., & 1,108 others. (2025). Humanity's Last Exam. arXiv preprint arXiv:2501.14249. https://arxiv.org/abs/2501.14249
2.Wang et al. (2024). Large language models empowered agent-based modeling and simulation: a survey and perspectives. Humanities and Social Sciences Communications, 11(1), 1-15. https://doi.org/10.1057/s41599-024-03611-3  Xi et al. (2023). The rise and potential of large language model based agents: a survey. arXiv preprint arXiv:2309.07864.
3.Wikipedia Contributors (2025). Multi-agent system. Wikipedia, The Free Encyclopedia. Retrieved October 23, 2025, from https://en.wikipedia.org/wiki/Multi-agent_system  Guo et al. (2024). Large Language Model based Multi-Agents: A Survey of Progress and Challenges. arXiv preprint arXiv:2402.01680. https://arxiv.org/abs/2402.01680
4.Aher et al. (2023). Using Large Language Models to Simulate Multiple Humans and Replicate Human Subject Studies. arXiv preprint arXiv:2208.10264. https://arxiv.org/abs/2208.10264  Park et al. (2023). Generative Agents: Interactive Simulacra of Human Behavior. arXiv preprint arXiv:2304.03442.
5.Argyle et al. (2023). Out of One, Many: Using Language Models to Simulate Human Samples. Journal of Politics, 85(3), 1234-1248.  Bisbee et al. (2024). Synthetic Replacements for Human Survey Data? The Perils of Large Language Models. Political Analysis, 32(4), 401-416. https://doi.org/10.1017/pan.2024.12
6.Li et al. (2024). Performance and biases of Large Language Models in public opinion simulation. Humanities and Social Sciences Communications, 11(1), 1-12. https://doi.org/10.1057/s41599-024-03609-x  Qu and Wang (2024). Should you use LLMs to simulate opinions? Quality checks for early-stage deliberation. arXiv preprint arXiv:2504.08954.
7.Flamino et al. (2025). Beyond Static Responses: Multi-Agent LLM Systems as a New Paradigm for Social Science Research. arXiv preprint arXiv:2506.01839. (Discusses topics like climate and gender in debates) Cao et al. (2023). Assessing cross-cultural alignment between ChatGPT and human societies: An empirical study. arXiv preprint arXiv:2304.04676.
8.Samuel et al. (2024). PersonaGym: Evaluating Persona Agents and LLMs. arXiv preprint arXiv:2407.18416. https://arxiv.org/abs/2407.18416 Argyle et al. (2023). Out of One, Many: Using Language Models to Simulate Human Samples. Journal of Politics, 85(3), 1234-1248. (Backstory/persona prompting)
9.Aher et al. (2023). Using Large Language Models to Simulate Multiple Humans and Replicate Human Subject Studies. arXiv preprint arXiv:2208.10264. (Discusses randomness control) Salecha et al. (2024). Large language models display human-like social desirability biases in Big Five personality surveys. PNAS Nexus, 3(12), pgae533. https://doi.org/10.1093/pnasnexus/pgae533
---
