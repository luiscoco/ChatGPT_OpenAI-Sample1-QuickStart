# ChatGPT_OpenAI: QuickStart

## 1. Sign up or Log in to the OpenAI platform

In the internet browser we navigate to the OpenAI platform URL: **https://platform.openai.com/**

We press on the **Sign up** button

![image](https://github.com/luiscoco/ChatGPT_OpenAI-Sample1-QuickStart/assets/32194879/b634a849-300f-4cc0-82b8-11a6e6135e50)

We create a new account or if we already have one we log in to our account

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

