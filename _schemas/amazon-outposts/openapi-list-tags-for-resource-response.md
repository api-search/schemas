---
description: ListTagsForResourceResponse schema from Amazon Outposts
layout: schema
name: ListTagsForResourceResponse
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-list-tags-for-resource-response-schema.json
slug: openapi-list-tags-for-resource-response
source_filename: openapi-list-tags-for-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-list-tags-for-resource-response-schema.json\",\n  \"title\": \"ListTagsForResourceResponse\",\n  \"description\": \"ListTagsForResourceResponse schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The resource tags.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-list-tags-for-resource-response-schema.json
tags:
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: ListTagsForResourceResponse
---
