---
description: Represents information about an error in CodePipeline.
layout: schema
name: ErrorDetails
properties_list:
- description: ''
  name: code
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-error-details-schema.json
slug: amazon-codepipeline-error-details
source_filename: amazon-codepipeline-error-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-error-details-schema.json\",\n  \"title\": \"ErrorDetails\",\n  \"description\": \"Represents information about an error in CodePipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Code\"\n        },\n        {\n          \"description\": \"The system ID or number code of the error.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"The text of the error message.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-error-details-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ErrorDetails
---
