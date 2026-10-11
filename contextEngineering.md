# Context Engineering

Large language models are powerful, but without access to the right information, they often make mistakes. RAG (Retrieval Augmented Generation) fixes that by grounding model responses in relevant, often private or up-to-date data. As LLMs move into real products and workflows, the ability to build robust, reliable RAG systems is becoming a must-have skill for engineers working in AI.

RAG is at the core of LLM systems that need to be accurate, grounded, and adaptable, whether for internal tools, customer-facing assistants, or specialized applications. This course helps you move beyond proof-of-concept demos into real-world deployment, equipping you with the skills to build, evaluate, and evolve RAG systems as the ecosystem grows.


## RAG (Retrieval Augmented Generation)

### 1. Introduction to RAG
    RAG is the approach that further improves the LLMs by giving them access to information that they dont know from their training.

1. The process of collecting usefull information is called **"Retrieval"** .
2. The process of reasoning over that information and responding is called **"Generation"**

![alt text](images/contextEngineering/image.png)

![alt text](images/contextEngineering/image-1.png)

All LLMs are not know whole things like, private database, the data which is not exposed publically. So how we can do that?

we can give along with the prompt.

![alt text](images/contextEngineering/image-2.png)

RAG Also do the same thing, everytime adding the relevant data in the prompt is difficult, so giving access to the relevant data.

And when user prompt something related to that data:
    step 1: Perform a retrieval step to gather relevant information  - RAG System
    step 2: The LLM would then provide an **"Augmented Prompt"** that includes both the original question and any retrieved information.

    Now the LLM has the information it needs to respond accurately.

![alt text](images/contextEngineering/image-3.png)

The component of the RAG System that handles Retrieval is called **"Retriever"**

![alt text](images/contextEngineering/image-4.png)


