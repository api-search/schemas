---
description: Represents the output of an <code>UpdatePipeline</code> action.
layout: schema
name: UpdatePipelineOutput
properties_list:
- description: ''
  name: pipeline
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-update-pipeline-output-schema.json
slug: amazon-codepipeline-update-pipeline-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-update-pipeline-output-schema.json\",\n  \"title\": \"UpdatePipelineOutput\",\n  \"description\": \"Represents the output of an <code>UpdatePipeline</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineDeclaration\"\n        },\n        {\n          \"description\": \"The structure of the updated pipeline.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-update-pipeline-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: UpdatePipelineOutput
---
