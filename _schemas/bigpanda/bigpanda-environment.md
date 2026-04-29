---
description: A BigPanda environment for incident grouping.
layout: schema
name: Environment
properties_list:
- description: Environment ID.
  name: id
  type: string
- description: Environment name.
  name: name
  type: string
- description: Environment description.
  name: description
  type: string
- description: Filter condition for grouping incidents.
  name: condition
  type: string
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-environment-schema.json
slug: bigpanda-environment
source_filename: bigpanda-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Environment\",\n  \"type\": \"object\",\n  \"description\": \"A BigPanda environment for incident grouping.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Environment ID.\",\n      \"example\": \"env-abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Environment name.\",\n      \"example\": \"Production\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Environment description.\",\n      \"example\": \"Production environment\"\n    },\n    \"condition\": {\n      \"type\": \"string\",\n      \"description\": \"Filter condition for grouping incidents.\",\n      \"example\": \"source = \\\"nagios\\\"\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-environment-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: Environment
---
