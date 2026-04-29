---
description: ListTagsForResourceOutput schema from Amazon MediaStore API
layout: schema
name: ListTagsForResourceOutput
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-list-tags-for-resource-output-schema.json
slug: mediastore-api-list-tags-for-resource-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-list-tags-for-resource-output-schema.json\",\n  \"title\": \"ListTagsForResourceOutput\",\n  \"description\": \"ListTagsForResourceOutput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"An array of key:value pairs that are assigned to the container.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-list-tags-for-resource-output-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListTagsForResourceOutput
---
