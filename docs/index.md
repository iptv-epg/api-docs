# IPTV EPG API Usage
Current version: *1.1.0*

## API Endpoint
epg.best provides a convenient REST API for external services to access the services provided by epg.best.

The API is available at `https://epg.best/api`

## JSON
The IPTV-EPG API uses JSON as the markup language for communication. 

## Authentication
The API utilizes OAuth2 for client authentication. For details, please refer to the authentication docs.

## Pagination

GET API endpoints have pagination by default. Usage in url parameters:

`{{API_URL}}?page={integer}&per_page={integer}`