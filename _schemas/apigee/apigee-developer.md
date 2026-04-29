---
description: A developer registered in an Apigee organization. Developers are consumers of APIs who register apps and obtain API keys to access API products.
layout: schema
name: Apigee Developer
properties_list:
- description: Required. Email address of the developer. Used as the unique identifier.
  name: email
  type: string
- description: Required. First name of the developer.
  name: firstName
  type: string
- description: Required. Last name of the developer.
  name: lastName
  type: string
- description: Required. User name of the developer.
  name: userName
  type: string
- description: Output only. System-generated developer ID.
  name: developerId
  type: string
- description: Output only. Name of the Apigee organization.
  name: organizationName
  type: string
- description: Status of the developer account.
  name: status
  type: string
- description: Output only. List of apps owned by the developer.
  name: apps
  type: array
- description: Custom attributes for the developer (maximum 18).
  name: attributes
  type: array
- description: Output only. Companies associated with the developer.
  name: companies
  type: array
- description: Output only. Time the developer was created in milliseconds since epoch.
  name: createdAt
  type: string
- description: Output only. Time the developer was last modified in milliseconds since epoch.
  name: lastModifiedAt
  type: string
- description: Access type of the developer.
  name: accessType
  type: string
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-developer-schema.json
slug: apigee-developer
source_filename: apigee-developer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/apigee/apigee-developer-schema.json\",\n  \"title\": \"Apigee Developer\",\n  \"description\": \"A developer registered in an Apigee organization. Developers are consumers of APIs who register apps and obtain API keys to access API products.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Required. Email address of the developer. Used as the unique identifier.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"Required. First name of the developer.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Required. Last name of the developer.\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"Required. User name of the developer.\"\n    },\n    \"developerId\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Output only. System-generated developer ID.\",\n      \"readOnly\": true\n    },\n    \"organizationName\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Name of the Apigee organization.\",\n      \"readOnly\": true\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the developer account.\",\n      \"enum\": [\"active\", \"inactive\"]\n    },\n    \"apps\": {\n      \"type\": \"array\",\n      \"description\": \"Output only. List of apps owned by the developer.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"attributes\": {\n      \"type\": \"array\",\n      \"description\": \"Custom attributes for the developer (maximum 18).\",\n      \"maxItems\": 18,\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"value\": { \"type\": \"string\" }\n   \
  \     },\n        \"required\": [\"name\", \"value\"]\n      }\n    },\n    \"companies\": {\n      \"type\": \"array\",\n      \"description\": \"Output only. Companies associated with the developer.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Time the developer was created in milliseconds since epoch.\",\n      \"readOnly\": true\n    },\n    \"lastModifiedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Time the developer was last modified in milliseconds since epoch.\",\n      \"readOnly\": true\n    },\n    \"accessType\": {\n      \"type\": \"string\",\n      \"description\": \"Access type of the developer.\"\n    }\n  },\n  \"required\": [\"email\", \"firstName\", \"lastName\", \"userName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/json-schema/apigee-developer-schema.json
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
title: Apigee Developer
---
