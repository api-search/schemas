---
description: A Cyclr cycle is an active integration workflow running within an account. Cycles are typically created by installing templates and consist of a series of steps that move data between connected applications.
layout: schema
name: Cyclr Cycle
properties_list:
- description: Unique cycle identifier
  name: Id
  type: string
- description: Cycle name
  name: Name
  type: string
- description: Cycle description
  name: Description
  type: string
- description: Current cycle status
  name: Status
  type: string
- description: When the cycle was created
  name: CreatedDate
  type: string
- description: When the cycle last ran
  name: LastRunDate
  type: string
- description: Connectors used by the cycle
  name: Connectors
  type: array
- description: Steps in the cycle
  name: Steps
  type: array
provider_name: Cyclr
provider_slug: cyclr
schema_file: json-schema/cyclr-cycle.json
slug: cyclr-cycle
source_filename: cyclr-cycle.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/json-schema/cyclr-cycle.json\",\n  \"title\": \"Cyclr Cycle\",\n  \"description\": \"A Cyclr cycle is an active integration workflow running within an account. Cycles are typically created by installing templates and consist of a series of steps that move data between connected applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique cycle identifier\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Cycle name\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Cycle description\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Current cycle status\",\n      \"enum\": [\"Active\", \"Inactive\", \"Paused\", \"Error\"]\n    },\n    \"CreatedDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the cycle was created\"\n    },\n    \"LastRunDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the cycle last ran\"\n    },\n    \"Connectors\": {\n      \"type\": \"array\",\n      \"description\": \"Connectors used by the cycle\",\n      \"items\": {\n        \"$ref\": \"cyclr-installed-connector.json\"\n      }\n    },\n    \"Steps\": {\n      \"type\": \"array\",\n      \"description\": \"Steps in the cycle\",\n      \"items\": {\n        \"$ref\": \"cyclr-step.json\"\n      }\n    }\n  },\n  \"required\": [\"Id\", \"Name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/json-schema/cyclr-cycle.json
tags:
- Connectors
- Custom Connectors
- Data Synchronization
- Embedded iPaaS
- Embedded SaaS Integration
- Embedded UI
- Integration Platform
- Integrations
- Marketplace
- OAuth 2.0
- REST API
- SaaS
- Templates
- Webhooks
- White Label
- Workflows
title: Cyclr Cycle
---
