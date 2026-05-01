---
description: The response to the request.
layout: schema
name: ListTagsForResourceResponse
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-list-tags-for-resource-response-schema.json
slug: iam-access-analyzer-list-tags-for-resource-response
source_filename: iam-access-analyzer-list-tags-for-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-tags-for-resource-response-schema.json\",\n  \"title\": \"ListTagsForResourceResponse\",\n  \"description\": \"The response to the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"The tags that are applied to the specified resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-tags-for-resource-response-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: ListTagsForResourceResponse
---
