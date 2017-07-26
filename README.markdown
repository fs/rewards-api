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
