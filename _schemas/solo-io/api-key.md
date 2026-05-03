---
description: An API key used to authenticate requests to API products exposed through the Gloo developer portal.
layout: schema
name: Solo.io Gloo Portal API Key
properties_list:
- description: Unique identifier for the API key.
  name: id
  type: string
- description: Name or label for the API key.
  name: name
  type: string
- description: ID of the API product this key grants access to.
  name: apiProductId
  type: string
- description: ID of the usage plan associated with this key.
  name: usagePlanId
  type: string
- description: Timestamp when the API key was created.
  name: createdAt
  type: string
- description: Additional metadata associated with the API key.
  name: metadata
  type: object
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/api-key.json
slug: api-key
source_filename: api-key.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/api-key.json\",\n  \"title\": \"Solo.io Gloo Portal API Key\",\n  \"description\": \"An API key used to authenticate requests to API products exposed through the Gloo developer portal.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API key.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name or label for the API key.\"\n    },\n    \"apiProductId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the API product this key grants access to.\"\n    },\n    \"usagePlanId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the usage plan associated with this key.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Timestamp when the API key was created.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional metadata associated with the API key.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/api-key.json
tags:
- AI Gateway
- Analytics
- Automation
- Gateways
- Management
- Monetization
- Observability
- Platform
- Resiliency
- Security
- Service Mesh
- Traffic Control
title: Solo.io Gloo Portal API Key
---
