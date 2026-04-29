---
description: ListTagsForResourceOutput
layout: schema
name: ListTagsForResourceOutput
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: Marker
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-tags-for-resource-output-schema.json
slug: amazon-storage-gateway-list-tags-for-resource-output
source_filename: amazon-storage-gateway-list-tags-for-resource-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-tags-for-resource-output-schema.json\",\n  \"title\": \"ListTagsForResourceOutput\",\n  \"description\": \"ListTagsForResourceOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource for which you want to list tags.\"\n        }\n      ]\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"An opaque string that indicates the position at which to stop returning the list of tags.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"An array that contains the tags for the specified resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-tags-for-resource-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListTagsForResourceOutput
---
