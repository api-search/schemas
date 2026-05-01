---
description: AddTagsToResourceInput
layout: schema
name: AddTagsToResourceInput
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-add-tags-to-resource-input-schema.json
slug: amazon-storage-gateway-add-tags-to-resource-input
source_filename: amazon-storage-gateway-add-tags-to-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-add-tags-to-resource-input-schema.json\",\n  \"title\": \"AddTagsToResourceInput\",\n  \"description\": \"AddTagsToResourceInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource you want to add tags to.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>The key-value pair that represents the tag you want to add to the resource. The value can be an empty string.</p> <note> <p>Valid characters for key and value are letters, spaces, and\
  \ numbers representable in UTF-8 format, and the following special characters: + - = . _ : / @. The maximum length of a tag's key is 128 characters, and the maximum length for a tag's value is 256.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceARN\",\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-add-tags-to-resource-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: AddTagsToResourceInput
---
