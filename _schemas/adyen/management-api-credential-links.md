---
description: ApiCredentialLinks schema from Adyen API
layout: schema
name: ApiCredentialLinks
properties_list:
- description: List of allowed origins.
  name: allowedOrigins
  type: object
- description: Company account that the API credential is linked to. Only present for company-level webhooks.
  name: company
  type: object
- description: Generates a new API key. When you generate a new one, the existing key remains valid for 24 hours.
  name: generateApiKey
  type: object
- description: Generates a new client key, used to authenticate client-side requests. When you generate a new one, the existing key remains valid for 24 hours.
  name: generateClientKey
  type: object
- description: The merchant account that the API credential is linked to. Only present for merchant-level API credentials.
  name: merchant
  type: object
- description: Link to the resource itself.
  name: self
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-api-credential-links-schema.json
slug: management-api-credential-links
source_filename: management-api-credential-links-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-api-credential-links-schema.json\",\n  \"title\": \"ApiCredentialLinks\",\n  \"description\": \"ApiCredentialLinks schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowedOrigins\": {\n      \"description\": \"List of allowed origins.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"company\": {\n      \"description\": \"Company account that the API credential is linked to. Only present for company-level webhooks.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"generateApiKey\": {\n      \"description\": \"Generates a new API key. When you generate a new one, the existing key remains valid for 24 hours. \",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"generateClientKey\": {\n      \"description\": \"\
  Generates a new client key, used to authenticate client-side requests. When you generate a new one, the existing key remains valid for 24 hours.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"merchant\": {\n      \"description\": \"The merchant account that the API credential is linked to. Only present for merchant-level API credentials.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"self\": {\n      \"description\": \"Link to the resource itself.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    }\n  },\n  \"required\": [\n    \"self\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-api-credential-links-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ApiCredentialLinks
---
