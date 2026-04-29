---
description: Represents the output of a <code>PutActionRevision</code> action.
layout: schema
name: PutActionRevisionOutput
properties_list:
- description: ''
  name: newRevision
  type: object
- description: ''
  name: pipelineExecutionId
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-put-action-revision-output-schema.json
slug: amazon-codepipeline-put-action-revision-output
source_filename: amazon-codepipeline-put-action-revision-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-action-revision-output-schema.json\",\n  \"title\": \"PutActionRevisionOutput\",\n  \"description\": \"Represents the output of a <code>PutActionRevision</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"newRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether the artifact revision was previously used in an execution of the specified pipeline.\"\n        }\n      ]\n    },\n    \"pipelineExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionId\"\n        },\n        {\n          \"description\": \"The ID of the current workflow state of the pipeline.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-action-revision-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PutActionRevisionOutput
---
