---
description: A Release represents a versioned deployment of an integration on the Pandium platform, allowing tenants to be pinned to specific versions.
layout: schema
name: Pandium Release
properties_list:
- description: Unique identifier for the release.
  name: id
  type: integer
- description: ID of the integration this release belongs to.
  name: integration_id
  type: integer
- description: Version label of the release.
  name: version
  type: string
- description: Date and time the release was created.
  name: created_date
  type: string
- description: Date and time the release was last modified.
  name: modified_date
  type: string
provider_name: Pandium
provider_slug: pandium
schema_file: json-schema/release.json
slug: release
source_filename: release.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/pandium/blob/main/json-schema/release.json\",\n  \"title\": \"Pandium Release\",\n  \"description\": \"A Release represents a versioned deployment of an integration on the Pandium platform, allowing tenants to be pinned to specific versions.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"integration_id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the release.\"\n    },\n    \"integration_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the integration this release belongs to.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version label of the release.\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the release was created.\"\n    },\n\
  \    \"modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the release was last modified.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/json-schema/release.json
tags:
- B2B
- Hubs
- Integrations
- Workflows
title: Pandium Release
---
