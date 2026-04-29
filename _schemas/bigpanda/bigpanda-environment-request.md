---
description: Payload for creating or updating an environment.
layout: schema
name: EnvironmentRequest
properties_list:
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
schema_file: json-schema/bigpanda-environment-request-schema.json
slug: bigpanda-environment-request
source_filename: bigpanda-environment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"EnvironmentRequest\",\n  \"type\": \"object\",\n  \"description\": \"Payload for creating or updating an environment.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Environment name.\",\n      \"example\": \"Production\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Environment description.\",\n      \"example\": \"Production environment\"\n    },\n    \"condition\": {\n      \"type\": \"string\",\n      \"description\": \"Filter condition for grouping incidents.\",\n      \"example\": \"source = \\\"nagios\\\"\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"condition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-environment-request-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: EnvironmentRequest
---
