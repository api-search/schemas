---
description: Installation schema from Ampersand API
layout: schema
name: Installation
properties_list:
- description: The installation ID.
  name: id
  type: string
- description: The Ampersand project ID.
  name: projectId
  type: string
- description: The integration ID.
  name: integrationId
  type: string
- description: ''
  name: group
  type: object
- description: The health status of the installation.
  name: healthStatus
  type: string
- description: The status of the latest operation for this installation.
  name: lastOperationStatus
  type: string
- description: ''
  name: connection
  type: object
- description: The time the installation was created.
  name: createTime
  type: string
- description: The person who did the installation, in the format of "consumer:{consumer-id}".
  name: createdBy
  type: string
- description: The time the installation was last updated with a new config.
  name: updateTime
  type: string
- description: ''
  name: config
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-installation-schema.json
slug: ampersand-api-installation
source_filename: ampersand-api-installation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-installation-schema.json\",\n  \"title\": \"Installation\",\n  \"description\": \"Installation schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The installation ID.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The Ampersand project ID.\",\n      \"example\": \"project-456\"\n    },\n    \"integrationId\": {\n      \"type\": \"string\",\n      \"description\": \"The integration ID.\"\n    },\n    \"group\": {\n      \"$ref\": \"#/components/schemas/Group\"\n    },\n    \"healthStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"healthy\",\n        \"unhealthy\"\n      ],\n      \"description\": \"The health status of the installation.\",\n \
  \     \"example\": \"healthy\"\n    },\n    \"lastOperationStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"success\",\n        \"failure\",\n        \"in_progress\"\n      ],\n      \"description\": \"The status of the latest operation for this installation.\\n\",\n      \"example\": \"success\"\n    },\n    \"connection\": {\n      \"$ref\": \"#/components/schemas/Connection\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the installation was created.\",\n      \"format\": \"date-time\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The person who did the installation, in the format of \\\"consumer:{consumer-id}\\\".\",\n      \"example\": \"consumer:consumer-123\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the installation was last updated with a new config.\",\n      \"format\": \"date-time\"\n    },\n    \"config\": {\n  \
  \    \"$ref\": \"#/components/schemas/Config\"\n    }\n  },\n  \"required\": [\n    \"config\",\n    \"connection\",\n    \"createTime\",\n    \"createdBy\",\n    \"healthStatus\",\n    \"id\",\n    \"integrationId\",\n    \"projectId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-installation-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: Installation
---
