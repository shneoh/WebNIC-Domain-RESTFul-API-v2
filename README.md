# WebNIC Domain RESTFul API version 2.
This is the API collecitons that ease the testing and development tasks for fellow partners.

Do take note there are two seperated environments (PROD and OTE), which only supported API Credential from respective envionment.

You can manage the API credentials in WebNIC Portal, Resource Access Management, API Management.

## Preparations
1. Download and install POSTMAN.
2. Download the POSTMAN Collection JSON file from here.
3. Acquire an API Credential Set from WebNIC Portal.
4. Whitelist your source IP Address.

## Setup in POSTMAN
1. Import the downloaded POSTMAN Collection JSON file to your POSTMAN.
2. Create a new Environment set with the following params:
   - `baseUrl` : URL to API endpoint.
   - `token_endpoint` : URL to request JWT token.
   - `client_id` : API Key.
   - `client_secret` : API Secret.
3. Please check with your account manager for the endpoints value.

   
