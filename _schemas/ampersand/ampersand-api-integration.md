---
description: Integration schema from Ampersand API
layout: schema
name: Integration
properties_list:
- description: The integration ID.
  name: id
  type: string
- description: The Ampersand project ID.
  name: projectId
  type: string
- description: The integration name.
  name: name
  type: string
- description: The SaaS provider that this integration connects to.
  name: provider
  type: string
- description: The time the integration was created.
  name: createTime
  type: string
- description: The time the integration was last updated.
  name: updateTime
  type: string
- description: ''
  name: latestRevision
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-integration-schema.json
slug: ampersand-api-integration
source_filename: ampersand-api-integration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-integration-schema.json\",\n  \"title\": \"Integration\",\n  \"description\": \"Integration schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The integration ID.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The Ampersand project ID.\",\n      \"example\": \"project-456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The integration name.\",\n      \"example\": \"read-accounts\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The SaaS provider that this integration connects to.\",\n      \"example\": \"salesforce\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The time the integration was created.\",\n      \"format\": \"date-time\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the integration was last updated.\",\n      \"format\": \"date-time\"\n    },\n    \"latestRevision\": {\n      \"$ref\": \"#/components/schemas/Revision\"\n    }\n  },\n  \"required\": [\n    \"createTime\",\n    \"id\",\n    \"latestRevision\",\n    \"name\",\n    \"projectId\",\n    \"provider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-integration-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: Integration
---
