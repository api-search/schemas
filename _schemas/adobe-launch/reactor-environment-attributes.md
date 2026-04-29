---
description: ''
layout: schema
name: EnvironmentAttributes
properties_list:
- description: The name of the environment.
  name: name
  type: string
- description: The environment stage.
  name: stage
  type: string
- description: Whether the build is delivered as a ZIP archive.
  name: archive
  type: boolean
- description: The URL path appended to the host domain for deployment.
  name: path
  type: string
- description: The custom library filename.
  name: library_name
  type: string
- description: The custom library path.
  name: library_path
  type: string
- description: A unique token for the environment.
  name: token
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/reactor-environment-attributes-schema.json
slug: reactor-environment-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvironmentAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the environment.\"\n    },\n    \"stage\": {\n      \"type\": \"string\",\n      \"description\": \"The environment stage.\"\n    },\n    \"archive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the build is delivered as a ZIP archive.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The URL path appended to the host domain for deployment.\"\n    },\n    \"library_name\": {\n      \"type\": \"string\",\n      \"description\": \"The custom library filename.\"\n    },\n    \"library_path\": {\n      \"type\": \"string\",\n      \"description\": \"The custom library path.\"\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"A unique token for the environment.\"\
  \n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/reactor-environment-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: EnvironmentAttributes
---
