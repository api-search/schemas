---
description: Returns a summary of a pipeline.
layout: schema
name: PipelineSummary
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: updated
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-pipeline-summary-schema.json
slug: amazon-codepipeline-pipeline-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-summary-schema.json\",\n  \"title\": \"PipelineSummary\",\n  \"description\": \"Returns a summary of a pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineVersion\"\n        },\n        {\n          \"description\": \"The version number of the pipeline.\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and\
  \ time the pipeline was created, in timestamp format.\"\n        }\n      ]\n    },\n    \"updated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time of the last update to the pipeline, in timestamp format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-summary-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PipelineSummary
---
