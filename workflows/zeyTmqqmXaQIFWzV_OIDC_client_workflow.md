# Documentation: OIDC client workflow

## Description
The "OIDC client workflow" facilitates OpenID Connect (OIDC) authentication and retrieves user information from an OIDC provider.

## Nodes
1. **Webhook**: Handles incoming requests and triggers the workflow.
2. **Code**: Parses cookies from incoming requests.
3. **user info**: Sends HTTP requests to retrieve user information from the OIDC provider.

## Web Services Involved
- **OIDC Provider**: Used for authentication and user information retrieval.
