---
description: A Tenant represents a customer instance of an integration on the Pandium platform, with its own configuration, schedule, and connection credentials.
layout: schema
name: Pandium Tenant
properties_list:
- description: Unique identifier for the tenant.
  name: id
  type: integer
- description: Name of the tenant.
  name: name
  type: string
- description: Whether the tenant is archived.
  name: archived
  type: boolean
- description: ID of the associated integration.
  name: integration_id
  type: integer
- description: Configuration settings for the tenant.
  name: configs
  type: object
- description: Date and time the tenant was created.
  name: created_date
  type: string
- description: Date and time the tenant was last modified.
  name: modified_date
  type: string
- description: Whether the tenant is paused.
  name: paused
  type: boolean
- description: The user-defined cron schedule for the tenant.
  name: user_schedule
  type: string
- description: The effective schedule for the tenant.
  name: schedule
  type: string
- description: The source of the tenant creation.
  name: source
  type: string
- description: ID of the integration release assigned to this tenant.
  name: integration_release_id
  type: integer
- description: The release channel for the tenant.
  name: integration_release_channel
  type: string
- description: Current status of the tenant.
  name: status
  type: string
provider_name: Pandium
provider_slug: pandium
schema_file: json-schema/tenant.json
slug: tenant
source_filename: tenant.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/pandium/blob/main/json-schema/tenant.json\",\n  \"title\": \"Pandium Tenant\",\n  \"description\": \"A Tenant represents a customer instance of an integration on the Pandium platform, with its own configuration, schedule, and connection credentials.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"integration_id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the tenant.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the tenant.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the tenant is archived.\"\n    },\n    \"integration_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the associated integration.\"\n    },\n    \"configs\": {\n      \"type\": \"object\",\n  \
  \    \"description\": \"Configuration settings for the tenant.\",\n      \"additionalProperties\": true\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the tenant was created.\"\n    },\n    \"modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the tenant was last modified.\"\n    },\n    \"paused\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the tenant is paused.\"\n    },\n    \"user_schedule\": {\n      \"type\": \"string\",\n      \"description\": \"The user-defined cron schedule for the tenant.\"\n    },\n    \"schedule\": {\n      \"type\": \"string\",\n      \"description\": \"The effective schedule for the tenant.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The source of the tenant creation.\"\n    },\n    \"integration_release_id\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"ID of the integration release assigned to this tenant.\"\n    },\n    \"integration_release_channel\": {\n      \"type\": \"string\",\n      \"description\": \"The release channel for the tenant.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the tenant.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/json-schema/tenant.json
tags:
- B2B
- Hubs
- Integrations
- Workflows
title: Pandium Tenant
---
