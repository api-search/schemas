---
description: ListTagsForResourceOutput schema from Amazon Step Functions API
layout: schema
name: ListTagsForResourceOutput
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-list-tags-for-resource-output-schema.json
slug: amazon-step-functions-list-tags-for-resource-output
source_filename: amazon-step-functions-list-tags-for-resource-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-list-tags-for-resource-output-schema.json\",\n  \"title\": \"ListTagsForResourceOutput\",\n  \"description\": \"ListTagsForResourceOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"An array of tags associated with the resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-list-tags-for-resource-output-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: ListTagsForResourceOutput
---
