---
description: A developer app registered in Apigee. Apps are associated with developers and contain API keys (credentials) that provide access to API products.
layout: schema
name: Apigee Developer App
properties_list:
- description: Name of the developer app.
  name: name
  type: string
- description: Output only. ID of the developer app.
  name: appId
  type: string
- description: Output only. Developer ID of the owning developer.
  name: developerId
  type: string
- description: List of API products associated with the app.
  name: apiProducts
  type: array
- description: Custom attributes for the developer app.
  name: attributes
  type: array
- description: Callback URL used by OAuth 2.0 authorization servers.
  name: callbackUrl
  type: string
- description: Output only. Credentials (API keys) for the app.
  name: credentials
  type: array
- description: Status of the developer app.
  name: status
  type: string
- description: OAuth scopes associated with the app.
  name: scopes
  type: array
- description: Output only. Time the app was created in milliseconds since epoch.
  name: createdAt
  type: string
- description: Output only. Time the app was last modified.
  name: lastModifiedAt
  type: string
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-developer-app-schema.json
slug: apigee-developer-app
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/apigee/apigee-developer-app-schema.json\",\n  \"title\": \"Apigee Developer App\",\n  \"description\": \"A developer app registered in Apigee. Apps are associated with developers and contain API keys (credentials) that provide access to API products.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the developer app.\"\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. ID of the developer app.\",\n      \"readOnly\": true\n    },\n    \"developerId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Developer ID of the owning developer.\",\n      \"readOnly\": true\n    },\n    \"apiProducts\": {\n      \"type\": \"array\",\n      \"description\": \"List of API products associated with the app.\",\n      \"items\": {\n        \"type\"\
  : \"string\"\n      }\n    },\n    \"attributes\": {\n      \"type\": \"array\",\n      \"description\": \"Custom attributes for the developer app.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"value\": { \"type\": \"string\" }\n        },\n        \"required\": [\"name\", \"value\"]\n      }\n    },\n    \"callbackUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Callback URL used by OAuth 2.0 authorization servers.\"\n    },\n    \"credentials\": {\n      \"type\": \"array\",\n      \"description\": \"Output only. Credentials (API keys) for the app.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/DeveloperAppKey\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the developer app.\",\n      \"enum\": [\"approved\", \"revoked\"]\n    },\n    \"scopes\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"OAuth scopes associated with the app.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Time the app was created in milliseconds since epoch.\",\n      \"readOnly\": true\n    },\n    \"lastModifiedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Time the app was last modified.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"name\"],\n  \"$defs\": {\n    \"DeveloperAppKey\": {\n      \"type\": \"object\",\n      \"description\": \"Consumer key and secret for a developer app.\",\n      \"properties\": {\n        \"consumerKey\": {\n          \"type\": \"string\",\n          \"description\": \"Consumer key (API key) for the developer app.\"\n        },\n        \"consumerSecret\": {\n          \"type\": \"string\",\n          \"description\": \"Consumer secret for the developer app.\"\n        },\n  \
  \      \"apiProducts\": {\n          \"type\": \"array\",\n          \"description\": \"API products associated with this key.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"apiproduct\": { \"type\": \"string\" },\n              \"status\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Status of the credential.\",\n          \"enum\": [\"approved\", \"revoked\"]\n        },\n        \"expiresAt\": {\n          \"type\": \"string\",\n          \"description\": \"Time the key expires in milliseconds since epoch.\"\n        },\n        \"issuedAt\": {\n          \"type\": \"string\",\n          \"description\": \"Output only. Time the key was issued.\",\n          \"readOnly\": true\n        },\n        \"scopes\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        }\n      }\n    }\n\
  \  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/json-schema/apigee-developer-app-schema.json
tags:
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Hybrid
- Integrations
- Microservices
- Monetization
title: Apigee Developer App
---
