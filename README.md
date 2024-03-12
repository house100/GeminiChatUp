
# Gemini ChatUp

[中文](./README.zh.md)

## About
This project is a chat application based on the Google GeminiPro API Key, with support for responsive layout. It can retain multiple sets of conversations, and the basic parameters for each set of conversations can be set separately.

## How to Use
[Demo](https://chatup.moca.one) 
>You need to log in with an account or provide your own Gemini Pro API Key.<br />
>Developers can click to see how to [deploy this feature](#user_credential).

#### Account/Password
|Test Account|Password|
|--|--|
|guest|guest123456|
<br />

#### Streaming Conversation
<img width="400" alt="SCR-20240121-shmh" src="https://github.com/loo-y/GeminiChatUp/assets/2792566/4f91a1b7-2773-4a5a-93a0-1fa294d17174">
<br />
<br />


## How to Deploy
### Get Gemini API Key

[Get API Key](https://makersuite.google.com/app/apikey)

### Deploy to Vercel
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Floo-y%2FGeminiChatUp&env=GOOGLE_GEMINI_API_KEY&envDescription=GeminiPro%20API%20Key&project-name=geminichatup&repository-name=GeminiChatUp&demo-url=https%3A%2F%2Fchatup.moca.one&demo-image=https%3A%2F%2Fgithub.com%2Floo-y%2FGeminiChatUp%2Fassets%2F2792566%2Fa69a57a5-598e-4958-a912-a7cc37dba2aa)

Click the button to deploy to Vercel and follow the prompts to enter your Google GeminiPro API Key. 

<a id="user_credential"></a>
### Adding User Authentication
This feature requires enabling Edge config in Vercel. Follow these steps:
1. After the project is deployed, switch to the Storage Tab and select "New Edge Config."
<br /><img width="800" alt="SCR-20240120-pofd" src="https://github.com/loo-y/GeminiChatUp/assets/2792566/96ff748d-8d3e-4b67-9a41-58e5d5ad022e">

2. In the Edge Config, switch to Projects and check if it is already associated with the current project.
<br /><img width="800" alt="SCR-20240120-pmob" src="https://github.com/loo-y/GeminiChatUp/assets/2792566/71151560-37d2-4069-a8d9-bc8ec2538b64">

3. Finally, switch to Items and at the bottom right, you can add usernames and passwords in JSON format by yourself.
<br /><img width="800" alt="SCR-20240120-pmyd" src="https://github.com/loo-y/GeminiChatUp/assets/2792566/99880c3a-b5dd-482d-a50c-6118921aa4d6">

<br />

### Local Start
1. Install dependencies
    ```
    npm i
    ```

2. Create a new ```.env```file,  copy the contents of ```.env.example``` into ```.env```, and modify it with your own API Key and configuration options.
<br />

3. Local Start
    ```javascript
    npm run dev
    ```

## Screenshots
<br />
<img width="300" src="https://github.com/loo-y/GeminiChatUp/assets/2792566/6924b5fe-f30a-4f9d-a69f-27a6fe2820a1" />  
<img width="300" src="https://github.com/loo-y/GeminiChatUp/assets/2792566/630b5181-bbdd-4dd0-bac5-9376b3f50d63" />
<br />
<br /><img width="800" alt="SCR-20240104-mgmn" src="https://github.com/loo-y/GeminiChatUp/assets/2792566/cf8c68ed-dded-483e-b69e-f19e022726b6" /><br />

<!-- <br /><img width="800" alt="SCR-20240104-mgju" src="https://github.com/loo-y/GeminiChatUp/assets/2792566/cdfd758f-eb8e-4165-9047-85124188dfce" /><br />
<br /><img width="800" alt="SCR-20240112-bylz" src="https://github.com/loo-y/GeminiChatUp/assets/2792566/a69a57a5-598e-4958-a912-a7cc37dba2aa" /><br /> 
-->

### To Be Completed

1. ~~Streaming Q&A~~ (completed)
2. ~~Clearing previous conversations~~ (completed)
3. ~~Calculating tokens and removing excess conversations~~ (completed)
4. ~~Global settings, supporting client integration with GeminiPro API~~ (completed)
5. Support for searching conversation content
6. ~~Add GeminiPro Vision API~~ (completed)
