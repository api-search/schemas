---
description: A notification endpoint configuration in Finout, supporting email, Slack, and Microsoft Teams channels for cost alerts and notifications.
layout: schema
name: Finout Endpoint
properties_list:
- description: The unique identifier of the endpoint.
  name: id
  type: string
- description: The name of the endpoint.
  name: name
  type: string
- description: The type of endpoint.
  name: type
  type: string
- description: Endpoint-specific configuration.
  name: configuration
  type: object
provider_name: Finout
provider_slug: finout
schema_file: json-schema/endpoint.json
slug: endpoint
source_filename: endpoint.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/finout/blob/main/json-schema/endpoint.json\",\n  \"title\": \"Finout Endpoint\",\n  \"description\": \"A notification endpoint configuration in Finout, supporting email, Slack, and Microsoft Teams channels for cost alerts and notifications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the endpoint.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the endpoint.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of endpoint.\",\n      \"enum\": [\"email\", \"slack\", \"teams\"]\n    },\n    \"configuration\": {\n      \"type\": \"object\",\n      \"description\": \"Endpoint-specific configuration.\",\n      \"properties\": {\n        \"to\": {\n          \"type\": \"string\",\n   \
  \       \"description\": \"The destination address. An email address for email endpoints or a webhook URL for Slack/Teams endpoints.\"\n        }\n      },\n      \"required\": [\"to\"]\n    }\n  },\n  \"required\": [\"id\", \"name\", \"type\", \"configuration\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/finout/refs/heads/main/json-schema/endpoint.json
tags:
- Budgets
- Costs
- FinOps
title: Finout Endpoint
---
