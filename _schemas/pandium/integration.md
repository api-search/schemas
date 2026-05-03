---
description: An Integration represents a configured connection between Pandium and an external application, enabling data synchronization and workflow automation for B2B SaaS companies.
layout: schema
name: Pandium Integration
properties_list:
- description: Unique identifier for the integration.
  name: id
  type: integer
- description: Name of the integration.
  name: name
  type: string
- description: Whether the integration is archived.
  name: archived
  type: boolean
- description: Date and time the integration was created.
  name: created_date
  type: string
- description: Date and time the integration was last modified.
  name: modified_date
  type: string
provider_name: Pandium
provider_slug: pandium
schema_file: json-schema/integration.json
slug: integration
source_filename: integration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/pandium/blob/main/json-schema/integration.json\",\n  \"title\": \"Pandium Integration\",\n  \"description\": \"An Integration represents a configured connection between Pandium and an external application, enabling data synchronization and workflow automation for B2B SaaS companies.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the integration.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the integration.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the integration is archived.\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the integration was created.\"\
  \n    },\n    \"modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the integration was last modified.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pandium/refs/heads/main/json-schema/integration.json
tags:
- B2B
- Hubs
- Integrations
- Workflows
title: Pandium Integration
---
