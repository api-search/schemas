---
description: A Cyclr step represents an individual action within a cycle. Each step calls a specific method on a connector and can include parameters and field mappings to transform data between steps.
layout: schema
name: Cyclr Step
properties_list:
- description: Unique step identifier
  name: Id
  type: string
- description: Step name
  name: Name
  type: string
- description: Step description
  name: Description
  type: string
- description: ID of the connector used by this step
  name: ConnectorId
  type: integer
- description: ID of the method called by this step
  name: MethodId
  type: string
provider_name: Cyclr
provider_slug: cyclr
schema_file: json-schema/cyclr-step.json
slug: cyclr-step
source_filename: cyclr-step.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/json-schema/cyclr-step.json\",\n  \"title\": \"Cyclr Step\",\n  \"description\": \"A Cyclr step represents an individual action within a cycle. Each step calls a specific method on a connector and can include parameters and field mappings to transform data between steps.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique step identifier\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Step name\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Step description\"\n    },\n    \"ConnectorId\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the connector used by this step\"\n    },\n    \"MethodId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the\
  \ method called by this step\"\n    }\n  },\n  \"required\": [\"Id\", \"Name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/json-schema/cyclr-step.json
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
title: Cyclr Step
---
