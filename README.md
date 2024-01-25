# ChatGPT_OpenAI: QuickStart

## 1. Sign up or Log in to the OpenAI platform

In the internet browser we navigate to the OpenAI platform URL: **https://platform.openai.com/**

We press on the **Sign up** button

![image](https://github.com/luiscoco/ChatGPT_OpenAI-Sample1-QuickStart/assets/32194879/b634a849-300f-4cc0-82b8-11a6e6135e50)

We **create a new account** or if we already have one we **log in** to our account

![image](https://github.com/luiscoco/ChatGPT_OpenAI-Sample1-QuickStart/assets/32194879/193d0d27-0396-4fdf-8ba2-ed614d1b7f33)

## 2. Account settings (set the payment method and spend limit)

We select the **Settings->Billing** option in the left hand side menu

https://platform.openai.com/account/billing/overview

![image](https://github.com/luiscoco/ChatGPT_OpenAI-Sample1-QuickStart/assets/32194879/a7b275e9-14f9-4fb3-a1d1-b284bc3dae67)

We have to enter the **Payment method**

https://platform.openai.com/account/billing/payment-methods

![image](https://github.com/luiscoco/ChatGPT_OpenAI-Sample1-QuickStart/assets/32194879/ef9128b8-c110-4648-8e92-b36175b43df0)

We input all the info required in the payment method form

![image](https://github.com/luiscoco/ChatGPT_OpenAI-Sample1-QuickStart/assets/32194879/98830a0f-0148-483f-acc9-51c35beb405b)

We can set an initial ammout of 12 euros per month

https://platform.openai.com/account/limits

![image](https://github.com/luiscoco/ChatGPT_OpenAI-Sample1-QuickStart/assets/32194879/d1418bb6-2e7a-41c9-a745-1b898fa90380)

## 3. Create API Key

We have to create an API Key in order to authorize when we send the API request

![image](https://github.com/luiscoco/ChatGPT_OpenAI-Sample1-QuickStart/assets/32194879/ac69918b-d490-4e67-8486-7f36a8a66a5b)

We copy and store the API Key value, we will need to introduce this value in the API header to authorize the service

## 4. OpenAI endpoints

We select the menu option Documentation or we navigate to this URL: **https://platform.openai.com/docs**

Inside the Documentation we have two options: **Documentation** or **API Reference**

https://platform.openai.com/docs/overview

https://platform.openai.com/docs/api-reference

We select the **API Reference** option and in the **ENDPOINTS** section we can see all the available OpenAI endpoints

We can start retriving the model list with this request: **GET https://api.openai.com/v1/models**

![image](https://github.com/luiscoco/ChatGPT_OpenAI-Sample1-QuickStart/assets/32194879/6a202d98-4273-4223-a31d-221e9df632e2)

We are going to user **Postman** for sending the API request

We run **Postman** and we enter in the **Bearer Token** the **OpenAI API Key**

![image](https://github.com/luiscoco/ChatGPT_OpenAI-Sample1-QuickStart/assets/32194879/429e6b92-d45d-4536-8bfa-9ca2f6c57e3f)

We input the **GET** request, in the **Body** we select **none**, and we press the **Send** button

![image](https://github.com/luiscoco/ChatGPT_OpenAI-Sample1-QuickStart/assets/32194879/54315ff8-bfda-4a2b-968e-e99a535fa646)

This is the **response** we receive

![image](https://github.com/luiscoco/ChatGPT_OpenAI-Sample1-QuickStart/assets/32194879/a9a3f3b1-3875-47c5-adb6-fa1acd962b13)

```json
{
    "object": "list",
    "data": [
        {
            "id": "gpt-3.5-turbo-1106",
            "object": "model",
            "created": 1698959748,
            "owned_by": "system"
        },
        {
            "id": "dall-e-3",
            "object": "model",
            "created": 1698785189,
            "owned_by": "system"
        },
        {
            "id": "whisper-1",
            "object": "model",
            "created": 1677532384,
            "owned_by": "openai-internal"
        },
        {
            "id": "dall-e-2",
            "object": "model",
            "created": 1698798177,
            "owned_by": "system"
        },
        {
            "id": "gpt-3.5-turbo-16k",
            "object": "model",
            "created": 1683758102,
            "owned_by": "openai-internal"
        },
        {
            "id": "text-embedding-ada-002",
            "object": "model",
            "created": 1671217299,
            "owned_by": "openai-internal"
        },
        {
            "id": "tts-1-hd-1106",
            "object": "model",
            "created": 1699053533,
            "owned_by": "system"
        },
        {
            "id": "tts-1-hd",
            "object": "model",
            "created": 1699046015,
            "owned_by": "system"
        },
        {
            "id": "gpt-3.5-turbo-instruct",
            "object": "model",
            "created": 1692901427,
            "owned_by": "system"
        },
        {
            "id": "davinci-002",
            "object": "model",
            "created": 1692634301,
            "owned_by": "system"
        },
        {
            "id": "babbage-002",
            "object": "model",
            "created": 1692634615,
            "owned_by": "system"
        },
        {
            "id": "gpt-4-0613",
            "object": "model",
            "created": 1686588896,
            "owned_by": "openai"
        },
        {
            "id": "gpt-3.5-turbo-16k-0613",
            "object": "model",
            "created": 1685474247,
            "owned_by": "openai"
        },
        {
            "id": "gpt-4-1106-preview",
            "object": "model",
            "created": 1698957206,
            "owned_by": "system"
        },
        {
            "id": "gpt-4",
            "object": "model",
            "created": 1687882411,
            "owned_by": "openai"
        },
        {
            "id": "gpt-4-vision-preview",
            "object": "model",
            "created": 1698894917,
            "owned_by": "system"
        },
        {
            "id": "tts-1-1106",
            "object": "model",
            "created": 1699053241,
            "owned_by": "system"
        },
        {
            "id": "tts-1",
            "object": "model",
            "created": 1681940951,
            "owned_by": "openai-internal"
        },
        {
            "id": "gpt-3.5-turbo-instruct-0914",
            "object": "model",
            "created": 1694122472,
            "owned_by": "system"
        },
        {
            "id": "gpt-3.5-turbo",
            "object": "model",
            "created": 1677610602,
            "owned_by": "openai"
        },
        {
            "id": "gpt-3.5-turbo-0301",
            "object": "model",
            "created": 1677649963,
            "owned_by": "openai"
        },
        {
            "id": "gpt-3.5-turbo-0613",
            "object": "model",
            "created": 1686587434,
            "owned_by": "openai"
        }
    ]
}
```

This is a brief explanation about all the OpenAI models:

**GPT (Generative Pre-trained Transformer) Models**

**GPT-3.5 Turbo** (Various Versions): These models are variations of GPT-3.5, optimized for faster responses and potentially tailored for specific applications or performance metrics. The "turbo" naming suggests enhanced performance, and the different versions (e.g., "1106", "16k", "instruct", etc.) could indicate updates, capacity (like token limits), or specialized training directives.

**GPT-4** (and Variants): GPT-4 represents an advancement over GPT-3.5, with improvements in understanding context, generating more accurate and nuanced text, and possibly handling more complex instructions. Variants like "GPT-4-0613" and "GPT-4-1106-preview" might refer to specific updates or experimental versions designed for testing new capabilities.

**DALL·E Models**

**DALL·E 2 and DALL·E 3**: These models specialize in generating images from textual descriptions. DALL·E 2 was a significant advancement in creating highly realistic and detailed images from text prompts. DALL·E 3, presumably, further enhances these capabilities, offering improvements in image quality, creativity, or the ability to understand more complex prompts.

**Whisper Model**

**Whisper-1**: OpenAI's Whisper model is designed for speech-to-text tasks, converting audio into written text. It's known for its robustness across different languages and accents, as well as its ability to handle noisy environments.

**Text Embedding Models**

**Text-Embedding-Ada-002:** This model is used for generating text embeddings, which are numerical representations of text that capture its semantic meaning. Such models are useful for a range of applications, including semantic search, content analysis, and more sophisticated natural language understanding tasks.

**TTS (Text-to-Speech) Models**

**TTS-1, TTS-1-HD, and Variants:** These models convert text into speech. The "HD" designation might indicate high-definition audio quality. Variants like "TTS-1-1106" could refer to specific versions with improvements in voice realism, emotional expressiveness, or support for multiple languages.

**Other Named Models**

**Davinci-002, Babbage-002:** These names align with OpenAI's convention for different versions of their language models, with Davinci being the most capable and Babbage offering a balance between performance and computational efficiency. The "002" suffix likely indicates specific iterations within these model families.

## 5. Samples with Postman

### 5.1. Chat Completion (Conversational Responses)

Endpoint: https://api.openai.com/v1/chat/completions

Method: POST

Headers:

Authorization: Bearer YOUR_API_KEY

Content-Type: application/json

Body:

```json
{
  "model": "gpt-4",
  "messages": [
    {"role": "user", "content": "What are the major differences between Python 2 and Python 3?"}
  ]
}
```

This request initiates a conversational exchange, suitable for building chatbots or interactive conversational agents.

### 5.2. Text Completion (Generating Text)

Endpoint: https://api.openai.com/v1/completions

Method: POST

Headers:

Authorization: Bearer YOUR_API_KEY

Content-Type: application/json

Body:

```json
{
  "model": "text-davinci-004",
  "prompt": "Write a short story about a robot learning to paint:",
  "temperature": 0.7,
  "max_tokens": 150,
  "top_p": 1,
  "frequency_penalty": 0,
  "presence_penalty": 0
}
```

This request is for generating creative text, such as stories, based on a prompt. You can adjust parameters like temperature and max_tokens to control creativity and length.

### 5.3. Editing (Improving Text)

Endpoint: https://api.openai.com/v1/edits

Method: POST

Headers:

Authorization: Bearer YOUR_API_KEY

Content-Type: application/json

Body:

```json
{
  "model": "text-davinci-edit-001",
  "input": "She no went to the market.",
  "instruction": "Fix grammatical mistakes"
}
```

This request is useful for refining or altering text based on specific instructions, such as correcting grammar or changing the style.

### 5.4. Embeddings (Generating Textual Representations)

Endpoint: https://api.openai.com/v1/embeddings

Method: POST

Headers:

Authorization: Bearer YOUR_API_KEY

Content-Type: application/json

Body:

```json
{
  "model": "text-similarity-davinci-001",
  "input": ["Puppies are adorable.", "Kittens are cute."]
}
```

This request generates embeddings for texts, which can be used for semantic text similarity, clustering, or search applications.
