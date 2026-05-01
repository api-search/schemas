---
description: Represents the input of a <code>PutActionRevision</code> action.
layout: schema
name: PutActionRevisionInput
properties_list:
- description: ''
  name: pipelineName
  type: object
- description: ''
  name: stageName
  type: object
- description: ''
  name: actionName
  type: object
- description: ''
  name: actionRevision
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-put-action-revision-input-schema.json
slug: amazon-codepipeline-put-action-revision-input
source_filename: amazon-codepipeline-put-action-revision-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-action-revision-input-schema.json\",\n  \"title\": \"PutActionRevisionInput\",\n  \"description\": \"Represents the input of a <code>PutActionRevision</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline that starts processing the revision to the source.\"\n        }\n      ]\n    },\n    \"stageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageName\"\n        },\n        {\n          \"description\": \"The name of the stage that contains the action that acts on the revision.\"\n        }\n      ]\n    },\n    \"actionName\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionName\"\n        },\n        {\n          \"description\": \"The name of the action that processes the revision.\"\n        }\n      ]\n    },\n    \"actionRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionRevision\"\n        },\n        {\n          \"description\": \"Represents information about the version (or revision) of an action.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pipelineName\",\n    \"stageName\",\n    \"actionName\",\n    \"actionRevision\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-action-revision-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PutActionRevisionInput
---
