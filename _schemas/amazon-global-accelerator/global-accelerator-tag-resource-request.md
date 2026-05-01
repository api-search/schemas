---
description: TagResourceRequest schema from Amazon Global Accelerator API
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-tag-resource-request-schema.json
slug: global-accelerator-tag-resource-request
source_filename: global-accelerator-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Global Accelerator resource to add tags to. An ARN uniquely identifies a resource.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"The tags to add to a resource. A tag consists of a key and a value that you define.\"\n        }\n      ]\n \
  \   }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-tag-resource-request-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: TagResourceRequest
---
