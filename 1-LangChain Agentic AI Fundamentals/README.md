# LangChain Agentic AI Fundamentals

This course provides a comprehensive overview of building intelligent agentic applications using LangChain. Participants will learn to create simple LangChain applications and explore structured outputs. The curriculum progresses through multi-step workflows, transitioning from LLM calls to developing agents, and covers essentialagentic design patterns. Key concepts include extending agents with tools, managing functions, and understandingstate management within LangGraph. Students will also implement short-term agent memory techniques and complete a hands-on project: building a report-generating agent.


## Notes
- LangChain is a framework for building applications powered by large language models (LLMs). It simplifies LLM integration, making it easier to develop AI-driven solutions like chatbots, retrieval-augmented generation (RAG) systems, document summarization tools, and autonomous agents.
- LangChain supports multiple programming languages, including Python, JavaScript, and TypeScript.
- Message objects in LangChain:
  - HumanMessage – Represents user input.
  - AIMessage – Represents model responses.
  - SystemMessage – Provides additional instructions.
  - ToolMessage – Used for function calling.
- LangChain uses prompt templates
```python
prompt_template = PromptTemplate(template="What is the capitol of {topic}")
llm.invoke(prompt_template.format(topic="Java"))
```
- When we use FewShotPromptTemplate we can pass examples eg
```python
few_shot_template = FewShotPromptTemplate(
  examples = examples,
  example_promp=example_prompt,
  suffix="Question: {input}",
  input_variables=["input]
)
```
