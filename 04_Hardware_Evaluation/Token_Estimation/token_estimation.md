4.1.) Hardware Token Estimation
This initial LLM system deployment is designed for a mid-sized user base. Not every single user will interact with the LLM, so realistic active usage will only be a portion of the total user population. Most users will be using the LLM primarily for simple conversational tasks, which will not put an immense amount of strain on the GPUs. What must be planned for in an environment is peak concurrent usage. 
This occurs during high-demand scenarios such as classroom environments, competitions, events, or busy work hours, where many users may be submitting requests to the LLM at the same time and using longer or more complex prompts, which places a higher load on GPU resources. Because of this, the system is designed to be able to handle peak concurrency while also operating smoothly during daily usage, ensuring stable performance even under heavy load. 
This is achieved through a variety of methods, including queueing mechanisms, Service Level Objective (SLO) planning, and optimal hardware selection.
The table below shows the estimates that hardware requirements will be based on. It takes into account normal daily usage, expected user interaction levels, and peak demand scenarios such as business usage or events. These estimates are based on scalable assumptions and are meant to act as a baseline model. The system is designed to adapt to increased usage over time, including growth in user adoption and higher demand in the environment it is deployed in.

GPU: NVIDIA L40
Tokens per Second: 200-450/sec
Light Token Load: Small prompts that are simple questions or short text
Heavy Token Load: Long prompts and several paragraphs of context.

Usage Categories:
Normal Daily Use
Moderate Group Use
High Concurrent Use
Requests Rate:
Infrequent
Moderate
Frequent
Estimated Concurrent Users:
Low Concurrency
Moderate Concurrency 
High Concurrency
Token Load Light:
~150-300 tokens
~300–500 tokens 
~400–800 tokens 
Token Load Heavy:
~400–800 tokens 
~800–1,500 tokens 
~1,500–3,000 tokens 
Average Response Time Light:
Fast with minimal delay
Fast with minimal delay
Fast with minimal delay
Average Response Time Heavy:
Longer than light responses but within acceptable ranges
Longer than light responses but within acceptable ranges
Longer than light responses but within acceptable ranges
GPUs Required
1 GPU | Low Concurrency
2 GPU | Medium Concurrency
2 GPU | High Concurrency



Total Cost:
Total GPU’s
Total Token Generation:
Max Load
3 x $8,000-$10,000 = $24,000-$30,000
3 GPUs (2 allocated for inference and 1 used for training, redundancy, or additional inference capacity if needed)
~500–900 tokens/sec baseline (~750–1250 tokens/sec if all GPUs are allocated)
Performance increases as additional GPU resources are allocated, allowing the system to handle greater demand while maintaining responsiveness.

