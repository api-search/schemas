---
description: Project schema from Ampersand API
layout: schema
name: Project
properties_list:
- description: The unique identifier for the project.
  name: id
  type: string
- description: The unique name for the project.
  name: name
  type: string
- description: The display name of the application, shown to end users during the connection flow.
  name: appName
  type: string
- description: The ID of the organization that this project belongs to.
  name: orgId
  type: string
- description: The time the project was created.
  name: createTime
  type: string
- description: The time the project was updated.
  name: updateTime
  type: string
- description: Plan-based feature flags for the project. These are managed by Ampersand and cannot be set via the API.
  name: entitlements
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-project-schema.json
slug: ampersand-api-project
source_filename: ampersand-api-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-project-schema.json\",\n  \"title\": \"Project\",\n  \"description\": \"Project schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the project.\",\n      \"example\": \"proj_9f7c3e2a-61b8-4f5c-8d1a-eb24f3b05d79\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name for the project.\",\n      \"example\": \"mailmonkey-staging\"\n    },\n    \"appName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the application, shown to end users during the connection flow.\",\n      \"example\": \"MailMonkey\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the organization\
  \ that this project belongs to.\",\n      \"example\": \"9f7c3e2a-61b8-4f5c-8d1a-eb24f3b05d79\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the project was created.\",\n      \"format\": \"date-time\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the project was updated.\",\n      \"format\": \"date-time\"\n    },\n    \"entitlements\": {\n      \"type\": \"object\",\n      \"description\": \"Plan-based feature flags for the project. These are managed by Ampersand and cannot be set via the API.\",\n      \"properties\": {\n        \"brandingRemoval\": {\n          \"type\": \"object\",\n          \"required\": [\n            \"value\"\n          ],\n          \"x-go-type-skip-optional-pointer\": true,\n          \"description\": \"Controls whether Ampersand branding is removed from the embeddable UI components.\",\n          \"properties\": {\n            \"value\": {\n              \"type\"\
  : \"boolean\",\n              \"description\": \"True if Ampersand branding has been removed for this project.\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"appName\",\n    \"createTime\",\n    \"id\",\n    \"name\",\n    \"orgId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-project-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: Project
---
