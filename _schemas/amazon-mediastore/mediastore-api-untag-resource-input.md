---
description: UntagResourceInput schema from Amazon MediaStore API
layout: schema
name: UntagResourceInput
properties_list:
- description: ''
  name: Resource
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-untag-resource-input-schema.json
slug: mediastore-api-untag-resource-input
source_filename: mediastore-api-untag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-untag-resource-input-schema.json\",\n  \"title\": \"UntagResourceInput\",\n  \"description\": \"UntagResourceInput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Resource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the container.\"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeyList\"\n        },\n        {\n          \"description\": \"A comma-separated list of keys for tags that you want to remove from the container. For example, if your container has two tags (customer:CompanyA and priority:High) and you want to remove one\
  \ of the tags (priority:High), you specify the key for the tag that you want to remove (priority).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Resource\",\n    \"TagKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-untag-resource-input-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UntagResourceInput
---
