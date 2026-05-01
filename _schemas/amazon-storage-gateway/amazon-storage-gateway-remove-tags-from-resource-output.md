---
description: RemoveTagsFromResourceOutput
layout: schema
name: RemoveTagsFromResourceOutput
properties_list:
- description: ''
  name: ResourceARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-remove-tags-from-resource-output-schema.json
slug: amazon-storage-gateway-remove-tags-from-resource-output
source_filename: amazon-storage-gateway-remove-tags-from-resource-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-remove-tags-from-resource-output-schema.json\",\n  \"title\": \"RemoveTagsFromResourceOutput\",\n  \"description\": \"RemoveTagsFromResourceOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource that the tags were removed from.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-remove-tags-from-resource-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: RemoveTagsFromResourceOutput
---
