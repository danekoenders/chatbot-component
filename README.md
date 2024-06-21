# chatbot-component (Vanilla JS)
This is an open source chatbot component that has most of the basic features a chatbot window needs.
Licensed under the MIT License.

## Features
- Chat Toggle
- Prompt email to start a chat (and receive a token in cookies)
- Send messages to backend route
- Retrieve different types of replies
- Updates buttons states on scenarios
- Fetch transcript on tab (page) switch/reload

## Requirements
- A backend application running the chatbot's logic. (Saving chatSessions with transcripts, providing answers on input and serve initial chatbot data if applicable.)
- A place to host this static js file.

## Steps to complete setup
1. First you will need to change all "your-app-domain" URI's to your actual backend app domain.
2. Serve data the chatbot needs to become personalized (only if you want it to be ofcourse). The structure is listed below*
3. Change the name of the chatbot (Right now it is Bibi) if you'd like.

#### *Data structure: **const chatbotData**
```
response = {
        customName: chatbot.customName,
        primaryColor: chatbot.primaryColor,
        secondaryColor: chatbot.secondaryColor,
        shop: {
          customName: chatbot.shop.customName,
        },
        transcript: chatSession.transcript,
      };
```
