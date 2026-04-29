---
description: RemoveTagsFromResourceInput
layout: schema
name: RemoveTagsFromResourceInput
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-remove-tags-from-resource-input-schema.json
slug: amazon-storage-gateway-remove-tags-from-resource-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-remove-tags-from-resource-input-schema.json\",\n  \"title\": \"RemoveTagsFromResourceInput\",\n  \"description\": \"RemoveTagsFromResourceInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource you want to remove the tags from.\"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeys\"\n        },\n        {\n          \"description\": \"The keys of the tags you want to remove from the specified resource. A tag is composed of a key-value pair.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"ResourceARN\",\n    \"TagKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-remove-tags-from-resource-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: RemoveTagsFromResourceInput
---
