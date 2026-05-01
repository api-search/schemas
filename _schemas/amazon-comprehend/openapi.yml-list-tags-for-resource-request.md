---
description: ListTagsForResourceRequest schema
layout: schema
name: ListTagsForResourceRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-list-tags-for-resource-request-schema.json
slug: openapi.yml-list-tags-for-resource-request
source_filename: openapi.yml-list-tags-for-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-tags-for-resource-request-schema.json\",\n  \"title\": \"ListTagsForResourceRequest\",\n  \"description\": \"ListTagsForResourceRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the given Amazon Comprehend resource you are querying. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-tags-for-resource-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ListTagsForResourceRequest
---
