---
description: team schema from Acquia Cloud API
layout: schema
name: Team
properties_list:
- description: The UUID of the team.
  name: uuid
  type: string
- description: The name of the team.
  name: name
  type: string
- description: The date the team was created.
  name: created_at
  type: string
- description: The date the team was last updated.
  name: updated_at
  type: string
- description: ''
  name: organization
  type: object
- description: ''
  name: _links
  type: object
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-team-schema.json
slug: acquia-cloud-team
source_filename: acquia-cloud-team-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-team-schema.json\",\n  \"title\": \"Team\",\n  \"description\": \"team schema from Acquia Cloud API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the team.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the team.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date the team was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date the team was last updated.\"\n    },\n    \"organization\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_organization-stub\"\
  \n    },\n    \"_links\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_links\"\n    }\n  },\n  \"required\": [\n    \"uuid\",\n    \"name\",\n    \"created_at\",\n    \"updated_at\",\n    \"organization\",\n    \"_links\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-team-schema.json
tags:
- Content
- Experience
title: Team
---
