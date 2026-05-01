---
description: ListTagsForResourceRequest schema from Amazon Global Accelerator API
layout: schema
name: ListTagsForResourceRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-list-tags-for-resource-request-schema.json
slug: global-accelerator-list-tags-for-resource-request
source_filename: global-accelerator-list-tags-for-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-list-tags-for-resource-request-schema.json\",\n  \"title\": \"ListTagsForResourceRequest\",\n  \"description\": \"ListTagsForResourceRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the accelerator to list tags for. An ARN uniquely identifies an accelerator.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-list-tags-for-resource-request-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: ListTagsForResourceRequest
---
