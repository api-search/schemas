---
description: A build agent resource in JetBrains TeamCity.
layout: schema
name: JetBrains TeamCity Build Agent
properties_list:
- description: Unique numeric identifier of the agent.
  name: id
  type: integer
- description: Name of the build agent.
  name: name
  type: string
- description: Agent type identifier.
  name: typeId
  type: integer
- description: Whether the agent is currently connected.
  name: connected
  type: boolean
- description: Whether the agent is enabled for builds.
  name: enabled
  type: boolean
- description: Whether the agent is authorized.
  name: authorized
  type: boolean
- description: IP address of the agent.
  name: ip
  type: string
- description: Agent pool the agent belongs to.
  name: pool
  type: object
- description: Operating system type of the agent.
  name: osType
  type: string
provider_name: JetBrains
provider_slug: jetbrains
schema_file: json-schema/build-agent.json
slug: build-agent
source_filename: build-agent.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"jetbrains-build-agent.json\",\n  \"title\": \"JetBrains TeamCity Build Agent\",\n  \"description\": \"A build agent resource in JetBrains TeamCity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier of the agent.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the build agent.\"\n    },\n    \"typeId\": {\n      \"type\": \"integer\",\n      \"description\": \"Agent type identifier.\"\n    },\n    \"connected\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the agent is currently connected.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the agent is enabled for builds.\"\n    },\n    \"authorized\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the agent is authorized.\"\n\
  \    },\n    \"ip\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the agent.\"\n    },\n    \"pool\": {\n      \"type\": \"object\",\n      \"description\": \"Agent pool the agent belongs to.\",\n      \"properties\": {\n        \"id\": { \"type\": \"integer\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"osType\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system type of the agent.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/json-schema/build-agent.json
tags:
- CI/CD
- Developer Tools
- IDE
title: JetBrains TeamCity Build Agent
---
