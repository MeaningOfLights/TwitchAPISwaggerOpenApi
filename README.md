# The Twitch Helix API 

## The Swagger/OpenApi REST Client Files

TwitchSwagger.yaml can be opened in https://editor.swagger.io/, for example:
https://app.swaggerhub.com/apis/Katzen48/TwitchAPI/Helix

I've converted it to a Postman Collection for you, eg:

    npm install openapi-to-postmanv2 

    npx openapi-to-postmanv2 -s TwitchSwagger.yaml -o TwitchPostmanCollection.json -p


## Getting started

Also to get you started I've added a **GetAccessToken** request and all you need is your Twitch Client_Id and Client_Secret.

## Issue

Twitch have changed the **client_id** to **client-id** for the https://api.twitch.tv/helix endpoint, it remains client_id for the auth endpoint https://id.twitch.tv/oauth2/token

You will see this error if you haven't changed it to client-id:

{
    "error": "Unauthorized",
    "status": 401,
    "message": "Client ID is missing"
}

I changed it in the TwitchSwagger.yaml after I converted it to Postman. You can convert it again or change it manually when you hit the issue.