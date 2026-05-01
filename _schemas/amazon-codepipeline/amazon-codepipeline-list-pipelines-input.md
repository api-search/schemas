---
description: Represents the input of a <code>ListPipelines</code> action.
layout: schema
name: ListPipelinesInput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-list-pipelines-input-schema.json
slug: amazon-codepipeline-list-pipelines-input
source_filename: amazon-codepipeline-list-pipelines-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-pipelines-input-schema.json\",\n  \"title\": \"ListPipelinesInput\",\n  \"description\": \"Represents the input of a <code>ListPipelines</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"An identifier that was returned from the previous list pipelines call. It can be used to return the next set of pipelines in the list.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxPipelines\"\n        },\n        {\n          \"description\": \"The maximum number of pipelines to return in a single call. To retrieve the remaining pipelines,\
  \ make another call with the returned nextToken value. The minimum value you can specify is 1. The maximum accepted value is 1000.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-pipelines-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ListPipelinesInput
---
