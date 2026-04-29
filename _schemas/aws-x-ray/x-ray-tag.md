---
description: ''
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: string
- description: ''
  name: Value
  type: string
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-tag-schema.json
slug: x-ray-tag
source_filename: x-ray-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tag\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\"\n    },\n    \"Value\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-tag-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: Tag
---
