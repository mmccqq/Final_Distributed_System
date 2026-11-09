Professor:
1. 
Hello all,

First, I'm missing Francis's contact so I apologize for not including them. Make sure they get this as well.

I looked into an option for mocking the LLM you'll need to do the different tasks and stumbled upon MockLLM: https://github.com/StacklokLabs/mockllm Open source, allows for deterministic responses since you provide them, and has settings to emulate network lag. This allows you to artifically emulate prompts that take longer as needed. If you are planning on trying to do some real E2E test with a real LLM at some point, I'd highly consider seeing if you can apply for a Claude Premium account through Northeastern to get access to the API. An open source one would do fine, but running it on AWS would probably burn through a lot of your credits.

Also, you'll probably find serverless computing as something to consider in your architecture: recall serverless computing can launch additional infrastructure as needed. So I suggest integrating that in part of your experiments.

Finally, from the feedback in class, make sure to clarify the role of the orchestrator so it is not confused with the load balancer.
s
Lucia Nunez