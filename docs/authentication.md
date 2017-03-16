# Authentication

The IPTV-EPG API utilizes OAuth2 for user authentication. Currently, only private access tokens are supported.
These are commonly reffered to as 'Api keys'. A user can create and delete as many tokens as necessary.

## Creating an API Key
To create an access token, go to https://www.iptv-epg.com/account/api. You can create as many tokens as necessary.
The API keys are shown only once, upon creation. If you lose it, you need to delete it and create another one. 
All keys are valid for one year.

## Authenticating an API request
To authenticate the user in an API request, pass the API key in the request header as follows:

`Authorization: Bearer <API KEY>`˙

## Unsucessful authentication
Upon authentication failure, the API responds with an `HTTP 401 - Unauthorized` status.