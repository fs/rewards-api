# Rewards API

This is API based on http://jsonapi.org to interact with Rewards appliaction as Bot.
Please checkout [complete list of endpoints for V1](v1/index.markdown).

You can play with Staging Rewards instance at http://rewards-staging.flts.tk

## Authentication

To perform API call JWT token should be provided via `Authorization` header. 
Token could be created using [`/api/v1/bot/tokens`](v1/bot_tokens/create_bot_token.markdown) endpoint.

Test bot created with these credentials:
* name: `birthday`
* password: `123456`

## Examples

In examples bellow [httpie](https://httpie.org/) tool used, please make sure you have it installed.

Get JWT token:
```
echo '{"data":{"attributes":{"name":"birthday","password":"123456"}}}' \
  | http -v http://rewards-staging.flts.tk/api/v1/bot/tokens 
```

Get list of users
```
http -v http://rewards-staging.flts.tk/api/v1/bot/users \
  "Authorization:Bearer <JWT_TOKEN>"
```

Create Birthday Bonus:
```
echo '{"data":{"attributes":{"text":"Testing bots +100 @ramil.gabdrakhmanov #be-curious-never-stop-learning"}}}' \
  | http -v http://rewards-staging.flts.tk/api/v1/bot/bonuses \
  "Authorization:Bearer <JWT_TOKEN>"
```
