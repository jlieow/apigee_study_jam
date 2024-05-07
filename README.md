# Apigee API Study Jam

This is the supporting material for a one-day hands-on workshop that introduces developers to Apigee. We call it a "**Apigee API Study Jam**".

All of the material here is released under the [Apache 2.0 License](./LICENSE)

### Agenda

-   A brief presentation : 15 mins
-   Product Demo : 35 mins

### [Core Labs](./Labs/Core)

1. [API Development - Create a Reverse Proxy with an HTTP Target](./Labs/Core/01-Create-a-Reverse-Proxy)
2. [API Development - Create a Reverse Proxy with a Nodejs Target](./Labs/Core/02-Proxy-with-Nodejs-Target)
3. [API Diagnostics - Trace tool ](./Labs/Core/03-Trace-tool)
4. [API Security - Securing APIs with API Keys ](./Labs/Core/04-Securing-APIs-with-API-Keys)
5. [API Security - Securing APIs with OAuth client credentials](./Labs/Core/05-Securing-APIs-with-OAuth-client-creds)
6. [API Security - Securing APIs with OAuth 3-legged](./Labs/Core/06-Securing-APIs-with-OAuth-3-legged)
7. [OpenID Connect Signin ](./Labs/Core/07-OpenID-Connect-Signin)
8. [Traffic Management - Rate Limit APIs ](./Labs/Core/08-Rate-Limit-APIs)
9. [Transformation - HTTP header injection ](./Labs/Core/09-HTTP-header-injection)
10. [API Development - Composite APIs ](./Labs/Core/10-Composite-APIs)
11. [JWT Verification ](./Labs/Core/11-JWT-Verification)

### [Appendix Labs](./Labs/Appendix)

There is no natural order to these additional exercises.

-   [API Analytics - Custom Reports](./Labs/Appendix/API%20Analytics%20-%20Custom%20Reports)
-   [API Design - Create a Reverse Proxy with OpenAPI specification](./Labs/Appendix/API%20Design%20-%20Create%20a%20Reverse%20Proxy%20with%20OpenAPI%20specification)
-   [API Development - Create a RESTful API from a SOAP service](./Labs/Appendix/API%20Development%20-%20Create%20a%20RESTful%20API%20from%20a%20SOAP%20service)
-   [API Performance - Caching](./Labs/Appendix/API%20Performance%20-%20Caching)
-   [API Publishing - Developer Portal Customization](./Labs/Appendix/API%20Publishing%20-%20Developer%20Portal%20Customization)
-   [API Publishing - Documentation](./Labs/Appendix/API%20Publishing%20-%20Documentation)
-   [API Security - Securing APIs with OAuth password grant](./Labs/Appendix/API%20Security%20-%20Securing%20APIs%20with%20OAuth%20password%20grant)
-   [API Security - Threat Protection](./Labs/Appendix/API%20Security%20-%20Threat%20Protection)
-   [API-Publishing---Packaging-APIs](./Labs/Appendix/API-Publishing---Packaging-APIs)
-   [Consume APIs](./Labs/Appendix/Consume%20APIs)
-   [Hybrid Deployment - Edge Microgateway](./Labs/Appendix/Hybrid%20Deployment%20-%20Edge%20Microgateway)
-   [Traffic Management - Throttle APIs](./Labs/Appendix/Traffic%20Management%20-%20Throttle%20APIs)

endpoint=https://prod-api.jeromelieow.com/oauth2-cc/token
curl -i -X POST \
 -H 'content-type: application/x-www-form-urlencoded' \
 -H 'Authorization: Basic bzBYd1Vic3Z6U1JrWUx0VWlIdGxQQmMwRzlDcHZ3YXZZdU9YdEdHcVpwTEFKaDV1OnJ2OHBkT0NGbmhXUHE2ZWQwOUlHcG5HcTFadUR4WXVNWmxSTmI3bm1xZ0NhQU80TkFzaXk4cHBhNHhySHRDQUQ=' \
 "$endpoint/oauth2-cc/token" \
 -d 'grant_type=client_credentials'

curl --location --request POST 'https://prod-api.jeromelieow.com/oauth2-cc/token' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Authorization: Basic bzBYd1Vic3Z6U1JrWUx0VWlIdGxQQmMwRzlDcHZ3YXZZdU9YdEdHcVpwTEFKaDV1OnJ2OHBkT0NGbmhXUHE2ZWQwOUlHcG5HcTFadUR4WXVNWmxSTmI3bm1xZ0NhQU80TkFzaXk4cHBhNHhySHRDQUQ=' \
-d 'grant_type=client_credentials'
