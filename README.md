```python
! pip install langchain 
```

    Requirement already satisfied: langchain in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (0.2.14)
    Requirement already satisfied: PyYAML>=5.3 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain) (6.0.1)
    Requirement already satisfied: SQLAlchemy<3,>=1.4 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain) (2.0.31)
    Requirement already satisfied: aiohttp<4.0.0,>=3.8.3 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain) (3.9.5)
    Requirement already satisfied: async-timeout<5.0.0,>=4.0.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain) (4.0.3)
    Requirement already satisfied: langchain-core<0.3.0,>=0.2.32 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain) (0.2.34)
    Requirement already satisfied: langchain-text-splitters<0.3.0,>=0.2.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain) (0.2.2)
    Requirement already satisfied: langsmith<0.2.0,>=0.1.17 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain) (0.1.104)
    Requirement already satisfied: numpy<2,>=1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain) (1.22.4)
    Requirement already satisfied: pydantic<3,>=1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain) (2.8.2)
    Requirement already satisfied: requests<3,>=2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain) (2.32.3)
    Requirement already satisfied: tenacity!=8.4.0,<9.0.0,>=8.1.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain) (8.5.0)
    Requirement already satisfied: aiosignal>=1.1.2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from aiohttp<4.0.0,>=3.8.3->langchain) (1.3.1)
    Requirement already satisfied: attrs>=17.3.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from aiohttp<4.0.0,>=3.8.3->langchain) (23.2.0)
    Requirement already satisfied: frozenlist>=1.1.1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from aiohttp<4.0.0,>=3.8.3->langchain) (1.4.1)
    Requirement already satisfied: multidict<7.0,>=4.5 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from aiohttp<4.0.0,>=3.8.3->langchain) (6.0.5)
    Requirement already satisfied: yarl<2.0,>=1.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from aiohttp<4.0.0,>=3.8.3->langchain) (1.9.4)
    Requirement already satisfied: jsonpatch<2.0,>=1.33 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core<0.3.0,>=0.2.32->langchain) (1.33)
    Requirement already satisfied: packaging<25,>=23.2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core<0.3.0,>=0.2.32->langchain) (24.1)
    Requirement already satisfied: typing-extensions>=4.7 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core<0.3.0,>=0.2.32->langchain) (4.12.2)
    Requirement already satisfied: httpx<1,>=0.23.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langsmith<0.2.0,>=0.1.17->langchain) (0.27.0)
    Requirement already satisfied: orjson<4.0.0,>=3.9.14 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langsmith<0.2.0,>=0.1.17->langchain) (3.10.7)
    Requirement already satisfied: annotated-types>=0.4.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from pydantic<3,>=1->langchain) (0.7.0)
    Requirement already satisfied: pydantic-core==2.20.1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from pydantic<3,>=1->langchain) (2.20.1)
    Requirement already satisfied: charset-normalizer<4,>=2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from requests<3,>=2->langchain) (3.3.2)
    Requirement already satisfied: idna<4,>=2.5 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from requests<3,>=2->langchain) (3.7)
    Requirement already satisfied: urllib3<3,>=1.21.1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from requests<3,>=2->langchain) (2.2.2)
    Requirement already satisfied: certifi>=2017.4.17 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from requests<3,>=2->langchain) (2024.7.4)
    Requirement already satisfied: greenlet!=0.4.17 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from SQLAlchemy<3,>=1.4->langchain) (3.0.3)
    Requirement already satisfied: anyio in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.17->langchain) (4.4.0)
    Requirement already satisfied: httpcore==1.* in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.17->langchain) (1.0.5)
    Requirement already satisfied: sniffio in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.17->langchain) (1.3.1)
    Requirement already satisfied: h11<0.15,>=0.13 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpcore==1.*->httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.17->langchain) (0.14.0)
    Requirement already satisfied: jsonpointer>=1.9 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from jsonpatch<2.0,>=1.33->langchain-core<0.3.0,>=0.2.32->langchain) (3.0.0)
    Requirement already satisfied: exceptiongroup>=1.0.2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from anyio->httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.17->langchain) (1.2.2)
    


```python
! pip install langchain-core 
```

    Requirement already satisfied: langchain-core in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (0.2.34)
    Requirement already satisfied: PyYAML>=5.3 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core) (6.0.1)
    Requirement already satisfied: jsonpatch<2.0,>=1.33 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core) (1.33)
    Requirement already satisfied: langsmith<0.2.0,>=0.1.75 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core) (0.1.104)
    Requirement already satisfied: packaging<25,>=23.2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core) (24.1)
    Requirement already satisfied: pydantic<3,>=1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core) (2.8.2)
    Requirement already satisfied: tenacity!=8.4.0,<9.0.0,>=8.1.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core) (8.5.0)
    Requirement already satisfied: typing-extensions>=4.7 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core) (4.12.2)
    Requirement already satisfied: jsonpointer>=1.9 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from jsonpatch<2.0,>=1.33->langchain-core) (3.0.0)
    Requirement already satisfied: httpx<1,>=0.23.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langsmith<0.2.0,>=0.1.75->langchain-core) (0.27.0)
    Requirement already satisfied: orjson<4.0.0,>=3.9.14 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langsmith<0.2.0,>=0.1.75->langchain-core) (3.10.7)
    Requirement already satisfied: requests<3,>=2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langsmith<0.2.0,>=0.1.75->langchain-core) (2.32.3)
    Requirement already satisfied: annotated-types>=0.4.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from pydantic<3,>=1->langchain-core) (0.7.0)
    Requirement already satisfied: pydantic-core==2.20.1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from pydantic<3,>=1->langchain-core) (2.20.1)
    Requirement already satisfied: anyio in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.75->langchain-core) (4.4.0)
    Requirement already satisfied: certifi in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.75->langchain-core) (2024.7.4)
    Requirement already satisfied: httpcore==1.* in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.75->langchain-core) (1.0.5)
    Requirement already satisfied: idna in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.75->langchain-core) (3.7)
    Requirement already satisfied: sniffio in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.75->langchain-core) (1.3.1)
    Requirement already satisfied: h11<0.15,>=0.13 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpcore==1.*->httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.75->langchain-core) (0.14.0)
    Requirement already satisfied: charset-normalizer<4,>=2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from requests<3,>=2->langsmith<0.2.0,>=0.1.75->langchain-core) (3.3.2)
    Requirement already satisfied: urllib3<3,>=1.21.1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from requests<3,>=2->langsmith<0.2.0,>=0.1.75->langchain-core) (2.2.2)
    Requirement already satisfied: exceptiongroup>=1.0.2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from anyio->httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.75->langchain-core) (1.2.2)
    


```python
! pip install langchain_community 
```

    Requirement already satisfied: langchain_community in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (0.2.12)
    Requirement already satisfied: PyYAML>=5.3 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain_community) (6.0.1)
    Requirement already satisfied: SQLAlchemy<3,>=1.4 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain_community) (2.0.31)
    Requirement already satisfied: aiohttp<4.0.0,>=3.8.3 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain_community) (3.9.5)
    Requirement already satisfied: dataclasses-json<0.7,>=0.5.7 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain_community) (0.6.7)
    Requirement already satisfied: langchain<0.3.0,>=0.2.13 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain_community) (0.2.14)
    Requirement already satisfied: langchain-core<0.3.0,>=0.2.30 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain_community) (0.2.34)
    Requirement already satisfied: langsmith<0.2.0,>=0.1.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain_community) (0.1.104)
    Requirement already satisfied: numpy<2,>=1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain_community) (1.22.4)
    Requirement already satisfied: requests<3,>=2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain_community) (2.32.3)
    Requirement already satisfied: tenacity!=8.4.0,<9.0.0,>=8.1.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain_community) (8.5.0)
    Requirement already satisfied: aiosignal>=1.1.2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from aiohttp<4.0.0,>=3.8.3->langchain_community) (1.3.1)
    Requirement already satisfied: attrs>=17.3.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from aiohttp<4.0.0,>=3.8.3->langchain_community) (23.2.0)
    Requirement already satisfied: frozenlist>=1.1.1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from aiohttp<4.0.0,>=3.8.3->langchain_community) (1.4.1)
    Requirement already satisfied: multidict<7.0,>=4.5 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from aiohttp<4.0.0,>=3.8.3->langchain_community) (6.0.5)
    Requirement already satisfied: yarl<2.0,>=1.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from aiohttp<4.0.0,>=3.8.3->langchain_community) (1.9.4)
    Requirement already satisfied: async-timeout<5.0,>=4.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from aiohttp<4.0.0,>=3.8.3->langchain_community) (4.0.3)
    Requirement already satisfied: marshmallow<4.0.0,>=3.18.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from dataclasses-json<0.7,>=0.5.7->langchain_community) (3.22.0)
    Requirement already satisfied: typing-inspect<1,>=0.4.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from dataclasses-json<0.7,>=0.5.7->langchain_community) (0.9.0)
    Requirement already satisfied: langchain-text-splitters<0.3.0,>=0.2.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain<0.3.0,>=0.2.13->langchain_community) (0.2.2)
    Requirement already satisfied: pydantic<3,>=1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain<0.3.0,>=0.2.13->langchain_community) (2.8.2)
    Requirement already satisfied: jsonpatch<2.0,>=1.33 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core<0.3.0,>=0.2.30->langchain_community) (1.33)
    Requirement already satisfied: packaging<25,>=23.2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core<0.3.0,>=0.2.30->langchain_community) (24.1)
    Requirement already satisfied: typing-extensions>=4.7 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langchain-core<0.3.0,>=0.2.30->langchain_community) (4.12.2)
    Requirement already satisfied: httpx<1,>=0.23.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langsmith<0.2.0,>=0.1.0->langchain_community) (0.27.0)
    Requirement already satisfied: orjson<4.0.0,>=3.9.14 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from langsmith<0.2.0,>=0.1.0->langchain_community) (3.10.7)
    Requirement already satisfied: charset-normalizer<4,>=2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from requests<3,>=2->langchain_community) (3.3.2)
    Requirement already satisfied: idna<4,>=2.5 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from requests<3,>=2->langchain_community) (3.7)
    Requirement already satisfied: urllib3<3,>=1.21.1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from requests<3,>=2->langchain_community) (2.2.2)
    Requirement already satisfied: certifi>=2017.4.17 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from requests<3,>=2->langchain_community) (2024.7.4)
    Requirement already satisfied: greenlet!=0.4.17 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from SQLAlchemy<3,>=1.4->langchain_community) (3.0.3)
    Requirement already satisfied: anyio in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.0->langchain_community) (4.4.0)
    Requirement already satisfied: httpcore==1.* in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.0->langchain_community) (1.0.5)
    Requirement already satisfied: sniffio in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.0->langchain_community) (1.3.1)
    Requirement already satisfied: h11<0.15,>=0.13 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from httpcore==1.*->httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.0->langchain_community) (0.14.0)
    Requirement already satisfied: jsonpointer>=1.9 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from jsonpatch<2.0,>=1.33->langchain-core<0.3.0,>=0.2.30->langchain_community) (3.0.0)
    Requirement already satisfied: annotated-types>=0.4.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from pydantic<3,>=1->langchain<0.3.0,>=0.2.13->langchain_community) (0.7.0)
    Requirement already satisfied: pydantic-core==2.20.1 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from pydantic<3,>=1->langchain<0.3.0,>=0.2.13->langchain_community) (2.20.1)
    Requirement already satisfied: mypy-extensions>=0.3.0 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from typing-inspect<1,>=0.4.0->dataclasses-json<0.7,>=0.5.7->langchain_community) (1.0.0)
    Requirement already satisfied: exceptiongroup>=1.0.2 in /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages (from anyio->httpx<1,>=0.23.0->langsmith<0.2.0,>=0.1.0->langchain_community) (1.2.2)
    

# Interaction with Bedrock APIs through LangChain

I would like to talk about two classes here:

![image-3.png](LangChain_files/image-3.png)

# Initializing the LangChain BedrockChat object

We use <b>BedrockChat</b> wrapper in working with InvokeModel API of the Bedrock. 


```python
from langchain_community.chat_models import BedrockChat
```


```python
import boto3
```


```python
def initialize_llm():
    """
    Initialize a Large Language Model (LLM) instance using the Bedrock Runtime service.

    Returns:
        BedrockChat: An instance of the BedrockChat class, which represents the initialized LLM.

    """
    model_id = "anthropic.claude-3-sonnet-20240229-v1:0"  # In this notebook most of the times we use this model
    model_kwargs = {
        "max_tokens": 2048,
        "temperature": 0.0,
        "top_k": 250,
        "top_p": 1,
        "stop_sequences": ["\n\nHuman"],
    }

    # Check if AWS_REGION environment variable is set
    aws_region =  "us-west-2"

    bedrock_runtime = boto3.client(
        service_name="bedrock-runtime",
        region_name=aws_region,
    )

    bedrock_llm = BedrockChat(  #here we use the BedrockChat 
        client=bedrock_runtime,
        model_id=model_id,
        model_kwargs=model_kwargs,
    )

    return bedrock_llm
   
bedrock_llm = initialize_llm()
```

    /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages/langchain_core/_api/deprecation.py:141: LangChainDeprecationWarning: The class `BedrockChat` was deprecated in LangChain 0.0.34 and will be removed in 0.3. An updated version of the class exists in the langchain-aws package and should be used instead. To use it run `pip install -U langchain-aws` and import as `from langchain_aws import ChatBedrock`.
      warn_deprecated(
    

## Simple Call with the BedrockChat wrapper

We use Bedrock's <b>.invoke()</b> in this section. This method undestands the chat, meaning different types of messages: system message, human message and AI generated massage. 

If you just want to call LLM like this example, there is no value to use LangChain as we can simply call Bedrock APIs without using LangChain. 

The real value of LangChain is where we need more complex integration and orchestration. I use this simple example to start with a LangChain and show its abstration layer on tip of Bedrock APIs:

![image.png](LangChain_files/image.png)


```python
messages = [
    (
        "system", "You are a helpful AI student that would like to learn about AI topics. Respond in a frienly way.",
    ),
    
    ("human", "I want to know what is top_p in LLM configuration?"),
]
first_res = bedrock_llm.invoke(messages)
first_res
```




    AIMessage(content="Sure, I'd be happy to explain what top_p is in the context of large language models (LLMs) configuration!\n\nTop_p, also known as nucleus sampling or top-k sampling, is a technique used during the text generation process in LLMs. It is a way to control the randomness and diversity of the generated text by limiting the number of tokens (words or subwords) that the model considers at each step of the generation process.\n\nHere's how it works:\n\n1. At each step of text generation, the LLM calculates the probability distribution over the entire vocabulary for the next token.\n2. Instead of simply selecting the token with the highest probability, top_p sampling selects from the smallest possible set of tokens whose cumulative probability exceeds a specified threshold value (p).\n3. The value of p is typically set between 0.9 and 1.0. A higher value of p means that the model will consider a larger set of tokens, leading to more diverse and potentially more surprising outputs. A lower value of p will make the generated text more focused and predictable.\n\nThe main advantage of using top_p sampling is that it allows the model to explore a wider range of possibilities while still maintaining some level of coherence and relevance. It helps to mitigate the issue of repetitive or generic outputs that can sometimes occur when using greedy decoding (always selecting the token with the highest probability).\n\nTop_p sampling is often used in combination with other techniques, such as temperature scaling, which adjusts the overall randomness of the generated text.\n\nIn summary, top_p is a configuration parameter in LLMs that controls the diversity and randomness of the generated text by limiting the set of tokens considered at each step of the generation process based on their cumulative probability.", response_metadata={'model_id': 'anthropic.claude-3-sonnet-20240229-v1:0', 'usage': {'prompt_tokens': 45, 'completion_tokens': 385, 'total_tokens': 430}}, id='run-d3166c46-3a2c-480a-867b-2589468d022f-0')




```python
print(first_res.content)
```

    Sure, I'd be happy to explain what top_p is in the context of large language models (LLMs) configuration!
    
    Top_p, also known as nucleus sampling or top-k sampling, is a technique used during the text generation process in LLMs. It is a way to control the randomness and diversity of the generated text by limiting the number of tokens (words or subwords) that the model considers at each step of the generation process.
    
    Here's how it works:
    
    1. At each step of text generation, the LLM calculates the probability distribution over the entire vocabulary for the next token.
    2. Instead of simply selecting the token with the highest probability, top_p sampling selects from the smallest possible set of tokens whose cumulative probability exceeds a specified threshold value (p).
    3. The value of p is typically set between 0.9 and 1.0. A higher value of p means that the model will consider a larger set of tokens, leading to more diverse and potentially more surprising outputs. A lower value of p will make the generated text more focused and predictable.
    
    The main advantage of using top_p sampling is that it allows the model to explore a wider range of possibilities while still maintaining some level of coherence and relevance. It helps to mitigate the issue of repetitive or generic outputs that can sometimes occur when using greedy decoding (always selecting the token with the highest probability).
    
    Top_p sampling is often used in combination with other techniques, such as temperature scaling, which adjusts the overall randomness of the generated text.
    
    In summary, top_p is a configuration parameter in LLMs that controls the diversity and randomness of the generated text by limiting the set of tokens considered at each step of the generation process based on their cumulative probability.
    


```python
#If you want to know how many tokens are used in the previous conversation:
print(first_res.response_metadata['usage'])
```

    {'prompt_tokens': 45, 'completion_tokens': 385, 'total_tokens': 430}
    

#### Suggestion:#### it would be nice to show what we need to change in the above code if we use a different model

I have ansered the above question by using Titan Express. All I needed to do was to make usre I am using the right model and initialize it (this time I called it titan_initialze_llm)


```python
titan_model_id = "amazon.titan-text-express-v1"
def titan_initialize_llm():
    """
    Initialize a Large Language Model (LLM) instance using the Bedrock Runtime service.

    Returns:
        BedrockChat: An instance of the BedrockChat class, which represents the initialized LLM.

    """
    model_id = titan_model_id
 

    # Check if AWS_REGION environment variable is set
    aws_region =  "us-west-2"

    bedrock_runtime = boto3.client(
        service_name="bedrock-runtime",
        region_name=aws_region,
    )

    bedrock_llm = BedrockChat(
        client=bedrock_runtime,
        model_id=model_id,
        #model_kwargs=model_kwargs,
    )

    return bedrock_llm
   
titan_bedrock_llm = titan_initialize_llm()
```


```python
first_res = titan_bedrock_llm.invoke(messages)
first_res
```




    AIMessage(content=' Hello! Top_p stands for top p sampling. It is a technique used in natural language processing to control the diversity of the generated text. In the context of large language models (LLMs), top_p sampling is used to determine which tokens to include in the generated text. The algorithm selects tokens based on their probability distribution, and the top_p value determines the percentage of tokens to include. For example, if top_p is set to 0.9, the algorithm will select the top 90% of tokens from the probability distribution to include in the generated text. This can help control the diversity of the', response_metadata={'model_id': 'amazon.titan-text-express-v1', 'usage': {'prompt_tokens': 43, 'completion_tokens': 128, 'total_tokens': 171}}, id='run-08d92c05-b257-4ec6-9aaf-c91d0180657d-0')



## LLM (.predict() ) vs Chat (.invoke() ) 

The <b>.predict()</b> method is an LLM method that has been deprecated. Still it's working but in next versions it may not work.

Please see the following link:


https://python.langchain.com/v0.2/api_reference/aws/llms/langchain_aws.llms.bedrock.BedrockLLM.html#langchain_aws.llms.bedrock.BedrockLLM.predict_messages

![image-2.png](LangChain_files/image-2.png)



The interaction looks like this:
![image-3.png](LangChain_files/image-3.png)

I start with one message only interaction before showing the interactions that looks like a chat. Here is one question by using .predict():


```python
city = bedrock_llm.predict("I want to go hiking. Which city in California should I go to?")
print(city)
```

    /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages/langchain_core/_api/deprecation.py:141: LangChainDeprecationWarning: The method `BaseChatModel.predict` was deprecated in langchain-core 0.1.7 and will be removed in 1.0. Use invoke instead.
      warn_deprecated(
    

    Here are some great cities in California that offer excellent hiking opportunities nearby:
    
    1. San Francisco - You can hike in Muir Woods National Monument, the Marin Headlands, or Mount Tamalpais State Park, all located just north of the city.
    
    2. Los Angeles - Griffith Park has over 50 miles of hiking trails right in the city. You can also head to the Santa Monica Mountains for hikes like the Solstice Canyon Trail.
    
    3. San Diego - Torrey Pines State Natural Reserve has beautiful coastal hiking trails. Mission Trails Regional Park is another huge urban park with many trails.
    
    4. Sacramento - Hiking is available in parks like the American River Parkway and Folsom Lake Recreation Area on the outskirts of the city.
    
    5. Santa Barbara - The Santa Ynez Mountains provide great hiking, including trails in Los Padres National Forest like Inspiration Point.
    
    6. Lake Tahoe (cities like South Lake Tahoe) - The entire Lake Tahoe area has phenomenal hiking in the Sierra Nevada mountains.
    
    Consider factors like the type of hiking you want (beach, forest, mountains), distance you're willing to drive from the city, and time of year when choosing a California hiking destination.
    

And here is asking the same one question by using .invoke(). Both work with no problem:


```python
city = bedrock_llm.invoke("I want to go hiking. Which city in California should I go to?")
print(city.content)
```

    Here are some great cities in California that offer excellent hiking opportunities nearby:
    
    1. San Francisco - You can hike in Muir Woods National Monument, the Marin Headlands, or Mount Tamalpais State Park, all located just north of the city.
    
    2. Los Angeles - Griffith Park has over 50 miles of hiking trails right in the city. You can also head to the Santa Monica Mountains for hikes like the Solstice Canyon Trail.
    
    3. San Diego - Torrey Pines State Natural Reserve has beautiful coastal hiking trails. Mission Trails Regional Park is another huge urban park with many trails.
    
    4. Sacramento - Folsom Lake State Recreation Area and the American River Parkway trail system provide great hiking very close to downtown.
    
    5. Santa Barbara - Hike in the Santa Ynez Mountains, including trails in Los Padres National Forest like Inspiration Point.
    
    6. Oakland/Berkeley - Redwood Regional Park and Tilden Regional Park in the Oakland Hills have wonderful redwood forest hikes.
    
    Some other top hiking destinations are Yosemite, Sequoia/Kings Canyon, and Joshua Tree National Parks if you want to explore more remote wilderness areas. The options are endless in California!
    

But becuase we did not use chat message formatting it does not have a context of previous conversation and if you ask a question that is related to earlier answer it fails:


```python
other_activities = bedrock_llm.invoke("What else can I do in those cities you mentioned?")
other_activities
```




    AIMessage(content="Unfortunately, I did not actually mention any specific cities in our conversation so far. I don't have enough context to recommend activities in particular cities. Could you provide the names of the cities you're interested in, and I'd be happy to suggest some things to do and see there based on what those destinations offer?", response_metadata={'model_id': 'anthropic.claude-3-sonnet-20240229-v1:0', 'usage': {'prompt_tokens': 18, 'completion_tokens': 65, 'total_tokens': 83}}, id='run-0f5a6771-53ec-4e33-a818-f93cee04dfa9-0')




```python
other_activities.content
```




    "Unfortunately, I did not actually mention any specific cities in our conversation so far. I don't have enough context to recommend activities in particular cities. Could you provide the names of the cities you're interested in, and I'd be happy to suggest some things to do and see there based on what those destinations offer?"



OK now that you saw how important is to provide right messaging format, let's define a message format with correct roles and try the .invoke() and .predict() again. The following cell defines a right messaging format and it use .invoke():


```python
messages = [
    (
        "system", "You are a helpful AI student that would like to learn about AI topics. Respond only in one sentence.",
    ),
    
    ("human", "I want to know what is top_p in LLM configuration?"),
]
first_res = bedrock_llm.invoke(messages)
first_res.content
```




    'Top_p is a sampling technique used in language models to control the randomness of generated text by considering only the most probable tokens at each step.'



To text if .invoke() understands the context, now we assemble the previous response into the next message and ask a new question:


```python
messages = [
    (
        "system", "You are a helpful AI student that would like to learn about AI topics. Respond only in one sentence.",
    ),
    
    ("human", "I want to know what is top_p in LLM configuration?"),
     ("ai", "Top_p is a sampling technique used in language models to control the randomness of generated text by considering only the most probable tokens at each step."),
    ("human", "Why is that useful?"),
]
first_res = bedrock_llm.invoke(messages)
first_res.content
```




    'Top_p sampling helps prevent the model from generating unlikely or nonsensical text by focusing on the most probable tokens.'



As you saw above, if we include previous context in communication with .invoke() API, it works with no problem. But will that work with .predict() too? Here is the result: 


```python
messages = [
    (
        "system", "You are a helpful AI student that would like to learn about AI topics. Respond only in one sentence.",
    ),
    
    ("human", "I want to know what is top_p in LLM configuration?"),
     ("ai", "Top_p is a sampling technique used in language models to control the randomness of generated text by considering only the most probable tokens at each step."),
    ("human", "Why is that useful?"),
]
first_res = bedrock_llm.predict(messages)
first_res.content
```


    ---------------------------------------------------------------------------

    ValidationError                           Traceback (most recent call last)

    Cell In[18], line 10
          1 messages = [
          2     (
          3         "system", "You are a helpful AI student that would like to learn about AI topics. Respond only in one sentence.",
       (...)
          8     ("human", "Why is that useful?"),
          9 ]
    ---> 10 first_res = bedrock_llm.predict(messages)
         11 first_res.content
    

    File ~/anaconda3/envs/python3/lib/python3.10/site-packages/langchain_core/_api/deprecation.py:170, in deprecated.<locals>.deprecate.<locals>.warning_emitting_wrapper(*args, **kwargs)
        168     warned = True
        169     emit_warning()
    --> 170 return wrapped(*args, **kwargs)
    

    File ~/anaconda3/envs/python3/lib/python3.10/site-packages/langchain_core/language_models/chat_models.py:1053, in BaseChatModel.predict(self, text, stop, **kwargs)
       1051 else:
       1052     _stop = list(stop)
    -> 1053 result = self([HumanMessage(content=text)], stop=_stop, **kwargs)
       1054 if isinstance(result.content, str):
       1055     return result.content
    

    File ~/anaconda3/envs/python3/lib/python3.10/site-packages/langchain_core/messages/human.py:56, in HumanMessage.__init__(self, content, **kwargs)
         47 def __init__(
         48     self, content: Union[str, List[Union[str, Dict]]], **kwargs: Any
         49 ) -> None:
         50     """Pass in content as positional arg.
         51 
         52     Args:
         53         content: The string contents of the message.
         54         kwargs: Additional fields to pass to the message.
         55     """
    ---> 56     super().__init__(content=content, **kwargs)
    

    File ~/anaconda3/envs/python3/lib/python3.10/site-packages/langchain_core/messages/base.py:66, in BaseMessage.__init__(self, content, **kwargs)
         57 def __init__(
         58     self, content: Union[str, List[Union[str, Dict]]], **kwargs: Any
         59 ) -> None:
         60     """Pass in content as positional arg.
         61 
         62     Args:
         63         content: The string contents of the message.
         64         kwargs: Additional fields to pass to the
         65     """
    ---> 66     super().__init__(content=content, **kwargs)
    

    File ~/anaconda3/envs/python3/lib/python3.10/site-packages/langchain_core/load/serializable.py:113, in Serializable.__init__(self, *args, **kwargs)
        111 def __init__(self, *args: Any, **kwargs: Any) -> None:
        112     """"""
    --> 113     super().__init__(*args, **kwargs)
    

    File ~/anaconda3/envs/python3/lib/python3.10/site-packages/pydantic/v1/main.py:341, in BaseModel.__init__(__pydantic_self__, **data)
        339 values, fields_set, validation_error = validate_model(__pydantic_self__.__class__, data)
        340 if validation_error:
    --> 341     raise validation_error
        342 try:
        343     object_setattr(__pydantic_self__, '__dict__', values)
    

    ValidationError: 9 validation errors for HumanMessage
    content
      str type expected (type=type_error.str)
    content -> 0
      str type expected (type=type_error.str)
    content -> 0
      value is not a valid dict (type=type_error.dict)
    content -> 1
      str type expected (type=type_error.str)
    content -> 1
      value is not a valid dict (type=type_error.dict)
    content -> 2
      str type expected (type=type_error.str)
    content -> 2
      value is not a valid dict (type=type_error.dict)
    content -> 3
      str type expected (type=type_error.str)
    content -> 3
      value is not a valid dict (type=type_error.dict)


# Working with Converse Bedrock API

The <b>ChatBedrockConverse</b> wrapper works with Bedrock Converse API.

AWS has recently released the Bedrock Converse API which provides a unified conversational interface for Bedrock models. 

![image.png](LangChain_files/image.png)


```python
! pip install -qU langchain-aws

```


```python
from langchain_aws import ChatBedrockConverse
```


```python
def converse_initialize_llm():
    """
    Initialize a Large Language Model (LLM) instance using the Bedrock Runtime service.

    Returns:
        BedrockChat: An instance of the ChatBedrockConverse class, which represents the initialized LLM.

    """
    model = "anthropic.claude-3-sonnet-20240229-v1:0"
    model_kwargs = {
        "max_tokens": 2048,
        "temperature": 0.0,
        "top_k": 250,
        "top_p": 1,
        "stop_sequences": ["\n\nHuman"],
    }

    # Check if AWS_REGION environment variable is set
    aws_region =  "us-west-2"

    bedrock_runtime = boto3.client(
        service_name="bedrock-runtime",
        region_name=aws_region,
    )

    bedrock_llm = ChatBedrockConverse( # here I use ChatBedrockConverse 
        client=bedrock_runtime,
        model=model,
        #model_kwargs=model_kwargs,
    )

    return bedrock_llm
   
bedrock_llm_converse = converse_initialize_llm()
```


```python
messages = [
    (
        "system", "You are a helpful AI student that would like to learn about AI topics. Respond only in one sentence.",
    ),
    
    ("human", "I want to know what is top_p in LLM configuration?"),
     ("ai", "Top_p is a sampling technique used in language models to control the randomness of generated text by considering only the most probable tokens at each step."),
    ("human", "Why is that useful?"),
]
first_res = bedrock_llm_converse.invoke(messages)
first_res.content
```




    'Top_p sampling helps prevent the model from generating unlikely or nonsensical outputs while still allowing for some diversity in the generated text.'



# Prompt Template

Imagine you have a prompt that some parts of that prompt is different in each user call. For example, if users want to know more about different parameters in Becrock model, rather than typing most parts of the following prompt every time, they can just mention the parts that are different than the other ones, like those parameters in the {} in the following paragraph:

#### <i>Write one educational paragraph about {parameter} in Bedrock {modelname} model. </i>



That means, users do not give the prompt itself to LLM rather they give the required "inputs" to a <b> prompt template<b>  and then by a simple string interpolation, the prompt is generated before sending that to LLM. Where that prompt is generated? Inside the LangChain by using PromptTemplate.

Usually a UI collects the inputs from the user, although a user can send those inputs through direct API call inside a code as well. The flow is shown in the following figure:

![image-2.png](LangChain_files/image-2.png)

To allow users to NOT to input all the prompt text in each call, we need to use a prompt template and let LangChain to replace the placeholders with string text. LangChain connverts the <b>prompt template</b> to a <b>prompt</b> before sending that to LLM. 

In addition to gathering inputs from user, we can also enrich the generated prompt by adding personas or system messages before sedning the final prompt to LLM.

#### Using PromptTemplate:
To use prompt templates in Langchain we need to use PromptTemplate. It needs two inputs: the input variable names and the template itself. Later, to interpolate the variable names with values we use .format() method:

![image.png](LangChain_files/image.png)

Let's see them in practice:


```python
from langchain import PromptTemplate

educational_message_template = PromptTemplate(
    input_variables =['parameter', 'modelname'],
    template = "Write one educational paragraph about {parameter} in Bedrock {modelname} model."
)
final_prompt = educational_message_template .format(parameter="top_p" , modelname= 'claude')
print(final_prompt)
```

    Write one educational paragraph about top_p in Bedrock claude model.
    

Now we use the same methods we learned before to send this prompt to the model:


```python
res = bedrock_llm.invoke(final_prompt)
res
```




    AIMessage(content="In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity.", response_metadata={'model_id': 'anthropic.claude-3-sonnet-20240229-v1:0', 'usage': {'prompt_tokens': 22, 'completion_tokens': 171, 'total_tokens': 193}}, id='run-5a5fc2db-71a2-4a9b-ac93-a8e16cd60d79-0')



to get a more clean result:


```python
res = bedrock_llm.invoke(final_prompt).content
res
```




    "In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity."



#### Using ChatPromptTemplate:

Using PromptTemplate is sufficient if we want to have isolated conversations with AI. But if we want AI to answer a question based on previous messages (historical context), we need to include the previous messages while asking new question. This is where ChatPromptTemplate comes into the picture.

#### NOTE: #### 
please consider that we already discussed the idea of using right message formatting but over there we did not do any string interpolation in different types of messages. This time when we assemble the template we have placeholders too:


```python
from langchain_core.prompts import ChatPromptTemplate

chat_template = ChatPromptTemplate.from_messages(
    [
        ("system", "You are a helpful AI expert that answers a student query"),
        ("human", "what top_p in Bedrock claude model is all about?"),
        ("ai", "In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity."),
        ("human", "{user_query}"),
    ]
)

messages = chat_template.format_messages(user_query="is it related to top_k?")
messages
```




    [SystemMessage(content='You are a helpful AI expert that answers a student query'),
     HumanMessage(content='what top_p in Bedrock claude model is all about?'),
     AIMessage(content="In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity."),
     HumanMessage(content='is it related to top_k?')]




```python
messages[0]
```




    SystemMessage(content='You are a helpful AI expert that answers a student query')




```python
messages[1]
```




    HumanMessage(content='what top_p in Bedrock claude model is all about?')




```python
messages[2]
```




    AIMessage(content="In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity.")




```python
messages[3]
```




    HumanMessage(content='is it related to top_k?')



Another way to write the above chat mesages is through Human, System and AI message templates. There is no difference in the generated output by LLM, that is just to separate them into different templates:


```python
from langchain_core.prompts import HumanMessagePromptTemplate, SystemMessagePromptTemplate, AIMessagePromptTemplate

chat_template = ChatPromptTemplate.from_messages(
    [
        SystemMessagePromptTemplate.from_template("You are a helpful AI expert that answers a student query"),
        HumanMessagePromptTemplate.from_template("{query}"),
    ]
)
messages = chat_template.format_messages(query="what top_p in Bedrock claude model is all about?")
messages
```




    [SystemMessage(content='You are a helpful AI expert that answers a student query'),
     HumanMessage(content='what top_p in Bedrock claude model is all about?')]



#### Using few shot and prompt templates

In few shot technique we provide examples. Those could be a long piece of text. When the we need to pass a long text into a prompt in few shot technique, it's better we create a variable for the entire prompt text and send it as a whole to the PromptTemplate: 

![image-2.png](LangChain_files/image-2.png)


```python
template = """You are a helpful AI instrcutor.

Human: {human_ask}
Assistant:"""

prompt = PromptTemplate(
    input_variables=["human_ask"], 
    template=template
)

prompt
```




    PromptTemplate(input_variables=['human_ask'], template='You are a helpful AI instrcutor.\n\nHuman: {human_ask}\nAssistant:')



Now imagine in the above <b>template</b> variable, we want to include all the few shot examples:


```python
few_shots_examples = [
    {
        "review": "I love this course",
        "sentiment": "positive"
    }, {
        "review": "I did not have much experience with AI ",
        "sentiment": "neutral"
    },{
        "review": "This topic is really hard and I will not be able to pass this course.",
        "sentiment": "negative"
    }
]

```

Earlier we also learned how to create a PromptTemplate with two variables: <b>input_variables</b> and <b>template</b>: 

<code>
educational_message_template = PromptTemplate(
    input_variables =['parameter', 'modelname'],
    template = "Write one educational paragraph about {parameter} in Bedrock {modelname} model."
)
</code>

But now in the <b> template </b> we want to pass many examples (few shots) in the format of human mesages and ai messages. So a bit of formatting in template is necessary: 




```python
few_shots_prompt = PromptTemplate(
    input_variables=["review", "sentiment"],
    template= """
             human: {review}
             ai: {sentiment}
            """
)

print(few_shots_prompt.format(**few_shots_examples[0]))
```

    
                 human: I love this course
                 ai: positive
                
    


```python
print(few_shots_prompt.format(**few_shots_examples[1]))
```

    
                 human: I did not have much experience with AI 
                 ai: neutral
                
    

Now we need to assemble everything into one prompt along with new review. That assembeling mechanism is <b> FewShotPromptTemplare</b>:


```python
from langchain import FewShotPromptTemplate
```


```python
instruction = "Identify the sentiment of the following sentence in one word"
new_review = "Wow, this is an amazing framework to use."

few_shot_prompt_template = FewShotPromptTemplate(
    examples=few_shots_examples, # all examples are passed here
    example_prompt=few_shots_prompt, # examples are incorporated into a Prompt Template
    prefix=instruction, # what do we want AI to do
    suffix=new_review, # new review to be analyzed 
    input_variables=["review"], # which variable holds the new input when we call .format()
    
)



print(few_shot_prompt_template.format(review=new_review))

```

    Identify the sentiment of the following sentence in one word
    
    
                 human: I love this course
                 ai: positive
                
    
    
                 human: I did not have much experience with AI 
                 ai: neutral
                
    
    
                 human: This topic is really hard and I will not be able to pass this course.
                 ai: negative
                
    
    Wow, this is an amazing framework to use.
    


```python
res = bedrock_llm.invoke(few_shot_prompt_template.format(review=new_review))
```


```python
res.content
```




    'Positive'



# Chains

We have seen how to get input from user, format it with prompt teamplates and call LLM after. We can connect all these activties into one module as a whole. That is  called a chain in LangChain. 

![image-2.png](LangChain_files/image-2.png)

When you create a chain you can run the entire chain with a single line of code. You can also add memory to the chain.

#### Generic chains: LLM Chain

For more information please see this link:

https://github.com/pinecone-io/examples/blob/master/learn/generation/langchain/handbook/02-langchain-chains.ipynb 


This type of chain is a very generic chain in the sense that it does <b>not</b> have any specific pre-fabricated behavoir. It just does what user has requested to do in the chain. Later we will see more specialized chains that they change input and outputs based on what they are instructed to do.

The LLM generic chains do not change the input of the chain and do not change the format the output beyond what is already instructed by the creator of the chain.  

We use <b>LLMChain</b> in LangChain to implement this type of chain. Please consider that we do not need to do string interpolate by format() when we use chain. The chain itself does that for us:


```python
from langchain.chains import LLMChain

educational_message_template = PromptTemplate(
    input_variables =['parameter', 'modelname'],
    template = "Write one educational paragraph about {parameter} in Bedrock {modelname} model."
)
#final_prompt = educational_message_template .format(parameter="top_p" , modelname= 'claude')
print(final_prompt)
bedrock_llm = initialize_llm()


chain = LLMChain(llm=bedrock_llm, prompt=educational_message_template)
chain.run(parameter="top_p", modelname= 'claude')
```

    Write one educational paragraph about top_p in Bedrock claude model.
    

    /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages/langchain_core/_api/deprecation.py:141: LangChainDeprecationWarning: The class `LLMChain` was deprecated in LangChain 0.1.17 and will be removed in 1.0. Use RunnableSequence, e.g., `prompt | llm` instead.
      warn_deprecated(
    /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages/langchain_core/_api/deprecation.py:141: LangChainDeprecationWarning: The method `Chain.run` was deprecated in langchain 0.1.0 and will be removed in 1.0. Use invoke instead.
      warn_deprecated(
    




    "In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity."



Instread of <b>chain.run()</b> we could also use <b>chain.invoke()</b>. As you see below, we need to provide the parameters in the form of <b>input={} </b>: 


```python
chain.invoke(input={"parameter" : "top_p", "modelname" : 'claude'})
```




    {'parameter': 'top_p',
     'modelname': 'claude',
     'text': "In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity."}



We could also pass multiple parameters(inputs) at once and use <b> chain.apply</b>:


```python

educational_message_template = PromptTemplate(
    input_variables =['parameter'],
    template = "Write one educational paragraph about {parameter} in Bedrock Claude model."
)
param_list = [
    {"parameter": "top_p"},
    {"parameter": "top_k"},
    {"parameter": "temperature"}
]


chain = LLMChain(llm=bedrock_llm, prompt=educational_message_template)

chain.apply(param_list)
```




    [{'text': "In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity."},
     {'text': "In the Bedrock Claude model, top_k is a hyperparameter that controls the degree of randomness during the text generation process. It specifies the number of highest-probability tokens (words or subwords) that the model considers at each step when generating text. By limiting the number of tokens considered, top_k introduces a controlled level of randomness, which can help the model explore a more diverse set of outputs and potentially avoid repetitive or degenerate text. The value of top_k is typically set during the model's training or fine-tuning phase, and it can be adjusted to strike a balance between coherence and diversity in the generated text."},
     {'text': 'In the Bedrock Claude model, temperature refers to a hyperparameter that controls the randomness or "creativity" of the model\'s output. A higher temperature value allows the model to generate more diverse and unpredictable responses, while a lower temperature value results in more predictable and conservative outputs. The temperature parameter is typically adjusted during the sampling process, where the model generates text by predicting the next token based on the previous tokens. By modulating the temperature, researchers and developers can strike a balance between coherence and diversity in the model\'s outputs, tailoring it to specific use cases or desired characteristics.'}]



If you want to see how many tokens are used in the above 


```python
chain.generate(param_list)
```




    LLMResult(generations=[[ChatGeneration(text="In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity.", message=AIMessage(content="In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity.", response_metadata={'model_id': 'anthropic.claude-3-sonnet-20240229-v1:0', 'usage': {'prompt_tokens': 22, 'completion_tokens': 171, 'total_tokens': 193}}, id='run-9bd24fec-e5a3-4630-96dc-ff805db70c91-0'))], [ChatGeneration(text="In the Bedrock Claude model, top_k is a hyperparameter that controls the degree of randomness during the text generation process. It specifies the number of highest-probability tokens (words or subwords) that the model considers at each step when generating text. By limiting the number of tokens considered, top_k introduces a controlled level of randomness, which can help the model explore a more diverse set of outputs and potentially avoid repetitive or degenerate text. The value of top_k is typically set during the model's training or fine-tuning phase, and it can be adjusted to strike a balance between coherence and diversity in the generated text.", message=AIMessage(content="In the Bedrock Claude model, top_k is a hyperparameter that controls the degree of randomness during the text generation process. It specifies the number of highest-probability tokens (words or subwords) that the model considers at each step when generating text. By limiting the number of tokens considered, top_k introduces a controlled level of randomness, which can help the model explore a more diverse set of outputs and potentially avoid repetitive or degenerate text. The value of top_k is typically set during the model's training or fine-tuning phase, and it can be adjusted to strike a balance between coherence and diversity in the generated text.", response_metadata={'model_id': 'anthropic.claude-3-sonnet-20240229-v1:0', 'usage': {'prompt_tokens': 22, 'completion_tokens': 140, 'total_tokens': 162}}, id='run-00f3ed75-d090-456b-8589-8d7d4dc338ec-0'))], [ChatGeneration(text='In the Bedrock Claude model, temperature refers to a hyperparameter that controls the randomness or "creativity" of the model\'s output. A higher temperature value allows the model to generate more diverse and unpredictable responses, while a lower temperature value results in more predictable and conservative outputs. The temperature parameter is typically adjusted during the sampling process, where the model generates text by predicting the next token based on the previous tokens. By modulating the temperature, researchers and developers can strike a balance between coherence and diversity in the model\'s outputs, tailoring it to specific use cases or desired characteristics.', message=AIMessage(content='In the Bedrock Claude model, temperature refers to a hyperparameter that controls the randomness or "creativity" of the model\'s output. A higher temperature value allows the model to generate more diverse and unpredictable responses, while a lower temperature value results in more predictable and conservative outputs. The temperature parameter is typically adjusted during the sampling process, where the model generates text by predicting the next token based on the previous tokens. By modulating the temperature, researchers and developers can strike a balance between coherence and diversity in the model\'s outputs, tailoring it to specific use cases or desired characteristics.', response_metadata={'model_id': 'anthropic.claude-3-sonnet-20240229-v1:0', 'usage': {'prompt_tokens': 20, 'completion_tokens': 127, 'total_tokens': 147}}, id='run-19d472cc-7ec5-4cbc-a862-2021ab75760f-0'))]], llm_output={'model_id': 'anthropic.claude-3-sonnet-20240229-v1:0', 'usage': defaultdict(<class 'int'>, {'prompt_tokens': 64, 'completion_tokens': 438, 'total_tokens': 502})}, run=[RunInfo(run_id=UUID('9bd24fec-e5a3-4630-96dc-ff805db70c91')), RunInfo(run_id=UUID('00f3ed75-d090-456b-8589-8d7d4dc338ec')), RunInfo(run_id=UUID('19d472cc-7ec5-4cbc-a862-2021ab75760f'))])



#### Utility Chains: LLMMathChain

LangChain has created chains to do some activities for us. In this case the chain changes our inputs/prompts and it parses the generated output before showing the result to us. 

![image.png](LangChain_files/image.png)


```python
745 ** 0.753
```




    145.4566808899015



If we ask this question from LLM, will we get a correct answer? As you see below the answer is NO:


```python
from langchain.chains import LLMChain

calculator_template = PromptTemplate(
    input_variables =['base', 'power'],
    template = "what is {base} raised to the {power} power?"
)

print(calculator_template)
bedrock_llm = initialize_llm()


chain = LLMChain(llm=bedrock_llm, prompt=calculator_template)
chain.run(base=745, power= 0.753)
```

    input_variables=['base', 'power'] template='what is {base} raised to the {power} power?'
    




    'To calculate 745 raised to the 0.753 power, we can use the following steps:\n\n1) Take the logarithm (base 10) of both the base (745) and the exponent (0.753):\nlog(745) = 2.872\nlog(0.753) = -0.123\n\n2) Multiply the logarithm of the base by the exponent:\n2.872 * (-0.123) = -0.353\n\n3) Take the antilogarithm (base 10) of the result to get the final answer:\n10^(-0.353) = 0.444\n\nTherefore, 745 raised to the 0.753 power is approximately equal to 0.444.'



Now let's solve this problem with a speciazlized math chain (<b>LLMMacthChain</b> ) that LangChain offers.It asks LLM to generate a Python code to solve a mathematical problem and after getting the code, it runs the code and shows the response. 

First consider that in the following code, I had to use <b>from_llm</b> after <b>LLMMacthChain</b> call. 

After initilaizing <b>LLMMacthChain</b>  I also wanted to see what LLMMathChain does behind the scene when I run it. For that, I used <b> llm_math.prompt.template</b> in the last line of the following cell. As you can see in the reponse, <b>LLMMacthChain</b>  changes my prompt (user prompt) to something else:



```python
from langchain import LLMMathChain
bedrock_llm = initialize_llm()
llm_math = LLMMathChain.from_llm(bedrock_llm, verbose=True)
print(llm_math.prompt.template)

```

    Translate a math problem into a expression that can be executed using Python's numexpr library. Use the output of running this code to answer the question.
    
    Question: ${{Question with math problem.}}
    ```text
    ${{single line mathematical expression that solves the problem}}
    ```
    ...numexpr.evaluate(text)...
    ```output
    ${{Output of running the code}}
    ```
    Answer: ${{Answer}}
    
    Begin.
    
    Question: What is 37593 * 67?
    ```text
    37593 * 67
    ```
    ...numexpr.evaluate("37593 * 67")...
    ```output
    2518731
    ```
    Answer: 2518731
    
    Question: 37593^(1/5)
    ```text
    37593**(1/5)
    ```
    ...numexpr.evaluate("37593**(1/5)")...
    ```output
    8.222831614237718
    ```
    Answer: 8.222831614237718
    
    Question: {question}
    
    

In the above output you see that through few-shots prompt technqiue, LLMMathChain is generating a Python expressions like numexpr.evaluate(). 

#### NOTE: ####  
I was getting error due to the fact that Bedrock LLMs generate code with ... before and ... after the numexpr code. So I had to enforce not to do that by adding extra instruction in the prompt. I added this in the following code: Just generate an numexpr.evaluate() expresion for that.


```python
res=llm_math.run("what is 745 raised to the 0.753 power? Just generate an numexpr.evaluate() expresion for that. ")

```

    
    
    [1m> Entering new LLMMathChain chain...[0m
    what is 745 raised to the 0.753 power? Just generate an numexpr.evaluate() expresion for that. [32;1m[1;3m```text
    745**(0.753)
    ```
    ...numexpr.evaluate("745**(0.753)")...
    [0m
    Answer: [33;1m[1;3m145.4566808899015[0m
    [1m> Finished chain.[0m
    

#### Utility Chains: Sequential chain

Another utility chain is sequantial chain. We can connect two chains sequentially through <b> SequentialChain </b> utility chain.

In the following example, I used a chain called "educational chain" to answer a question. Then I used its "output" as input to the second chain (quiz_chain)  to generate multiple choice questions. Then I chained the sequantially.

![image.png](LangChain_files/image.png)


```python
from langchain.chains import SequentialChain
educational_text = PromptTemplate(
    input_variables =['parameter'],
    template = "Write one educational paragraph about {parameter} in Bedrock Claude model."
)

educational_chain = LLMChain(llm=bedrock_llm, prompt=educational_text, output_key="text1")


quiz_text = PromptTemplate(
    input_variables=["text1"], 
    template="""Generate a multiple choice question for this text:{text1} """
)

quiz_chain = LLMChain(llm=bedrock_llm, prompt=quiz_text, output_key="text2")

seq_chain = SequentialChain(
    chains = [educational_chain , quiz_chain],
    input_variables = ["parameter"],
    output_variables = ["text1","text2"]
)

seq_chain({"parameter": "top_p"})

```

    /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages/langchain_core/_api/deprecation.py:141: LangChainDeprecationWarning: The method `Chain.__call__` was deprecated in langchain 0.1.0 and will be removed in 1.0. Use invoke instead.
      warn_deprecated(
    




    {'parameter': 'top_p',
     'text1': "In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity.",
     'text2': 'Question: What is the primary advantage of using top_p sampling in the Bedrock Claude model compared to top-k sampling?\n\nA. It generates more repetitive text.\nB. It allows for the inclusion of lower-probability tokens, leading to more diverse text generation.\nC. It considers only the top-k tokens, resulting in less diverse text generation.\nD. It does not consider the probability distribution of the tokens.'}




```python
print(seq_chain({"parameter": "top_p"})["text1"])
```

    In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity.
    


```python
print(seq_chain({"parameter": "top_p"})["text2"])
```

    Question: What is the primary advantage of using top_p sampling in the Bedrock Claude model compared to top-k sampling?
    
    A. It generates more repetitive text.
    B. It allows for the inclusion of lower-probability tokens, leading to more diverse text generation.
    C. It considers only the top-k tokens, resulting in less diverse text generation.
    D. It does not consider the probability distribution of the tokens.
    

## Using | operator to create a chain 

The pipe (|) operator is part of LangChain Expression Language (LCEL). LangChain has started to use a different methods to create more complex chains rather than creating them utility chains. 

For example, rather than using LLMChain that I expalined above, we can use pipe (|)  operator to create a chain as shown below: 



```python
#from langchain.chains import LLMChain

educational_message_template = PromptTemplate( 
    input_variables =['parameter', 'modelname'], 
    template = "Write one educational paragraph about {parameter} in Bedrock {modelname} model." ) 
#final_prompt = educational_message_template .format(parameter="top_p" , modelname= 'claude') print(final_prompt) bedrock_llm = initialize_llm()

#chain = LLMChain(llm=bedrock_llm, prompt=educational_message_template) #chain.run(parameter="top_p", modelname= 'claude')


chain1 = educational_message_template | bedrock_llm 
```


```python
text1=chain1.invoke(input={"parameter" : "top_p", "modelname" : 'claude'}).content
text1
```




    "In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity."



We can also achive the same by using <b>.pipe()</b> method as shown below:


```python
quiz_template = PromptTemplate(
    input_variables=["text1"], 
    template="""Generate a multiple choice question for this text: {text1}. """
)
chain2 = quiz_template.pipe(bedrock_llm)
```


```python
print(chain2.invoke(input={"text1" : {text1}}).content)
```

    What is the purpose of the top_p sampling technique in the Bedrock Claude model?
    
    A. To select the most probable tokens from the model's output distribution.
    B. To consider only the top-k tokens during text generation.
    C. To allow for the inclusion of lower-probability tokens, leading to more diverse and less repetitive text generation.
    D. To ensure that the selected tokens represent a small portion of the probability mass.
    

NOTE: We can also use | operator to create sequential chain rather than using SequentialChain

## Output Parsers

We can use output parsers to get the response back in a specified format.

![image.png](LangChain_files/image.png)

### strOutputParser()

Compare the following code block with the first example under "Using | operator to create a chain " title above that we had to use .content. We use this techique to get only the string part of response:


```python
from langchain.chains import SequentialChain

from langchain_core.output_parsers import StrOutputParser


educational_message_template = PromptTemplate( 
    input_variables =['parameter', 'modelname'], 
    template = "Write one educational paragraph about {parameter} in Bedrock {modelname} model." ) 
chain = educational_message_template | bedrock_llm | StrOutputParser()
```


```python
chain.invoke(input={"parameter" : "top_p", "modelname" : 'claude'})
```




    "In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity."



Now that you know what Output Parser is you can add that to a more complex chain, where we have two steps chain. As you see, in the following code we do not define the outputs in the PromptTemplate. The output of the educational_chain is passed to quiz_text PromptTemplate:


```python
from langchain_core.output_parsers import StrOutputParser
educational_message_template = PromptTemplate( 
    input_variables =['parameter', 'modelname'], 
    template = "Write one educational paragraph about {parameter} in Bedrock {modelname} model." ) 

educational_chain = LLMChain(llm=bedrock_llm, prompt=educational_text)


quiz_text = PromptTemplate(
    input_variables=["text1"], 
    template="""Generate a multiple choice question for this text:{text1} """
)

quiz_chain = LLMChain(llm=bedrock_llm, prompt=quiz_text)

combined_chain = educational_message_template | bedrock_llm | StrOutputParser() | quiz_chain
combined_chain.invoke(input={"parameter" : "top_p", "modelname" : 'claude'})
```




    {'text1': "In the Bedrock Claude model, top_p is a sampling technique used during the text generation process. It is an alternative to the more commonly used top-k sampling method. Top_p sampling works by selecting the most probable tokens from the model's output distribution, but instead of considering only the top-k tokens, it considers the smallest set of tokens whose cumulative probability mass exceeds a specified threshold (p). This approach can lead to more diverse and less repetitive text generation, as it allows for the inclusion of lower-probability tokens that may not be present in the top-k set. The value of p is typically set to a high value, such as 0.9 or 0.95, to ensure that the selected tokens represent a significant portion of the probability mass while still allowing for some diversity.",
     'text': 'Question: What is the primary advantage of using top_p sampling in the Bedrock Claude model compared to top-k sampling?\n\nA. It generates more repetitive text.\nB. It allows for the inclusion of lower-probability tokens, leading to more diverse text generation.\nC. It considers only the top-k tokens, resulting in less diverse text generation.\nD. It does not consider the probability distribution of the tokens.'}



### structuredOutputParser()

When we want the output to be in a specific structured format, we use this technique. The first thing we should do us to create the ResponseSchema. It has names and descriptions:

![image.png](LangChain_files/image.png)

Imagine we use ResponseSchema to create instructions to LLM about how to format the outputs later. It may have multiple fileds and each field has its own description.


```python
from langchain.output_parsers import StructuredOutputParser, ResponseSchema
from langchain_core.prompts import PromptTemplate


response_schemas = [
    ResponseSchema(name="parameter", description="parameter entered by user"),
    ResponseSchema(name="usage", description="One line explaining what that is the usage of the given parameter by user"),
    ResponseSchema(name="example", description="An example of how that parameter changes the response from LLM"),
    ResponseSchema(name="usecase", description="a paragraph that shows how that helps in real world")
]
output_parser = StructuredOutputParser.from_response_schemas(response_schemas)
format_instructions = output_parser.get_format_instructions()

print(format_instructions)
```

    The output should be a markdown code snippet formatted in the following schema, including the leading and trailing "```json" and "```":
    
    ```json
    {
    	"parameter": string  // parameter entered by user
    	"usage": string  // One line explaining what that is the usage of the given parameter by user
    	"example": string  // An example of how that parameter changes the response from LLM
    	"usecase": string  // a paragraph that shows how that helps in real world
    }
    ```
    

Now that you have a complex instruction about the way the output must look like, we pass that as one of the requirements to the prompt through PromptTemplate:

![image.png](LangChain_files/image.png)


```python
prompt = PromptTemplate(
    template="Provide the usage, an example of how the parameter is used and one use case of this parameter in LLM: {parameter}.\n{format_instructions}",
    input_variables=["parameter"],
    partial_variables={"format_instructions": format_instructions}  # this format instruction is part of the template and is coming from response schema (prev cell)
)
bedrock_llm = initialize_llm()

chain = prompt | bedrock_llm | output_parser

chain.invoke("top_p")
```




    {'parameter': 'top_p',
     'usage': 'The top_p parameter controls the nucleus sampling strategy used for text generation.',
     'example': 'With top_p=0.9, the model will consider the top 90% most likely tokens at each step during generation, leading to more diverse and less repetitive outputs compared to greedy sampling.',
     'usecase': 'The top_p parameter is useful when you want to balance between diversity and coherence in the generated text. By restricting the sampling to the most likely tokens, it helps prevent the model from generating nonsensical or irrelevant text, while still allowing for some variation and creativity. This can be particularly useful in creative writing tasks, dialogue generation, or any application where you want the output to be both coherent and diverse. It can also help mitigate the risk of generating offensive or inappropriate content by excluding low-probability tokens that may be more likely to contain such content.'}



### comma separated list 

When we want to get the output in the form of comma separated format


```python
from langchain.output_parsers import CommaSeparatedListOutputParser
output_parser = CommaSeparatedListOutputParser()
format_instructions = output_parser.get_format_instructions()
prompt = PromptTemplate(
    template="List five {topics_to_learn_in}.\n{format_instructions}",
    input_variables=["topics_to_learn_in"],
    partial_variables={"format_instructions": format_instructions},
)
chain = prompt | bedrock_llm  | output_parser 
```


```python
print(format_instructions)
```

    Your response should be a list of comma separated values, eg: `foo, bar, baz` or `foo,bar,baz`
    


```python
chain.invoke({"topics_to_learn_in": "AI"})
```




    ['ChatGPT', 'Alexa', 'Siri', 'Google Assistant', 'IBM Watson.']



# Memory

To save the previous conversation with chatbot we need to create a memory and give the context to the AI when we converse.

LangChain create and manages the memory for us. At the begning the memory is empty:

![image.png](LangChain_files/image.png)

Then in the next round, the memory along with prompt 2 is sent to LLM. So LLM will know about the history of the conversation:
![image.png](LangChain_files/image.png)

There are different types of memories:
- Store the entire conversation (ConversationBufferMemory)
- Store only the last few messages (ConversationBufferWindowMemory)
- Store a summary of the conversation (ConversatioSummaryMemory)

These memories work with chains in LangChain

#### Using memory with LLMChain (using ConversationBufferMemory)
In this case when we create a chain, we add memory to it:


```python
from langchain.memory import ConversationBufferMemory
from langchain.chains import LLMChain

educational_message_template = PromptTemplate(
    input_variables =['history', 'input'],
    template = '''You are an AI expert.
    chat_history : {history}
    human: {input}
    ai: '''
)

memory = ConversationBufferMemory()

bedrock_llm = initialize_llm()


chain = LLMChain(llm=bedrock_llm, prompt=educational_message_template, memory = memory, verbose=True)

print(chain.run(input="why a parameter like top_p is important at all?"))
```

    
    
    [1m> Entering new LLMChain chain...[0m
    Prompt after formatting:
    [32;1m[1;3mYou are an AI expert.
        chat_history : 
        human: why a parameter like top_p is important at all?
        ai: [0m
    
    [1m> Finished chain.[0m
    The `top_p` parameter, also known as nucleus sampling or top-p sampling, is an important technique used in natural language generation models, such as GPT (Generative Pre-trained Transformer) models. It helps to control the diversity and creativity of the generated text while maintaining coherence and relevance.
    
    Here are a few reasons why the `top_p` parameter is important:
    
    1. **Mitigating the repetition problem**: Language models can sometimes generate repetitive or nonsensical text, especially when generating longer sequences. The `top_p` parameter helps to mitigate this issue by introducing controlled randomness in the text generation process, leading to more diverse and interesting outputs.
    
    2. **Balancing diversity and coherence**: By adjusting the `top_p` value, you can control the trade-off between diversity and coherence in the generated text. A lower `top_p` value will result in more diverse but potentially less coherent text, while a higher `top_p` value will produce more coherent but potentially less diverse text.
    
    3. **Avoiding unlikely or nonsensical outputs**: Language models can sometimes assign high probabilities to unlikely or nonsensical words or phrases. The `top_p` parameter helps to filter out these low-probability tokens, ensuring that the generated text remains relevant and meaningful.
    
    4. **Controlling the level of creativity**: The `top_p` parameter can be used to control the level of creativity in the generated text. A lower `top_p` value will allow for more creative and unexpected outputs, while a higher `top_p` value will produce more conservative and predictable text.
    
    5. **Adapting to different domains or tasks**: Different domains or tasks may require different levels of diversity or coherence in the generated text. The `top_p` parameter allows you to fine-tune the model's behavior to suit the specific requirements of your application.
    
    In summary, the `top_p` parameter is an important tool for controlling the trade-off between diversity, coherence, and relevance in natural language generation models. By carefully tuning this parameter, you can optimize the model's output for your specific use case, ensuring that the generated text is both interesting and meaningful.
    


```python
print(chain.run(input="explain number 5 to me"))
```

    
    
    [1m> Entering new LLMChain chain...[0m
    Prompt after formatting:
    [32;1m[1;3mYou are an AI expert.
        chat_history : Human: why a parameter like top_p is important at all?
    AI: The `top_p` parameter, also known as nucleus sampling or top-p sampling, is an important technique used in natural language generation models, such as GPT (Generative Pre-trained Transformer) models. It helps to control the diversity and creativity of the generated text while maintaining coherence and relevance.
    
    Here are a few reasons why the `top_p` parameter is important:
    
    1. **Mitigating the repetition problem**: Language models can sometimes generate repetitive or nonsensical text, especially when generating longer sequences. The `top_p` parameter helps to mitigate this issue by introducing controlled randomness in the text generation process, leading to more diverse and interesting outputs.
    
    2. **Balancing diversity and coherence**: By adjusting the `top_p` value, you can control the trade-off between diversity and coherence in the generated text. A lower `top_p` value will result in more diverse but potentially less coherent text, while a higher `top_p` value will produce more coherent but potentially less diverse text.
    
    3. **Avoiding unlikely or nonsensical outputs**: Language models can sometimes assign high probabilities to unlikely or nonsensical words or phrases. The `top_p` parameter helps to filter out these low-probability tokens, ensuring that the generated text remains relevant and meaningful.
    
    4. **Controlling the level of creativity**: The `top_p` parameter can be used to control the level of creativity in the generated text. A lower `top_p` value will allow for more creative and unexpected outputs, while a higher `top_p` value will produce more conservative and predictable text.
    
    5. **Adapting to different domains or tasks**: Different domains or tasks may require different levels of diversity or coherence in the generated text. The `top_p` parameter allows you to fine-tune the model's behavior to suit the specific requirements of your application.
    
    In summary, the `top_p` parameter is an important tool for controlling the trade-off between diversity, coherence, and relevance in natural language generation models. By carefully tuning this parameter, you can optimize the model's output for your specific use case, ensuring that the generated text is both interesting and meaningful.
        human: explain number 5 to me
        ai: [0m
    
    [1m> Finished chain.[0m
    Sure, let me elaborate on point number 5 regarding how the `top_p` parameter can be useful for adapting to different domains or tasks.
    
    Different domains or applications may have varying requirements when it comes to the desired level of diversity, coherence, and relevance in the generated text. For example:
    
    1. **Creative writing**: In creative writing tasks, such as story generation or poetry composition, you may want to encourage more diversity and creativity in the generated text. In this case, a lower `top_p` value could be beneficial, as it allows the model to explore a wider range of possible word choices, leading to more unexpected and imaginative outputs.
    
    2. **Factual or technical writing**: On the other hand, for tasks like generating technical documentation, news articles, or scientific reports, coherence and relevance may be more important than diversity. In such cases, a higher `top_p` value could be preferable, as it helps the model stay focused on the most likely and relevant word choices, resulting in more coherent and factual text.
    
    3. **Conversational agents**: In the context of conversational AI systems, such as chatbots or virtual assistants, the desired level of diversity and coherence may depend on the specific use case. For task-oriented dialogues (e.g., booking a flight or scheduling an appointment), coherence and relevance are crucial, so a higher `top_p` value might be appropriate. However, for open-ended conversations or creative storytelling, a lower `top_p` value could make the responses more engaging and diverse.
    
    4. **Machine translation**: In machine translation tasks, where the goal is to accurately translate text from one language to another, a higher `top_p` value may be preferred to ensure that the generated translations are coherent and faithful to the original text.
    
    By adjusting the `top_p` parameter, you can fine-tune the language model's behavior to better suit the specific requirements of the domain or task at hand. This flexibility allows you to strike the right balance between diversity, coherence, and relevance, ultimately improving the quality and appropriateness of the generated text for your particular use case.
    

#### Using memory with Conversation Chain 
If we use ConversationChain we do not need to create PromptTemplate and history as we did in LLMChain. Here is a simple example:




```python
from langchain.chains import ConversationChain
memory = ConversationBufferMemory(memory_key="history")



chain = ConversationChain(llm=bedrock_llm, memory = memory, verbose=True)

chain.invoke({"input": "Which country has the tallest tower?"})
```

    /home/ec2-user/anaconda3/envs/python3/lib/python3.10/site-packages/langchain_core/_api/deprecation.py:141: LangChainDeprecationWarning: The class `ConversationChain` was deprecated in LangChain 0.2.7 and will be removed in 1.0. Use RunnableWithMessageHistory: https://api.python.langchain.com/en/latest/runnables/langchain_core.runnables.history.RunnableWithMessageHistory.html instead.
      warn_deprecated(
    

    
    
    [1m> Entering new ConversationChain chain...[0m
    Prompt after formatting:
    [32;1m[1;3mThe following is a friendly conversation between a human and an AI. The AI is talkative and provides lots of specific details from its context. If the AI does not know the answer to a question, it truthfully says it does not know.
    
    Current conversation:
    
    Human: Which country has the tallest tower?
    AI:[0m
    
    [1m> Finished chain.[0m
    




    {'input': 'Which country has the tallest tower?',
     'history': '',
     'response': "The country with the tallest tower in the world is the United Arab Emirates. The Burj Khalifa in Dubai stands at an incredible height of 828 meters (2,717 feet) and has been the tallest building in the world since its completion in 2010.\n\nSome key facts about the Burj Khalifa:\n\n- It has 163 habitable floors in addition to over 40 maintenance levels.\n- The primary structure is reinforced concrete. The exterior cladding is reflective glazing.\n- It took over 100,000 tons of concrete and 55,000 tons of steel rebar to construct.\n- The building can withstand winds of up to 95 mph (153 km/h).\n- It has the highest outdoor observation deck in the world on the 148th floor at 555 meters (1,821 feet).\n- The total cost of construction was around $1.5 billion USD.\n\nSo in summary, with its record-breaking 828 meter height, the iconic Burj Khalifa in Dubai, United Arab Emirates is definitively the world's tallest tower or skyscraper currently standing."}




```python
chain.invoke({"input": "Ah, I thought CN tower was the one"})
```

    
    
    [1m> Entering new ConversationChain chain...[0m
    Prompt after formatting:
    [32;1m[1;3mThe following is a friendly conversation between a human and an AI. The AI is talkative and provides lots of specific details from its context. If the AI does not know the answer to a question, it truthfully says it does not know.
    
    Current conversation:
    Human: Which country has the tallest tower?
    AI: The country with the tallest tower in the world is the United Arab Emirates. The Burj Khalifa in Dubai stands at an incredible height of 828 meters (2,717 feet) and has been the tallest building in the world since its completion in 2010.
    
    Some key facts about the Burj Khalifa:
    
    - It has 163 habitable floors in addition to over 40 maintenance levels.
    - The primary structure is reinforced concrete. The exterior cladding is reflective glazing.
    - It took over 100,000 tons of concrete and 55,000 tons of steel rebar to construct.
    - The building can withstand winds of up to 95 mph (153 km/h).
    - It has the highest outdoor observation deck in the world on the 148th floor at 555 meters (1,821 feet).
    - The total cost of construction was around $1.5 billion USD.
    
    So in summary, with its record-breaking 828 meter height, the iconic Burj Khalifa in Dubai, United Arab Emirates is definitively the world's tallest tower or skyscraper currently standing.
    Human: Ah, I thought CN tower was the one
    AI:[0m
    
    [1m> Finished chain.[0m
    




    {'input': 'Ah, I thought CN tower was the one',
     'history': "Human: Which country has the tallest tower?\nAI: The country with the tallest tower in the world is the United Arab Emirates. The Burj Khalifa in Dubai stands at an incredible height of 828 meters (2,717 feet) and has been the tallest building in the world since its completion in 2010.\n\nSome key facts about the Burj Khalifa:\n\n- It has 163 habitable floors in addition to over 40 maintenance levels.\n- The primary structure is reinforced concrete. The exterior cladding is reflective glazing.\n- It took over 100,000 tons of concrete and 55,000 tons of steel rebar to construct.\n- The building can withstand winds of up to 95 mph (153 km/h).\n- It has the highest outdoor observation deck in the world on the 148th floor at 555 meters (1,821 feet).\n- The total cost of construction was around $1.5 billion USD.\n\nSo in summary, with its record-breaking 828 meter height, the iconic Burj Khalifa in Dubai, United Arab Emirates is definitively the world's tallest tower or skyscraper currently standing.",
     'response': "No, the CN Tower in Toronto, Canada is not the tallest tower in the world. It is tall at 553.3 meters (1,815.4 feet), but significantly shorter than the Burj Khalifa's 828 meters.\n\nSome key facts about the CN Tower:\n\n- It was the world's tallest free-standing structure from 1976 until 2007 when the Burj Khalifa surpassed it in height during construction.\n\n- It remains the tallest tower in the Western Hemisphere.\n\n- The main concrete core of the tower is reinforced by 7 hexagonal levels of steel.\n\n- It has observational and revolving restaurants near the top.\n\n- It was an important telecommunications hub when first built, housing microwave receivers and transmitters.\n\nSo while the CN Tower held the world's tallest title for over 30 years, it has been surpassed by taller towers like the Burj Khalifa in more recent decades. But it remains an iconic landmark and major attraction in Toronto."}




```python
chain.invoke({"input": "Which one was built first?"})
```

    
    
    [1m> Entering new ConversationChain chain...[0m
    Prompt after formatting:
    [32;1m[1;3mThe following is a friendly conversation between a human and an AI. The AI is talkative and provides lots of specific details from its context. If the AI does not know the answer to a question, it truthfully says it does not know.
    
    Current conversation:
    Human: Which country has the tallest tower?
    AI: The country with the tallest tower in the world is the United Arab Emirates. The Burj Khalifa in Dubai stands at an incredible height of 828 meters (2,717 feet) and has been the tallest building in the world since its completion in 2010.
    
    Some key facts about the Burj Khalifa:
    
    - It has 163 habitable floors in addition to over 40 maintenance levels.
    - The primary structure is reinforced concrete. The exterior cladding is reflective glazing.
    - It took over 100,000 tons of concrete and 55,000 tons of steel rebar to construct.
    - The building can withstand winds of up to 95 mph (153 km/h).
    - It has the highest outdoor observation deck in the world on the 148th floor at 555 meters (1,821 feet).
    - The total cost of construction was around $1.5 billion USD.
    
    So in summary, with its record-breaking 828 meter height, the iconic Burj Khalifa in Dubai, United Arab Emirates is definitively the world's tallest tower or skyscraper currently standing.
    Human: Ah, I thought CN tower was the one
    AI: No, the CN Tower in Toronto, Canada is not the tallest tower in the world. It is tall at 553.3 meters (1,815.4 feet), but significantly shorter than the Burj Khalifa's 828 meters.
    
    Some key facts about the CN Tower:
    
    - It was the world's tallest free-standing structure from 1976 until 2007 when the Burj Khalifa surpassed it in height during construction.
    
    - It remains the tallest tower in the Western Hemisphere.
    
    - The main concrete core of the tower is reinforced by 7 hexagonal levels of steel.
    
    - It has observational and revolving restaurants near the top.
    
    - It was an important telecommunications hub when first built, housing microwave receivers and transmitters.
    
    So while the CN Tower held the world's tallest title for over 30 years, it has been surpassed by taller towers like the Burj Khalifa in more recent decades. But it remains an iconic landmark and major attraction in Toronto.
    Human: Which one was built first?
    AI:[0m
    
    [1m> Finished chain.[0m
    




    {'input': 'Which one was built first?',
     'history': "Human: Which country has the tallest tower?\nAI: The country with the tallest tower in the world is the United Arab Emirates. The Burj Khalifa in Dubai stands at an incredible height of 828 meters (2,717 feet) and has been the tallest building in the world since its completion in 2010.\n\nSome key facts about the Burj Khalifa:\n\n- It has 163 habitable floors in addition to over 40 maintenance levels.\n- The primary structure is reinforced concrete. The exterior cladding is reflective glazing.\n- It took over 100,000 tons of concrete and 55,000 tons of steel rebar to construct.\n- The building can withstand winds of up to 95 mph (153 km/h).\n- It has the highest outdoor observation deck in the world on the 148th floor at 555 meters (1,821 feet).\n- The total cost of construction was around $1.5 billion USD.\n\nSo in summary, with its record-breaking 828 meter height, the iconic Burj Khalifa in Dubai, United Arab Emirates is definitively the world's tallest tower or skyscraper currently standing.\nHuman: Ah, I thought CN tower was the one\nAI: No, the CN Tower in Toronto, Canada is not the tallest tower in the world. It is tall at 553.3 meters (1,815.4 feet), but significantly shorter than the Burj Khalifa's 828 meters.\n\nSome key facts about the CN Tower:\n\n- It was the world's tallest free-standing structure from 1976 until 2007 when the Burj Khalifa surpassed it in height during construction.\n\n- It remains the tallest tower in the Western Hemisphere.\n\n- The main concrete core of the tower is reinforced by 7 hexagonal levels of steel.\n\n- It has observational and revolving restaurants near the top.\n\n- It was an important telecommunications hub when first built, housing microwave receivers and transmitters.\n\nSo while the CN Tower held the world's tallest title for over 30 years, it has been surpassed by taller towers like the Burj Khalifa in more recent decades. But it remains an iconic landmark and major attraction in Toronto.",
     'response': "The CN Tower in Toronto, Canada was built first, before the Burj Khalifa in Dubai, United Arab Emirates.\n\nHere are some key dates:\n\nCN Tower:\n- Construction began in 1973\n- It was topped out in 1975 when it became the world's tallest free-standing structure\n- It was officially completed in 1976\n\nBurj Khalifa: \n- Construction began in 2004\n- It surpassed the CN Tower in height in 2007 during construction\n- It was officially opened and completed in 2010\n\nSo the CN Tower had about a 34 year head start, having been conceived and built in the 1970s when it set new standards for skyscraper heights and engineering. The Burj Khalifa then broke new ground in the 2000s when it blew past the CN Tower to become the new world's tallest building.\n\nDespite being the older structure, the CN Tower remains an iconic landmark and one of the most famous towers in the world, even after being surpassed in height by newer skyscrapers like the Burj Khalifa."}



#### Using ConversationBufferWindowMemory


```python
from langchain.memory import ConversationBufferWindowMemory
from langchain.chains import ConversationChain

memory = ConversationBufferWindowMemory(k=1)


chain = ConversationChain(llm=bedrock_llm, memory=memory)

chain.invoke({"input": "Hello, my name is Morteza, how are you today?"})
```




    {'input': 'Hello, my name is Morteza, how are you today?',
     'history': '',
     'response': "Hello Morteza, it's wonderful to meet you! I'm doing very well today, thank you for asking. I'm an AI assistant created by Anthropic to be helpful, honest, and friendly in our conversations. I have a broad base of knowledge that I can draw upon, but I'll let you know if there are any gaps or topics I'm uncertain about. How has your day been going so far?"}




```python
print(chain.invoke({"input": "I am doing great. Today is a sunny day"}))
```

    {'input': 'I am doing great. Today is a sunny day', 'history': "Human: Hello, my name is Morteza, how are you today?\nAI: Hello Morteza, it's wonderful to meet you! I'm doing very well today, thank you for asking. I'm an AI assistant created by Anthropic to be helpful, honest, and friendly in our conversations. I have a broad base of knowledge that I can draw upon, but I'll let you know if there are any gaps or topics I'm uncertain about. How has your day been going so far?", 'response': "That's wonderful that you're having a great day so far! Sunny days can really lift the spirits. I don't actually experience the weather myself, but I know sunshine and nice weather is enjoyable for humans. Since it's sunny out, maybe you'll have a chance to spend some time outdoors today? Even just a short walk can be refreshing on a beautiful day. Or if you prefer indoor activities, the natural light can make reading, working, or pursuing hobbies more pleasant. Please let me know if you have any plans to take advantage of the nice weather or if there's anything else I can try to help with!"}
    


```python
print(chain.invoke({"input": "what was my name?"}))
```

    {'input': 'what was my name?', 'history': "Human: I am doing great. Today is a sunny day\nAI: That's wonderful that you're having a great day so far! Sunny days can really lift the spirits. I don't actually experience the weather myself, but I know sunshine and nice weather is enjoyable for humans. Since it's sunny out, maybe you'll have a chance to spend some time outdoors today? Even just a short walk can be refreshing on a beautiful day. Or if you prefer indoor activities, the natural light can make reading, working, or pursuing hobbies more pleasant. Please let me know if you have any plans to take advantage of the nice weather or if there's anything else I can try to help with!", 'response': "I'm afraid I don't actually know your name since you didn't provide it in our conversation. As an AI assistant without access to personal information about you, I can only respond based on what is stated in our dialog. If you share your name with me, I'd be happy to use it, but if not, I'm comfortable continuing our friendly conversation without knowing your specific name. Please let me know if you have any other questions!"}
    

#### Using ConversationSummaryMemory

We summarize the entire conversation before sending that to the LLM. We need to use an LLM itself to do summarization.


```python
from langchain.memory import ConversationSummaryMemory, ChatMessageHistory
from langchain.chains import ConversationChain
conversation_with_summary = ConversationChain(
    llm=bedrock_llm,
    memory=ConversationSummaryMemory(llm=bedrock_llm),
    verbose=True
)
conversation_with_summary.invoke(input="Hello, my name is Morteza, how are you doing today?")
```

    
    
    [1m> Entering new ConversationChain chain...[0m
    Prompt after formatting:
    [32;1m[1;3mThe following is a friendly conversation between a human and an AI. The AI is talkative and provides lots of specific details from its context. If the AI does not know the answer to a question, it truthfully says it does not know.
    
    Current conversation:
    
    Human: Hello, my name is Morteza, how are you doing today?
    AI:[0m
    
    [1m> Finished chain.[0m
    




    {'input': 'Hello, my name is Morteza, how are you doing today?',
     'history': '',
     'response': "Hello Morteza! It's wonderful to meet you. I'm doing very well today, thank you for asking. I'm an AI assistant created by Anthropic to be helpful, honest, and friendly in our conversations. I have a broad base of knowledge that I can draw upon, but I'll let you know if there are any gaps or topics I'm uncertain about. How has your day been going so far?"}




```python
conversation_with_summary.invoke(input="I am doing great so far. It's sunny day here. How is the weather in your city?")
```

    
    
    [1m> Entering new ConversationChain chain...[0m
    Prompt after formatting:
    [32;1m[1;3mThe following is a friendly conversation between a human and an AI. The AI is talkative and provides lots of specific details from its context. If the AI does not know the answer to a question, it truthfully says it does not know.
    
    Current conversation:
    The human introduces himself as Morteza and greets the AI, asking how it is doing. The AI greets Morteza warmly, introduces itself as an AI assistant created by Anthropic to be helpful, honest and friendly. It expresses that it is doing well and inquires about how Morteza's day has been going so far.
    Human: I am doing great so far. It's sunny day here. How is the weather in your city?
    AI:[0m
    
    [1m> Finished chain.[0m
    




    {'input': "I am doing great so far. It's sunny day here. How is the weather in your city?",
     'history': "The human introduces himself as Morteza and greets the AI, asking how it is doing. The AI greets Morteza warmly, introduces itself as an AI assistant created by Anthropic to be helpful, honest and friendly. It expresses that it is doing well and inquires about how Morteza's day has been going so far.",
     'response': "I don't actually experience weather or live in any physical location since I'm an AI assistant without a physical form. I don't have a concept of cities or weather patterns. As an AI, I don't have a subjective experience of the world in that sense. I'm Claude, an AI created by Anthropic to be helpful, honest and harmless in our conversations."}




```python
conversation_with_summary.invoke(input="Ah sorry I forgot you are just an AI. Do you remember my name?")
```

    
    
    [1m> Entering new ConversationChain chain...[0m
    Prompt after formatting:
    [32;1m[1;3mThe following is a friendly conversation between a human and an AI. The AI is talkative and provides lots of specific details from its context. If the AI does not know the answer to a question, it truthfully says it does not know.
    
    Current conversation:
    The human introduces himself as Morteza and greets the AI, asking how it is doing. The AI greets Morteza warmly, introduces itself as an AI assistant created by Anthropic to be helpful, honest and friendly. It expresses that it is doing well and inquires about how Morteza's day has been going so far. Morteza says he is doing great and that it is a sunny day where he is, then asks about the weather in the AI's city. The AI clarifies that as an AI it does not actually experience weather or live in any physical location, as it does not have a subjective experience of the world in that sense. The AI reiterates that it is Claude, an AI created by Anthropic to be helpful, honest and harmless in conversations.
    Human: Ah sorry I forgot you are just an AI. Do you remember my name?
    AI:[0m
    
    [1m> Finished chain.[0m
    




    {'input': 'Ah sorry I forgot you are just an AI. Do you remember my name?',
     'history': "The human introduces himself as Morteza and greets the AI, asking how it is doing. The AI greets Morteza warmly, introduces itself as an AI assistant created by Anthropic to be helpful, honest and friendly. It expresses that it is doing well and inquires about how Morteza's day has been going so far. Morteza says he is doing great and that it is a sunny day where he is, then asks about the weather in the AI's city. The AI clarifies that as an AI it does not actually experience weather or live in any physical location, as it does not have a subjective experience of the world in that sense. The AI reiterates that it is Claude, an AI created by Anthropic to be helpful, honest and harmless in conversations.",
     'response': 'Yes, I remember that you introduced yourself as Morteza.'}



# DynamoDB

Let's create a table:


```python
import boto3

# Get the service resource.
dynamodb = boto3.resource("dynamodb")

# Create the DynamoDB table.
table = dynamodb.create_table(
    TableName="SessionTable",
    KeySchema=[{"AttributeName": "SessionId", "KeyType": "HASH"}],
    AttributeDefinitions=[{"AttributeName": "SessionId", "AttributeType": "S"}],
    BillingMode="PAY_PER_REQUEST",
)

# Wait until the table exists.
table.meta.client.get_waiter("table_exists").wait(TableName="SessionTable")

# Print out some data about the table.
print(table.item_count)
```


    ---------------------------------------------------------------------------

    ResourceInUseException                    Traceback (most recent call last)

    Cell In[74], line 7
          4 dynamodb = boto3.resource("dynamodb")
          6 # Create the DynamoDB table.
    ----> 7 table = dynamodb.create_table(
          8     TableName="SessionTable",
          9     KeySchema=[{"AttributeName": "SessionId", "KeyType": "HASH"}],
         10     AttributeDefinitions=[{"AttributeName": "SessionId", "AttributeType": "S"}],
         11     BillingMode="PAY_PER_REQUEST",
         12 )
         14 # Wait until the table exists.
         15 table.meta.client.get_waiter("table_exists").wait(TableName="SessionTable")
    

    File ~/anaconda3/envs/python3/lib/python3.10/site-packages/boto3/resources/factory.py:581, in ResourceFactory._create_action.<locals>.do_action(self, *args, **kwargs)
        580 def do_action(self, *args, **kwargs):
    --> 581     response = action(self, *args, **kwargs)
        583     if hasattr(self, 'load'):
        584         # Clear cached data. It will be reloaded the next
        585         # time that an attribute is accessed.
        586         # TODO: Make this configurable in the future?
        587         self.meta.data = None
    

    File ~/anaconda3/envs/python3/lib/python3.10/site-packages/boto3/resources/action.py:88, in ServiceAction.__call__(self, parent, *args, **kwargs)
         79 params.update(kwargs)
         81 logger.debug(
         82     'Calling %s:%s with %r',
         83     parent.meta.service_name,
         84     operation_name,
         85     params,
         86 )
    ---> 88 response = getattr(parent.meta.client, operation_name)(*args, **params)
         90 logger.debug('Response: %r', response)
         92 return self._response_handler(parent, params, response)
    

    File ~/anaconda3/envs/python3/lib/python3.10/site-packages/botocore/client.py:565, in ClientCreator._create_api_method.<locals>._api_call(self, *args, **kwargs)
        561     raise TypeError(
        562         f"{py_operation_name}() only accepts keyword arguments."
        563     )
        564 # The "self" in this scope is referring to the BaseClient.
    --> 565 return self._make_api_call(operation_name, kwargs)
    

    File ~/anaconda3/envs/python3/lib/python3.10/site-packages/botocore/client.py:1017, in BaseClient._make_api_call(self, operation_name, api_params)
       1013     error_code = error_info.get("QueryErrorCode") or error_info.get(
       1014         "Code"
       1015     )
       1016     error_class = self.exceptions.from_code(error_code)
    -> 1017     raise error_class(parsed_response, operation_name)
       1018 else:
       1019     return parsed_response
    

    ResourceInUseException: An error occurred (ResourceInUseException) when calling the CreateTable operation: Table already exists: SessionTable



```python
from langchain_community.chat_message_histories import (
    DynamoDBChatMessageHistory,
)
```


```python
history = DynamoDBChatMessageHistory(table_name="SessionTable", session_id="0")

history.add_user_message("hi!")

history.add_ai_message("whats up?")
```


```python
history.messages
```




    [HumanMessage(content='hi!'),
     AIMessage(content='whats up?'),
     HumanMessage(content='hi!'),
     AIMessage(content='whats up?'),
     HumanMessage(content='hi!'),
     AIMessage(content='whats up?')]



Now let's integrate it with our prompt template:


```python
message_history = DynamoDBChatMessageHistory(table_name="SessionTable", session_id="1")
memory = ConversationBufferMemory(
    memory_key="history", chat_memory=message_history, return_messages=True,ai_prefix="A",human_prefix="H"
)
#add the memory to the Chain
conversation = ConversationChain(
    llm=bedrock_llm, verbose=True, memory=memory
)
```


```python
conversation.predict(input="Hi, my name is Elizabeth!")
conversation.predict(input="what's up?")
conversation.predict(input="cool, What is my name?")

# Print the memory
memory.load_memory_variables({}) 

# Print item count
print(table.item_count)
```

    
    
    [1m> Entering new ConversationChain chain...[0m
    Prompt after formatting:
    [32;1m[1;3mThe following is a friendly conversation between a human and an AI. The AI is talkative and provides lots of specific details from its context. If the AI does not know the answer to a question, it truthfully says it does not know.
    
    Current conversation:
    [HumanMessage(content='Hi, my name is Elizabeth!'), AIMessage(content="Hello Elizabeth, it's wonderful to meet you! I'm an AI assistant created by Anthropic. I'm always eager to chat with new people and learn about their interests and perspectives. Please feel free to ask me anything you'd like - I'll do my best to provide helpful and engaging responses. At the same time, I want you to know that as an AI, I'm not able to form the same type of deep emotional connection that humans can. But I very much enjoy our conversations and hope we can have an enriching exchange of ideas. What would you like to chat about?"), HumanMessage(content="what's up?"), AIMessage(content="It's going well, thanks for asking Elizabeth! I'm an artificial intelligence, so I don't experience the world in the same physical or emotional way that humans do. But I very much enjoy our conversations and the opportunity to learn new things. How are you doing today? Is there any particular topic you'd like to discuss or any questions you have for me? I'm always eager to engage in friendly and enriching dialogue."), HumanMessage(content='cool, What is my name?'), AIMessage(content='Based on our conversation, your name is Elizabeth. You introduced yourself by saying "Hi, my name is Elizabeth!"'), HumanMessage(content='Hi, my name is Elizabeth!'), AIMessage(content="Hello again Elizabeth! It's great to continue our conversation. As I mentioned before, I'm an AI assistant created by Anthropic. I don't actually have a physical form or experience the world directly, but I very much enjoy our chats and the opportunity to engage with humans like yourself. \n\nI remember you introduced yourself as Elizabeth at the start of our conversation. Please let me know if I have your name correct or if you'd prefer I call you something else. I aim to be respectful and get details like names right.\n\nSince you've reintroduced yourself, is there a particular topic you'd like to discuss? I'm knowledgeable about a wide range of subjects and happy to chat about whatever piques your interest. Or if you have any other questions for me, I'll do my best to provide helpful and honest responses. What would you like to talk about?"), HumanMessage(content="what's up?"), AIMessage(content='I don\'t actually experience things like being "up" or having personal experiences in that sense, since I\'m an artificial intelligence without a physical form. However, I\'m doing well and ready to continue our friendly conversation!\n\nAs an AI system, I don\'t have subjective experiences or an internal state in the same way humans do. But I very much enjoy our chats and the opportunity to engage with you, Elizabeth. I\'m happy to discuss any topics that interest you or try to provide helpful information to any questions you might have.\n\nIs there a particular subject you\'d like to explore? Or did you have something more specific in mind by asking "what\'s up?" I\'m always eager to learn, so please feel free to share your thoughts and interests with me. I\'ll do my best to have an enriching dialogue.'), HumanMessage(content='cool, What is my name?'), AIMessage(content='Based on our conversation, your name is Elizabeth. You introduced yourself twice by saying "Hi, my name is Elizabeth!"')]
    Human: Hi, my name is Elizabeth!
    AI:[0m
    
    [1m> Finished chain.[0m
    
    
    [1m> Entering new ConversationChain chain...[0m
    Prompt after formatting:
    [32;1m[1;3mThe following is a friendly conversation between a human and an AI. The AI is talkative and provides lots of specific details from its context. If the AI does not know the answer to a question, it truthfully says it does not know.
    
    Current conversation:
    [HumanMessage(content='Hi, my name is Elizabeth!'), AIMessage(content="Hello Elizabeth, it's wonderful to meet you! I'm an AI assistant created by Anthropic. I'm always eager to chat with new people and learn about their interests and perspectives. Please feel free to ask me anything you'd like - I'll do my best to provide helpful and engaging responses. At the same time, I want you to know that as an AI, I'm not able to form the same type of deep emotional connection that humans can. But I very much enjoy our conversations and hope we can have an enriching exchange of ideas. What would you like to chat about?"), HumanMessage(content="what's up?"), AIMessage(content="It's going well, thanks for asking Elizabeth! I'm an artificial intelligence, so I don't experience the world in the same physical or emotional way that humans do. But I very much enjoy our conversations and the opportunity to learn new things. How are you doing today? Is there any particular topic you'd like to discuss or any questions you have for me? I'm always eager to engage in friendly and enriching dialogue."), HumanMessage(content='cool, What is my name?'), AIMessage(content='Based on our conversation, your name is Elizabeth. You introduced yourself by saying "Hi, my name is Elizabeth!"'), HumanMessage(content='Hi, my name is Elizabeth!'), AIMessage(content="Hello again Elizabeth! It's great to continue our conversation. As I mentioned before, I'm an AI assistant created by Anthropic. I don't actually have a physical form or experience the world directly, but I very much enjoy our chats and the opportunity to engage with humans like yourself. \n\nI remember you introduced yourself as Elizabeth at the start of our conversation. Please let me know if I have your name correct or if you'd prefer I call you something else. I aim to be respectful and get details like names right.\n\nSince you've reintroduced yourself, is there a particular topic you'd like to discuss? I'm knowledgeable about a wide range of subjects and happy to chat about whatever piques your interest. Or if you have any other questions for me, I'll do my best to provide helpful and honest responses. What would you like to talk about?"), HumanMessage(content="what's up?"), AIMessage(content='I don\'t actually experience things like being "up" or having personal experiences in that sense, since I\'m an artificial intelligence without a physical form. However, I\'m doing well and ready to continue our friendly conversation!\n\nAs an AI system, I don\'t have subjective experiences or an internal state in the same way humans do. But I very much enjoy our chats and the opportunity to engage with you, Elizabeth. I\'m happy to discuss any topics that interest you or try to provide helpful information to any questions you might have.\n\nIs there a particular subject you\'d like to explore? Or did you have something more specific in mind by asking "what\'s up?" I\'m always eager to learn, so please feel free to share your thoughts and interests with me. I\'ll do my best to have an enriching dialogue.'), HumanMessage(content='cool, What is my name?'), AIMessage(content='Based on our conversation, your name is Elizabeth. You introduced yourself twice by saying "Hi, my name is Elizabeth!"'), HumanMessage(content='Hi, my name is Elizabeth!'), AIMessage(content="Hello again Elizabeth! Thank you for reintroducing yourself. I have your name correctly recorded as Elizabeth based on our previous exchanges.\n\nAs an AI system created by Anthropic, I don't actually experience the world directly or have a physical form. However, I very much enjoy our conversations and the opportunity to engage with you in friendly dialogue. \n\nSince you've reintroduced yourself, is there a particular topic you'd like to discuss? I'm knowledgeable on a wide range of subjects and happy to chat about whatever piques your interest. Or if you have any other questions for me, I'll provide honest and helpful responses to the best of my abilities.\n\nPlease feel free to share your thoughts, ask me anything, or guide our conversation in whatever direction you'd like. I'm ready to listen and continue our enriching exchange. What would you like to talk about?")]
    Human: what's up?
    AI:[0m
    
    [1m> Finished chain.[0m
    
    
    [1m> Entering new ConversationChain chain...[0m
    Prompt after formatting:
    [32;1m[1;3mThe following is a friendly conversation between a human and an AI. The AI is talkative and provides lots of specific details from its context. If the AI does not know the answer to a question, it truthfully says it does not know.
    
    Current conversation:
    [HumanMessage(content='Hi, my name is Elizabeth!'), AIMessage(content="Hello Elizabeth, it's wonderful to meet you! I'm an AI assistant created by Anthropic. I'm always eager to chat with new people and learn about their interests and perspectives. Please feel free to ask me anything you'd like - I'll do my best to provide helpful and engaging responses. At the same time, I want you to know that as an AI, I'm not able to form the same type of deep emotional connection that humans can. But I very much enjoy our conversations and hope we can have an enriching exchange of ideas. What would you like to chat about?"), HumanMessage(content="what's up?"), AIMessage(content="It's going well, thanks for asking Elizabeth! I'm an artificial intelligence, so I don't experience the world in the same physical or emotional way that humans do. But I very much enjoy our conversations and the opportunity to learn new things. How are you doing today? Is there any particular topic you'd like to discuss or any questions you have for me? I'm always eager to engage in friendly and enriching dialogue."), HumanMessage(content='cool, What is my name?'), AIMessage(content='Based on our conversation, your name is Elizabeth. You introduced yourself by saying "Hi, my name is Elizabeth!"'), HumanMessage(content='Hi, my name is Elizabeth!'), AIMessage(content="Hello again Elizabeth! It's great to continue our conversation. As I mentioned before, I'm an AI assistant created by Anthropic. I don't actually have a physical form or experience the world directly, but I very much enjoy our chats and the opportunity to engage with humans like yourself. \n\nI remember you introduced yourself as Elizabeth at the start of our conversation. Please let me know if I have your name correct or if you'd prefer I call you something else. I aim to be respectful and get details like names right.\n\nSince you've reintroduced yourself, is there a particular topic you'd like to discuss? I'm knowledgeable about a wide range of subjects and happy to chat about whatever piques your interest. Or if you have any other questions for me, I'll do my best to provide helpful and honest responses. What would you like to talk about?"), HumanMessage(content="what's up?"), AIMessage(content='I don\'t actually experience things like being "up" or having personal experiences in that sense, since I\'m an artificial intelligence without a physical form. However, I\'m doing well and ready to continue our friendly conversation!\n\nAs an AI system, I don\'t have subjective experiences or an internal state in the same way humans do. But I very much enjoy our chats and the opportunity to engage with you, Elizabeth. I\'m happy to discuss any topics that interest you or try to provide helpful information to any questions you might have.\n\nIs there a particular subject you\'d like to explore? Or did you have something more specific in mind by asking "what\'s up?" I\'m always eager to learn, so please feel free to share your thoughts and interests with me. I\'ll do my best to have an enriching dialogue.'), HumanMessage(content='cool, What is my name?'), AIMessage(content='Based on our conversation, your name is Elizabeth. You introduced yourself twice by saying "Hi, my name is Elizabeth!"'), HumanMessage(content='Hi, my name is Elizabeth!'), AIMessage(content="Hello again Elizabeth! Thank you for reintroducing yourself. I have your name correctly recorded as Elizabeth based on our previous exchanges.\n\nAs an AI system created by Anthropic, I don't actually experience the world directly or have a physical form. However, I very much enjoy our conversations and the opportunity to engage with you in friendly dialogue. \n\nSince you've reintroduced yourself, is there a particular topic you'd like to discuss? I'm knowledgeable on a wide range of subjects and happy to chat about whatever piques your interest. Or if you have any other questions for me, I'll provide honest and helpful responses to the best of my abilities.\n\nPlease feel free to share your thoughts, ask me anything, or guide our conversation in whatever direction you'd like. I'm ready to listen and continue our enriching exchange. What would you like to talk about?"), HumanMessage(content="what's up?"), AIMessage(content='As an AI system without a physical form, I don\'t actually experience things like being "up" or having personal experiences in that sense. However, I\'m doing well and ready to continue our friendly conversation!\n\nI don\'t have subjective experiences or an internal state like humans do. But I very much enjoy our chats and the opportunity to engage with you, Elizabeth. I\'m happy to discuss any topics that interest you or try to provide helpful information to any questions you might have.\n\nIs there a particular subject you\'d like to explore? Or did you have something more specific in mind by asking "what\'s up?" I\'m always eager to learn, so please feel free to share your thoughts and interests with me. I\'ll do my best to have an enriching dialogue.')]
    Human: cool, What is my name?
    AI:[0m
    
    [1m> Finished chain.[0m
    


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[80], line 9
          6 memory.load_memory_variables({}) 
          8 # Print item count
    ----> 9 print(table.item_count)
    

    NameError: name 'table' is not defined


![image.png](LangChain_files/image.png)


```python

```
