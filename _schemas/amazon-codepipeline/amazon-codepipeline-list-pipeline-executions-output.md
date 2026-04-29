---
description: Represents the output of a <code>ListPipelineExecutions</code> action.
layout: schema
name: ListPipelineExecutionsOutput
properties_list:
- description: ''
  name: pipelineExecutionSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-list-pipeline-executions-output-schema.json
slug: amazon-codepipeline-list-pipeline-executions-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-pipeline-executions-output-schema.json\",\n  \"title\": \"ListPipelineExecutionsOutput\",\n  \"description\": \"Represents the output of a <code>ListPipelineExecutions</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineExecutionSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionSummaryList\"\n        },\n        {\n          \"description\": \"A list of executions in the history of a pipeline.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that can be used in the next <code>ListPipelineExecutions</code> call. To view all items in the list, continue\
  \ to call this operation with each subsequent token until no more nextToken values are returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-pipeline-executions-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ListPipelineExecutionsOutput
---
