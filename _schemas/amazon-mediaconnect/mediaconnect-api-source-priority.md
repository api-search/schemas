---
description: The priority you want to assign to a source. You can have a primary stream and a backup stream or two equally prioritized streams.
layout: schema
name: SourcePriority
properties_list:
- description: ''
  name: PrimarySource
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-source-priority-schema.json
slug: mediaconnect-api-source-priority
source_filename: mediaconnect-api-source-priority-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-source-priority-schema.json\",\n  \"title\": \"SourcePriority\",\n  \"description\": \"The priority you want to assign to a source. You can have a primary stream and a backup stream or two equally prioritized streams.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PrimarySource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"primarySource\"\n          },\n          \"description\": \"The name of the source you choose as the primary source for this flow.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-source-priority-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: SourcePriority
---
