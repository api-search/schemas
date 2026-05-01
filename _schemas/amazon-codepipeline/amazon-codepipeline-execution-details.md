---
description: The details of the actions taken and results produced on an artifact as it passes through stages in the pipeline.
layout: schema
name: ExecutionDetails
properties_list:
- description: ''
  name: summary
  type: object
- description: ''
  name: externalExecutionId
  type: object
- description: ''
  name: percentComplete
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-execution-details-schema.json
slug: amazon-codepipeline-execution-details
source_filename: amazon-codepipeline-execution-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-execution-details-schema.json\",\n  \"title\": \"ExecutionDetails\",\n  \"description\": \"The details of the actions taken and results produced on an artifact as it passes through stages in the pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"summary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionSummary\"\n        },\n        {\n          \"description\": \"The summary of the current status of the actions.\"\n        }\n      ]\n    },\n    \"externalExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionId\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of this action used to identify this job worker in any external systems, such as CodeDeploy.\"\
  \n        }\n      ]\n    },\n    \"percentComplete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The percentage of work completed on the action, represented on a scale of 0 to 100 percent.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-execution-details-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ExecutionDetails
---
