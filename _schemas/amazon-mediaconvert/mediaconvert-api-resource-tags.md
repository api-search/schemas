---
description: The Amazon Resource Name (ARN) and tags for an AWS Elemental MediaConvert resource.
layout: schema
name: ResourceTags
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-resource-tags-schema.json
slug: mediaconvert-api-resource-tags
source_filename: mediaconvert-api-resource-tags-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-resource-tags-schema.json\",\n  \"title\": \"ResourceTags\",\n  \"description\": \"The Amazon Resource Name (ARN) and tags for an AWS Elemental MediaConvert resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the resource.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags for the resource.\"\n        }\n   \
  \   ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-resource-tags-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ResourceTags
---
