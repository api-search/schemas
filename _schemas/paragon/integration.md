---
description: An Integration represents a third-party SaaS application that can be connected and configured through Paragon's Connect Portal.
layout: schema
name: Paragon Integration
properties_list:
- description: The unique identifier for the integration.
  name: id
  type: string
- description: The display name of the integration (e.g., Salesforce, HubSpot).
  name: name
  type: string
- description: The integration type identifier used in API paths (e.g., salesforce, hubspot).
  name: type
  type: string
- description: Whether the integration is enabled for the authenticated user.
  name: enabled
  type: boolean
- description: URL to the integration icon.
  name: icon
  type: string
provider_name: Paragon
provider_slug: paragon
schema_file: json-schema/integration.json
slug: integration
source_filename: integration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/paragon/blob/main/json-schema/integration.json\",\n  \"title\": \"Paragon Integration\",\n  \"description\": \"An Integration represents a third-party SaaS application that can be connected and configured through Paragon's Connect Portal.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the integration.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the integration (e.g., Salesforce, HubSpot).\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The integration type identifier used in API paths (e.g., salesforce, hubspot).\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the integration is enabled for the authenticated user.\"\n    },\n  \
  \  \"icon\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the integration icon.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/json-schema/integration.json
tags:
- Embedded iPaaS
- Integrations
title: Paragon Integration
---
