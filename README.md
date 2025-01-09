# The Twitch Helix API 

## The Swagger/OpenApi REST Client Files

TwitchSwagger.yaml can be opened in https://editor.swagger.io/, for example:
https://app.swaggerhub.com/apis/Katzen48/TwitchAPI/Helix

I've converted it to a Postman Collection for you, eg:

    npm install openapi-to-postmanv2 

    npx openapi-to-postmanv2 -s TwitchSwagger.yaml -o TwitchPostmanCollection.json -p


Also to get you started I've added a **GetAccessToken** request and all you need is your Twitch Client_Id and Client_Secret.