---
description: ApiCredential schema from Adyen API
layout: schema
name: ApiCredential
properties_list:
- description: References to resources linked to the API credential.
  name: _links
  type: object
- description: Indicates if the API credential is enabled. Must be set to **true** to use the credential in your integration.
  name: active
  type: boolean
- description: List of IP addresses from which your client can make requests. If the list is empty, we allow requests from any IP. If the list is not empty and we get a request from an IP which is not on the list, y
  name: allowedIpAddresses
  type: array
- description: List containing the [allowed origins](https://docs.adyen.com/development-resources/client-side-authentication#allowed-origins) linked to the API credential.
  name: allowedOrigins
  type: array
- description: Public key used for [client-side authentication](https://docs.adyen.com/development-resources/client-side-authentication). The client key is required for Drop-in and Components integrations.
  name: clientKey
  type: string
- description: Description of the API credential.
  name: description
  type: string
- description: Unique identifier of the API credential.
  name: id
  type: string
- description: List of [roles](https://docs.adyen.com/development-resources/api-credentials#roles-1) for the API credential.
  name: roles
  type: array
- description: The name of the [API credential](https://docs.adyen.com/development-resources/api-credentials), for example **ws@Company.TestCompany**.
  name: username
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-api-credential-schema.json
slug: management-api-credential
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-api-credential-schema.json\",\n  \"title\": \"ApiCredential\",\n  \"description\": \"ApiCredential schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_links\": {\n      \"description\": \"References to resources linked to the API credential.\",\n      \"$ref\": \"#/components/schemas/ApiCredentialLinks\"\n    },\n    \"active\": {\n      \"description\": \"Indicates if the API credential is enabled. Must be set to **true** to use the credential in your integration.\",\n      \"type\": \"boolean\"\n    },\n    \"allowedIpAddresses\": {\n      \"description\": \"List of IP addresses from which your client can make requests.\\n\\nIf the list is empty, we allow requests from any IP.\\nIf the list is not empty and we get a request from an IP which is not on the list, you get a security\
  \ error.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"allowedOrigins\": {\n      \"description\": \"List containing the [allowed origins](https://docs.adyen.com/development-resources/client-side-authentication#allowed-origins) linked to the API credential.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AllowedOrigin\"\n      },\n      \"type\": \"array\"\n    },\n    \"clientKey\": {\n      \"description\": \"Public key used for [client-side authentication](https://docs.adyen.com/development-resources/client-side-authentication). The client key is required for Drop-in and Components integrations.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"Description of the API credential.\",\n      \"maxLength\": 50,\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"Unique identifier of the API credential.\",\n      \"type\": \"string\"\n    },\n    \"\
  roles\": {\n      \"description\": \"List of [roles](https://docs.adyen.com/development-resources/api-credentials#roles-1) for the API credential.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"username\": {\n      \"description\": \"The name of the [API credential](https://docs.adyen.com/development-resources/api-credentials), for example **ws@Company.TestCompany**.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"username\",\n    \"clientKey\",\n    \"allowedIpAddresses\",\n    \"roles\",\n    \"active\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-api-credential-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ApiCredential
---
