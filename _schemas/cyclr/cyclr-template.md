---
description: A Cyclr template is a reusable integration blueprint that defines a pre-configured workflow of steps and connector mappings. Templates can be installed into accounts to create active integration cycles.
layout: schema
name: Cyclr Template
properties_list:
- description: Unique template identifier
  name: Id
  type: string
- description: Template name
  name: Name
  type: string
- description: Template description
  name: Description
  type: string
- description: Connectors used by the template
  name: Connectors
  type: array
- description: Tags associated with the template
  name: Tags
  type: array
provider_name: Cyclr
provider_slug: cyclr
schema_file: json-schema/cyclr-template.json
slug: cyclr-template
source_filename: cyclr-template.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/json-schema/cyclr-template.json\",\n  \"title\": \"Cyclr Template\",\n  \"description\": \"A Cyclr template is a reusable integration blueprint that defines a pre-configured workflow of steps and connector mappings. Templates can be installed into accounts to create active integration cycles.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique template identifier\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Template name\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Template description\"\n    },\n    \"Connectors\": {\n      \"type\": \"array\",\n      \"description\": \"Connectors used by the template\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"Id\": {\n            \"type\": \"integer\",\n            \"description\": \"Connector identifier\"\n          },\n          \"Name\": {\n            \"type\": \"string\",\n            \"description\": \"Connector name\"\n          }\n        }\n      }\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the template\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\"Id\", \"Name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/json-schema/cyclr-template.json
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
title: Cyclr Template
---
