---
description: An API managed within the APIIDA API Control Plane, representing a logical API resource that can be versioned and deployed to gateways.
layout: schema
name: APIIDA API
properties_list:
- description: Unique identifier for the API
  name: id
  type: string
- description: Display name of the API
  name: name
  type: string
- description: Human-readable description of the API
  name: description
  type: string
- description: Current lifecycle status of the API
  name: status
  type: string
- description: Tags for categorizing the API
  name: tags
  type: array
- description: The current active version identifier
  name: currentVersion
  type: string
- description: Timestamp when the API was created
  name: createdAt
  type: string
- description: Timestamp when the API was last updated
  name: updatedAt
  type: string
provider_name: APIIDA
provider_slug: apiida
schema_file: json-schema/apiida-api.json
slug: apiida-api
source_filename: apiida-api.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"apiida-api.json\",\n  \"title\": \"APIIDA API\",\n  \"description\": \"An API managed within the APIIDA API Control Plane, representing a logical API resource that can be versioned and deployed to gateways.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the API\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the API\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft\", \"published\", \"deprecated\", \"retired\"],\n      \"description\": \"Current lifecycle status of the API\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"\
  type\": \"string\"\n      },\n      \"description\": \"Tags for categorizing the API\"\n    },\n    \"currentVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The current active version identifier\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apiida/refs/heads/main/json-schema/apiida-api.json
tags:
- API Gateway
- API Management
- Federated API Management
- Governance
- Layer7
title: APIIDA API
---
