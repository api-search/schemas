---
description: Represents information about failure details.
layout: schema
name: FailureDetails
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: externalExecutionId
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-failure-details-schema.json
slug: amazon-codepipeline-failure-details
source_filename: amazon-codepipeline-failure-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-failure-details-schema.json\",\n  \"title\": \"FailureDetails\",\n  \"description\": \"Represents information about failure details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureType\"\n        },\n        {\n          \"description\": \"The type of the failure.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"The message about the failure.\"\n        }\n      ]\n    },\n    \"externalExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionId\"\n        },\n        {\n          \"description\": \"\
  The external ID of the run of the action that failed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-failure-details-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: FailureDetails
---
