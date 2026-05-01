---
description: Represents information about a stage to a job worker.
layout: schema
name: StageContext
properties_list:
- description: ''
  name: name
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-stage-context-schema.json
slug: amazon-codepipeline-stage-context
source_filename: amazon-codepipeline-stage-context-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stage-context-schema.json\",\n  \"title\": \"StageContext\",\n  \"description\": \"Represents information about a stage to a job worker.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageName\"\n        },\n        {\n          \"description\": \"The name of the stage.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stage-context-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: StageContext
---
