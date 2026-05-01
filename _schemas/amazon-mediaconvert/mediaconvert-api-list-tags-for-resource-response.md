---
description: ListTagsForResourceResponse schema from Amazon MediaConvert API
layout: schema
name: ListTagsForResourceResponse
properties_list:
- description: ''
  name: ResourceTags
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-list-tags-for-resource-response-schema.json
slug: mediaconvert-api-list-tags-for-resource-response
source_filename: mediaconvert-api-list-tags-for-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-list-tags-for-resource-response-schema.json\",\n  \"title\": \"ListTagsForResourceResponse\",\n  \"description\": \"ListTagsForResourceResponse schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceTags\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) and tags for an AWS Elemental MediaConvert resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-list-tags-for-resource-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListTagsForResourceResponse
---
