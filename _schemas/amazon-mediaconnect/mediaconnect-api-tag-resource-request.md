---
description: The tags to add to the resource. A tag is an array of key-value pairs. Tag keys can have a maximum character length of 128 characters, and tag values can have a maximum length of 256 characters.
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-tag-resource-request-schema.json
slug: mediaconnect-api-tag-resource-request
source_filename: mediaconnect-api-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"The tags to add to the resource. A tag is an array of key-value pairs. Tag keys can have a maximum character length of 128 characters, and tag values can have a maximum length of 256 characters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A map from tag keys to values. Tag keys can have a maximum character length of 128 characters, and tag values can have a maximum length of 256 characters.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Tags\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-tag-resource-request-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: TagResourceRequest
---
