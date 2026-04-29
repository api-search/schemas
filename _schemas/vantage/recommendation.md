---
description: A cost optimization Recommendation identifying potential savings for a specific cloud resource.
layout: schema
name: Vantage Recommendation
properties_list:
- description: The unique token identifier for the Recommendation.
  name: token
  type: string
- description: The type of recommendation.
  name: type
  type: string
- description: A description of the recommendation.
  name: description
  type: string
- description: The estimated monthly savings.
  name: estimated_savings
  type: string
- description: The cloud provider.
  name: provider
  type: string
- description: The cloud service.
  name: service
  type: string
- description: The resource identifier.
  name: resource_id
  type: string
- description: The date and time the Recommendation was generated.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/recommendation.json
slug: recommendation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/recommendation.json\",\n  \"title\": \"Vantage Recommendation\",\n  \"description\": \"A cost optimization Recommendation identifying potential savings for a specific cloud resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Recommendation.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of recommendation.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the recommendation.\"\n    },\n    \"estimated_savings\": {\n      \"type\": \"string\",\n      \"description\": \"The estimated monthly savings.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider.\"\n    },\n    \"\
  service\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud service.\"\n    },\n    \"resource_id\": {\n      \"type\": \"string\",\n      \"description\": \"The resource identifier.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the Recommendation was generated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/recommendation.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Recommendation
---
