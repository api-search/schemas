---
description: ListTagsForResourceInput schema from Amazon CodePipeline
layout: schema
name: ListTagsForResourceInput
properties_list:
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-list-tags-for-resource-input-schema.json
slug: amazon-codepipeline-list-tags-for-resource-input
source_filename: amazon-codepipeline-list-tags-for-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-tags-for-resource-input-schema.json\",\n  \"title\": \"ListTagsForResourceInput\",\n  \"description\": \"ListTagsForResourceInput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource to get tags for.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token that was returned from the previous API call, which would be used to return the next page of the list. The ListTagsforResource call lists all\
  \ available tags in one call and does not use pagination.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of results to return in a single call.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-tags-for-resource-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ListTagsForResourceInput
---
