---
description: ProviderApp schema from Ampersand API
layout: schema
name: ProviderApp
properties_list:
- description: The provider app ID.
  name: id
  type: string
- description: The Ampersand project ID.
  name: projectId
  type: string
- description: The ID used by the provider to identify the app (optional).
  name: externalRef
  type: string
- description: The SaaS provider that this app connects to.
  name: provider
  type: string
- description: The OAuth client ID for this app.
  name: clientId
  type: string
- description: The OAuth scopes for this app.
  name: scopes
  type: array
- description: ''
  name: metadata
  type: object
- description: The time the provider app was created.
  name: createTime
  type: string
- description: The time the provider app was updated.
  name: updateTime
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-provider-app-schema.json
slug: ampersand-api-provider-app
source_filename: ampersand-api-provider-app-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-provider-app-schema.json\",\n  \"title\": \"ProviderApp\",\n  \"description\": \"ProviderApp schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The provider app ID.\",\n      \"example\": \"provider-app-123\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The Ampersand project ID.\",\n      \"example\": \"project-456\"\n    },\n    \"externalRef\": {\n      \"type\": \"string\",\n      \"description\": \"The ID used by the provider to identify the app (optional).\",\n      \"example\": \"external-id-123\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The SaaS provider that this app connects to.\",\n      \"example\": \"salesforce\"\
  \n    },\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"The OAuth client ID for this app.\",\n      \"example\": \"client-id-123\"\n    },\n    \"scopes\": {\n      \"type\": \"array\",\n      \"description\": \"The OAuth scopes for this app.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"example\": [\n          \"oauth\",\n          \"offline\",\n          \"crm.read\"\n        ]\n      }\n    },\n    \"metadata\": {\n      \"$ref\": \"#/components/schemas/ProviderAppMetadata\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the provider app was created.\",\n      \"format\": \"date-time\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the provider app was updated.\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"clientId\",\n    \"createTime\",\n    \"id\",\n    \"projectId\",\n    \"provider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-provider-app-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: ProviderApp
---
