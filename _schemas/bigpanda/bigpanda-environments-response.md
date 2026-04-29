---
description: List of BigPanda environments.
layout: schema
name: EnvironmentsResponse
properties_list:
- description: Array of environments.
  name: environments
  type: array
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-environments-response-schema.json
slug: bigpanda-environments-response
source_filename: bigpanda-environments-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"EnvironmentsResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of BigPanda environments.\",\n  \"properties\": {\n    \"environments\": {\n      \"type\": \"array\",\n      \"description\": \"Array of environments.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Environment\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-environments-response-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: EnvironmentsResponse
---
