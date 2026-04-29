---
description: ListTagsForResourceInput schema from Amazon MediaStore API
layout: schema
name: ListTagsForResourceInput
properties_list:
- description: ''
  name: Resource
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-list-tags-for-resource-input-schema.json
slug: mediastore-api-list-tags-for-resource-input
source_filename: mediastore-api-list-tags-for-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-list-tags-for-resource-input-schema.json\",\n  \"title\": \"ListTagsForResourceInput\",\n  \"description\": \"ListTagsForResourceInput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Resource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the container.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Resource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-list-tags-for-resource-input-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListTagsForResourceInput
---
