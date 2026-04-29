---
description: Org schema from Ampersand API
layout: schema
name: Org
properties_list:
- description: The organization ID.
  name: id
  type: string
- description: The organization label.
  name: label
  type: string
- description: The ID of the Everyone team for the org.
  name: defaultTeamId
  type: string
- description: The time the organization was created.
  name: createTime
  type: string
- description: The time the organization was updated.
  name: updateTime
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-org-schema.json
slug: ampersand-api-org
source_filename: ampersand-api-org-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-org-schema.json\",\n  \"title\": \"Org\",\n  \"description\": \"Org schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The organization ID.\",\n      \"example\": \"9f7c3e2a-61b8-4f5c-8d1a-eb24f3b05d79\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The organization label.\",\n      \"example\": \"Acme Inc\"\n    },\n    \"defaultTeamId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Everyone team for the org.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the organization was created.\",\n      \"format\": \"date-time\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The time the organization was updated.\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"label\",\n    \"createTime\",\n    \"defaultTeamId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-org-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: Org
---
