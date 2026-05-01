---
description: Represents the output of a <code>ListPipelines</code> action.
layout: schema
name: ListPipelinesOutput
properties_list:
- description: ''
  name: pipelines
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-list-pipelines-output-schema.json
slug: amazon-codepipeline-list-pipelines-output
source_filename: amazon-codepipeline-list-pipelines-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-pipelines-output-schema.json\",\n  \"title\": \"ListPipelinesOutput\",\n  \"description\": \"Represents the output of a <code>ListPipelines</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelines\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineList\"\n        },\n        {\n          \"description\": \"The list of pipelines.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If the amount of returned information is significantly large, an identifier is also returned. It can be used in a subsequent list pipelines call to return the next set of pipelines in the list.\"\n  \
  \      }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-pipelines-output-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ListPipelinesOutput
---
