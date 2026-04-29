---
description: CreateCompanyApiCredentialRequest schema from Adyen API
layout: schema
name: CreateCompanyApiCredentialRequest
properties_list:
- description: List of [allowed origins](https://docs.adyen.com/development-resources/client-side-authentication#allowed-origins) for the new API credential.
  name: allowedOrigins
  type: array
- description: List of merchant accounts that the API credential has access to.
  name: associatedMerchantAccounts
  type: array
- description: Description of the API credential.
  name: description
  type: string
- description: List of [roles](https://docs.adyen.com/development-resources/api-credentials#roles-1) for the API credential. Only roles assigned to 'ws@Company.<CompanyName>' can be assigned to other API credentials
  name: roles
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-create-company-api-credential-request-schema.json
slug: management-create-company-api-credential-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-create-company-api-credential-request-schema.json\",\n  \"title\": \"CreateCompanyApiCredentialRequest\",\n  \"description\": \"CreateCompanyApiCredentialRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowedOrigins\": {\n      \"description\": \"List of [allowed origins](https://docs.adyen.com/development-resources/client-side-authentication#allowed-origins) for the new API credential.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"associatedMerchantAccounts\": {\n      \"description\": \"List of merchant accounts that the API credential has access to.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"description\": {\n      \"description\": \"Description\
  \ of the API credential.\",\n      \"type\": \"string\"\n    },\n    \"roles\": {\n      \"description\": \"List of [roles](https://docs.adyen.com/development-resources/api-credentials#roles-1) for the API credential. Only roles assigned to 'ws@Company.<CompanyName>' can be assigned to other API credentials.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-create-company-api-credential-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateCompanyApiCredentialRequest
---
