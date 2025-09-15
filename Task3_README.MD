\## Python Screening Task 3: Evaluating Open Source Models for Student Competence Analysis



\# Research Plan



My approach to evaluating open source models for high-level student competence analysis would begin with a focused literature review and a survey of relevant open source platforms. I would specifically look for models trained or fine-tuned on code-related tasks, such as code generation, bug fixing, or code summarization. My initial search would focus on model architectures like Transformers and their derivatives (e.g., GPT, BERT), as they have proven effective in capturing the nuances of programming languages. The evaluation criteria would be multi-faceted, starting with the model's ability to ingest and parse Python code accurately, followed by its capacity to identify common errors and logical flaws. To provide a rigorous, data-driven assessment, I would use metrics such as accuracy, precision, and recall on bug detection tasks. I would then assess its ability to generate high-level, conceptual prompts rather than direct solutions.



To validate the model's applicability, I would set up a controlled test environment. This would involve creating a dataset of Python code snippets with known bugs, anti-patterns, and conceptual errors. For each code snippet, I would also create a set of desired "competence analysis prompts" that a human tutor would typically use. I would then run the model against this dataset, comparing its generated prompts and insights to my pre-defined "gold standard" prompts. The final stage would involve a qualitative analysis of the model's output to assess its tone and pedagogical value, ensuring it encourages self-discovery and deeper learning, rather than just providing hints.



\#Reasoning



Q1. What makes a model suitable for high-level competence analysis?

Ans:- A model is suitable for high-level competence analysis if it can move beyond syntax and surface-level errors to understand the underlying logic and intent of the code. This requires a model with strong semantic understanding of the programming language, as well as a pre-trained knowledge of common programming concepts, algorithms, and data structures. It must be able to recognize patterns of thought, identify common misconceptions, and articulate its feedback in a way that guides the student's reasoning without simply handing them the answer. A model that can frame its observations as questions is particularly well-suited for this purpose.



Q2. How would you test whether a model generates meaningful prompts?

Ans:- To test for meaningful prompts, I would employ a combination of automated and human-in-the-loop evaluation. The automated part would involve scoring the prompts against a rubric that measures factors like relevance to the bug, conceptual depth (e.g., does it reference a core programming principle?), and non-solution-giving nature. A "meaningful" prompt would score high on these metrics. The human evaluation would involve a panel of experienced Python tutors or educators. They would be presented with the student's code and the model's generated prompt, and asked to rate the prompt's quality, helpfulness, and its potential to guide the student toward a correct solution on their own.



Q3. What trade-offs might exist between accuracy, interpretability, and cost?

Ans:- There are significant trade-offs to consider. Larger, more accurate models often come with a high computational cost for both training and inference. They can be "black boxes," making it difficult to interpret how they arrived at a specific prompt or conclusion, which is a major limitation for a pedagogical tool. A less accurate but more interpretable model might be preferable, as its reasoning could be explained to the student, adding to the learning experience. The trade-off is between the model’s performance on a given task and the ability to understand and trust its output. This would likely necessitate a hybrid approach, where a smaller, more specialized model is used for the core analysis, and a larger, more general-purpose model is used for generating more creative, higher-level prompts.



Q4. Why did you choose the model you evaluated, and what are its strengths or limitations?

Ans:- For this task, I would choose to evaluate an open-source model from the Code Llama family of large language models. A strength of these models is their specific training on code, which could allow them to analyze larger student codebases and understand the relationships between different parts of a program. Their open-source nature means they are freely available for research and fine-tuning, which is essential for adapting them to a specific pedagogical use case. The main limitation is that they are general-purpose models for code and not specifically trained for pedagogical purposes. This means they may have a tendency to provide direct solutions or code suggestions, which would require careful prompting and fine-tuning to mitigate, ensuring they act as a tutor rather than a solution provider.





\# Reference:

Meta AI. (2023). Code Llama: a large language model for coding. Retrieved from https://ai.meta.com/blog/code-llama-large-language-model-coding/

