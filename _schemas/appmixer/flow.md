---
description: A Flow represents an automation workflow in Appmixer, consisting of connected components that define integration logic between services.
layout: schema
name: Appmixer Flow
properties_list:
- description: Unique identifier for the flow.
  name: id
  type: string
- description: Human-readable name of the flow.
  name: name
  type: string
- description: Flow definition object containing the workflow graph and component configurations.
  name: flow
  type: object
- description: Current execution state of the flow.
  name: stage
  type: string
- description: Creation timestamp of the flow.
  name: btime
  type: string
- description: Last modification timestamp of the flow.
  name: mtime
  type: string
- description: URL or data URI of the flow thumbnail image.
  name: thumbnail
  type: string
- description: Custom metadata key-value pairs associated with the flow.
  name: customFields
  type: object
provider_name: Appmixer
provider_slug: appmixer
schema_file: json-schema/flow.json
slug: flow
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/appmixer/blob/main/json-schema/flow.json\",\n  \"title\": \"Appmixer Flow\",\n  \"description\": \"A Flow represents an automation workflow in Appmixer, consisting of connected components that define integration logic between services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the flow.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the flow.\"\n    },\n    \"flow\": {\n      \"type\": \"object\",\n      \"description\": \"Flow definition object containing the workflow graph and component configurations.\"\n    },\n    \"stage\": {\n      \"type\": \"string\",\n      \"enum\": [\"running\", \"stopped\"],\n      \"description\": \"Current execution state of the flow.\"\n    },\n    \"btime\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp of the flow.\"\n    },\n    \"mtime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp of the flow.\"\n    },\n    \"thumbnail\": {\n      \"type\": \"string\",\n      \"description\": \"URL or data URI of the flow thumbnail image.\"\n    },\n    \"customFields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata key-value pairs associated with the flow.\",\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/json-schema/flow.json
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
title: Appmixer Flow
---
