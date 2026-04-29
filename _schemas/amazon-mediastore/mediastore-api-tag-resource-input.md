---
description: TagResourceInput schema from Amazon MediaStore API
layout: schema
name: TagResourceInput
properties_list:
- description: ''
  name: Resource
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-tag-resource-input-schema.json
slug: mediastore-api-tag-resource-input
source_filename: mediastore-api-tag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-tag-resource-input-schema.json\",\n  \"title\": \"TagResourceInput\",\n  \"description\": \"TagResourceInput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Resource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the container. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"An array of key:value pairs that you want to add to the container. You need to specify only the tags that you want to add or update. For example, suppose a container already has two tags (customer:CompanyA\
  \ and priority:High). You want to change the priority tag and also add a third tag (type:Contract). For TagResource, you specify the following tags: priority:Medium, type:Contract. The result is that your container has three tags: customer:CompanyA, priority:Medium, and type:Contract.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Resource\",\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-tag-resource-input-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TagResourceInput
---
