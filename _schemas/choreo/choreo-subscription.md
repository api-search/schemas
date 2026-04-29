---
description: A subscription linking a Choreo developer portal application to a published API under a specific business plan.
layout: schema
name: Choreo Subscription
properties_list:
- description: Unique identifier for the subscription.
  name: id
  type: string
- description: Application identifier.
  name: applicationId
  type: string
- description: API identifier.
  name: apiId
  type: string
- description: Business plan governing the rate limit for this subscription.
  name: businessPlan
  type: string
- description: Status of the subscription.
  name: status
  type: string
- description: Timestamp when the subscription was created.
  name: createdAt
  type: string
provider_name: Choreo
provider_slug: choreo
schema_file: json-schema/choreo-subscription.json
slug: choreo-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-subscription.json\",\n  \"title\": \"Choreo Subscription\",\n  \"description\": \"A subscription linking a Choreo developer portal application to a published API under a specific business plan.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the subscription.\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"Application identifier.\"\n    },\n    \"apiId\": {\n      \"type\": \"string\",\n      \"description\": \"API identifier.\"\n    },\n    \"businessPlan\": {\n      \"type\": \"string\",\n      \"description\": \"Business plan governing the rate limit for this subscription.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"UNBLOCKED\", \"BLOCKED\"\
  , \"PROD_ONLY_BLOCKED\"],\n      \"description\": \"Status of the subscription.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the subscription was created.\"\n    }\n  },\n  \"required\": [\"id\", \"applicationId\", \"apiId\", \"businessPlan\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-subscription.json
tags:
- AI Apps
- API Management
- CI/CD
- Cloud Native
- DevOps
- Developer Portal
- FinOps
- IDE
- Internal Developer Platform
- Kubernetes
- Lifecycle
- Observability
- Orchestration
- Platform Engineering
- Pro-Code API Composition
- Unified
- WSO2
- Workflows
title: Choreo Subscription
---
