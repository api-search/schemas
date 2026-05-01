---
description: Represents an API plan in the Gravitee platform that defines access tiers, security policies, and rate limits for API consumers.
layout: schema
name: Gravitee Plan
properties_list:
- description: Unique identifier for the plan.
  name: id
  type: string
- description: Name of the plan.
  name: name
  type: string
- description: Description of the plan and its access tier.
  name: description
  type: string
- description: Security type required for consumers using this plan.
  name: security
  type: string
- description: Current status of the plan.
  name: status
  type: string
- description: Subscription validation mode - AUTO approves immediately, MANUAL requires admin approval.
  name: validation
  type: string
provider_name: Gravitee
provider_slug: gravitee
schema_file: json-schema/gravitee-plan-schema.json
slug: gravitee-plan
source_filename: gravitee-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://gravitee.io/schemas/gravitee/plan.json\",\n  \"title\": \"Gravitee Plan\",\n  \"description\": \"Represents an API plan in the Gravitee platform that defines access tiers, security policies, and rate limits for API consumers.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"security\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the plan.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the plan.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the plan and its access tier.\"\n    },\n    \"security\": {\n      \"type\": \"string\",\n      \"description\": \"Security type required for consumers using this plan.\",\n      \"enum\": [\"KEY_LESS\", \"API_KEY\", \"OAUTH2\", \"JWT\"]\n    },\n\
  \    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the plan.\",\n      \"enum\": [\"STAGING\", \"PUBLISHED\", \"CLOSED\", \"DEPRECATED\"]\n    },\n    \"validation\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription validation mode - AUTO approves immediately, MANUAL requires admin approval.\",\n      \"enum\": [\"AUTO\", \"MANUAL\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gravitee/refs/heads/main/json-schema/gravitee-plan-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: Gravitee Plan
---
