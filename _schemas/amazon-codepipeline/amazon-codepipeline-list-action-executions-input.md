---
description: ListActionExecutionsInput schema from Amazon CodePipeline
layout: schema
name: ListActionExecutionsInput
properties_list:
- description: ''
  name: pipelineName
  type: object
- description: ''
  name: filter
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-list-action-executions-input-schema.json
slug: amazon-codepipeline-list-action-executions-input
source_filename: amazon-codepipeline-list-action-executions-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-action-executions-input-schema.json\",\n  \"title\": \"ListActionExecutionsInput\",\n  \"description\": \"ListActionExecutionsInput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \" The name of the pipeline for which you want to list action execution history.\"\n        }\n      ]\n    },\n    \"filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionExecutionFilter\"\n        },\n        {\n          \"description\": \"Input information used to filter action execution history.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of results to return in a single call. To retrieve the remaining results, make another call with the returned nextToken value. Action execution history is retained for up to 12 months, based on action execution start times. Default value is 100. </p> <note> <p>Detailed execution history is available for executions run on or after February 21, 2019.</p> </note>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token that was returned from the previous <code>ListActionExecutions</code> call, which can be used to return the next set of action executions in the list.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pipelineName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-action-executions-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ListActionExecutionsInput
---
