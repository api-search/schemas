---
description: UntagResourceRequest schema from Amazon Global Accelerator API
layout: schema
name: UntagResourceRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-untag-resource-request-schema.json
slug: global-accelerator-untag-resource-request
source_filename: global-accelerator-untag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-untag-resource-request-schema.json\",\n  \"title\": \"UntagResourceRequest\",\n  \"description\": \"UntagResourceRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Global Accelerator resource to remove tags from. An ARN uniquely identifies a resource.\"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeys\"\n        },\n        {\n          \"description\": \"The tag key pairs that you want to remove from the specified resources.\"\n        }\n     \
  \ ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"TagKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-untag-resource-request-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: UntagResourceRequest
---
