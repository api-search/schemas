---
description: AddTagsToResourceOutput
layout: schema
name: AddTagsToResourceOutput
properties_list:
- description: ''
  name: ResourceARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-add-tags-to-resource-output-schema.json
slug: amazon-storage-gateway-add-tags-to-resource-output
source_filename: amazon-storage-gateway-add-tags-to-resource-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-add-tags-to-resource-output-schema.json\",\n  \"title\": \"AddTagsToResourceOutput\",\n  \"description\": \"AddTagsToResourceOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource you want to add tags to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-add-tags-to-resource-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: AddTagsToResourceOutput
---
