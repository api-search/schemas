---
description: A usage plan that defines rate limiting policies, quotas, and access levels for API products in the Gloo developer portal.
layout: schema
name: Solo.io Gloo Portal Usage Plan
properties_list:
- description: Unique identifier for the usage plan.
  name: id
  type: string
- description: Name of the usage plan.
  name: name
  type: string
- description: Description of the usage plan.
  name: description
  type: string
- description: Rate limiting configuration for this plan.
  name: rateLimitPolicy
  type: object
- description: List of API product IDs available under this plan.
  name: apiProducts
  type: array
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/usage-plan.json
slug: usage-plan
source_filename: usage-plan.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/usage-plan.json\",\n  \"title\": \"Solo.io Gloo Portal Usage Plan\",\n  \"description\": \"A usage plan that defines rate limiting policies, quotas, and access levels for API products in the Gloo developer portal.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the usage plan.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the usage plan.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the usage plan.\"\n    },\n    \"rateLimitPolicy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"requestsPerUnit\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of allowed requests per time unit.\"\n        },\n\
  \        \"unit\": {\n          \"type\": \"string\",\n          \"enum\": [\"SECOND\", \"MINUTE\", \"HOUR\", \"DAY\"],\n          \"description\": \"Time unit for rate limiting.\"\n        }\n      },\n      \"description\": \"Rate limiting configuration for this plan.\"\n    },\n    \"apiProducts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of API product IDs available under this plan.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/usage-plan.json
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
title: Solo.io Gloo Portal Usage Plan
---
