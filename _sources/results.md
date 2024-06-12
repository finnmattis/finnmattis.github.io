# Results

EvidenceBench offers 4 different tasks. Evidence Retrival (ER) tasks ask a model to find a evidence for a hypothesis using the entire paper while Result Evidence Retrival (Result ER) tasks only tasks the model with pulling sentences from the resulsts section. The ER tasks are broken up into the ER @ Optimal task in which the model stops being prompted once it has reached the smallest (optimal) number of sentences needed to support the hypothesis and ER @ 10 which stops prompting the model after 10 sentences. The Result ER tasks are broken up into Result ER @ Optimal and Result ER @ 5 which stops prompting the model after 5 sentences.

These results represent the peak performance of each model for each task, utilizing the prompting strategies of Chain of Thought (CoT), In-Context Learning (ICL), and Section-by-Section.


| Model           | ER @ optimal | ER @ 10 | Result ER @ optimal | Result ER @ 5 |
|-----------------|--------------|---------|---------------------|---------------|
| Max Random      | 100.0        | 99.3    | 100.0               | 99.8          |
| GPT-4o          | 9.6          | 22.3    | 4.4                 | 11.4          |
| Claude-Opus     | 51.4         | 71.6    | 52.6                | 70.8          |
| Gemini-1.5      | 47.6         | 66.4    | 51.7                | 68.7          |
| LLaMA3-70b      | 48.3         | 65.4    | 46.7                | 65.4          |
| OpenAI Emb      | 46.7         | 65.4    | 46.2                | 63.7          |
| VoyageAI        | 25.1         | 42.2    | 19.1                | 33.1          |
| GritLM          | 22.7         | 42.0    | 18.3                | 31.9          |
| E5-Mistral      | 27.0         | 46.4    | 18.9                | 39.1          |
| ER              | 22.7         | 41.9    | 19.3                | 33.6          |