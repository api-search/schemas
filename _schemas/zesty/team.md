---
description: A Zesty.io team groups multiple users together for shared access and role management across instances.
layout: schema
name: Zesty Team
properties_list:
- description: The Zesty Universal Identifier for the team.
  name: ZUID
  type: string
- description: The name of the team.
  name: name
  type: string
- description: A description of the team.
  name: description
  type: string
- description: Timestamp when the team was created.
  name: createdAt
  type: string
- description: Timestamp when the team was last updated.
  name: updatedAt
  type: string
provider_name: Zesty
provider_slug: zesty
schema_file: json-schema/team.json
slug: team
source_filename: team.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zesty/blob/main/json-schema/team.json\",\n  \"title\": \"Zesty Team\",\n  \"description\": \"A Zesty.io team groups multiple users together for shared access and role management across instances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The Zesty Universal Identifier for the team.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the team.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the team.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the team was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when\
  \ the team was last updated.\"\n    }\n  },\n  \"required\": [\"ZUID\", \"name\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/json-schema/team.json
tags:
- CMS
- Composable
- Content Management
- Headless CMS
- Media
title: Zesty Team
---
