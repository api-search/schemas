---
description: Placeholder documentation for CreateMultiplexResponse
layout: schema
name: CreateMultiplexResponse
properties_list:
- description: ''
  name: Multiplex
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-create-multiplex-response-schema.json
slug: medialive-api-create-multiplex-response
source_filename: medialive-api-create-multiplex-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-multiplex-response-schema.json\",\n  \"title\": \"CreateMultiplexResponse\",\n  \"description\": \"Placeholder documentation for CreateMultiplexResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Multiplex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Multiplex\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplex\"\n          },\n          \"description\": \"The newly created multiplex.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-multiplex-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreateMultiplexResponse
---
