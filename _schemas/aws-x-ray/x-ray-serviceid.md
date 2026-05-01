---
description: ''
layout: schema
name: ServiceId
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: Names
  type: array
- description: ''
  name: AccountId
  type: string
- description: ''
  name: Type
  type: string
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-serviceid-schema.json
slug: x-ray-serviceid
source_filename: x-ray-serviceid-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceId\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"Names\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"AccountId\": {\n      \"type\": \"string\"\n    },\n    \"Type\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-serviceid-schema.json
tags:
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: ServiceId
---
