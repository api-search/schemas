---
description: ListTagsForResourceOutput schema from Amazon CodePipeline
layout: schema
name: ListTagsForResourceOutput
properties_list:
- description: ''
  name: tags
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-list-tags-for-resource-output-schema.json
slug: amazon-codepipeline-list-tags-for-resource-output
source_filename: amazon-codepipeline-list-tags-for-resource-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-tags-for-resource-output-schema.json\",\n  \"title\": \"ListTagsForResourceOutput\",\n  \"description\": \"ListTagsForResourceOutput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags for the resource.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If the amount of returned information is significantly large, an identifier is also returned and can be used in a subsequent API call to return the next page of the list. The ListTagsforResource call\
  \ lists all available tags in one call and does not use pagination.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-tags-for-resource-output-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ListTagsForResourceOutput
---
