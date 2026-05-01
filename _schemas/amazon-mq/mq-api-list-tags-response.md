---
description: ListTagsResponse schema from Amazon MQ API
layout: schema
name: ListTagsResponse
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-list-tags-response-schema.json
slug: mq-api-list-tags-response
source_filename: mq-api-list-tags-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-list-tags-response-schema.json\",\n  \"title\": \"ListTagsResponse\",\n  \"description\": \"ListTagsResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The key-value pair for the resource tag.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-list-tags-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListTagsResponse
---
