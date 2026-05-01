---
description: UntagResourceRequest schema from Amazon MediaConvert API
layout: schema
name: UntagResourceRequest
properties_list:
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-untag-resource-request-schema.json
slug: mediaconvert-api-untag-resource-request
source_filename: mediaconvert-api-untag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-untag-resource-request-schema.json\",\n  \"title\": \"UntagResourceRequest\",\n  \"description\": \"UntagResourceRequest schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tagKeys\"\n          },\n          \"description\": \"The keys of the tags that you want to remove from the resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-untag-resource-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UntagResourceRequest
---
