---
description: ListTagsForResourceInput schema from Amazon Proton API
layout: schema
name: ListTagsForResourceInput
properties_list:
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: resourceArn
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-tags-for-resource-input-schema.json
slug: amazon-proton-list-tags-for-resource-input
source_filename: amazon-proton-list-tags-for-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-tags-for-resource-input-schema.json\",\n  \"title\": \"ListTagsForResourceInput\",\n  \"description\": \"ListTagsForResourceInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxPageResults\"\n        },\n        {\n          \"description\": \"The maximum number of tags to list.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next resource tag in the array of resource tags, after the list of resource tags that was previously requested.\"\n        }\n      ]\n    },\n    \"resourceArn\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource for the listed tags.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-tags-for-resource-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListTagsForResourceInput
---
