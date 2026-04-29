---
description: TagResourceRequest schema from Amazon MediaConvert API
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-tag-resource-request-schema.json
slug: mediaconvert-api-tag-resource-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the resource that you want to tag. To get the ARN, send a GET request with the resource name.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n         \
  \ \"description\": \"The tags that you want to add to the resource. You can tag resources with a key-value pair or with only a key.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\",\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-tag-resource-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TagResourceRequest
---
