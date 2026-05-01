---
description: Additional information about a build phase that has an error. You can use this information for troubleshooting.
layout: schema
name: PhaseContext
properties_list:
- description: ''
  name: statusCode
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-phase-context-schema.json
slug: amazon-codebuild-phase-context
source_filename: amazon-codebuild-phase-context-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-phase-context-schema.json\",\n  \"title\": \"PhaseContext\",\n  \"description\": \"Additional information about a build phase that has an error. You can use this information for troubleshooting.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The status code for the context of the build phase.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An explanation of the build phase's context. This might include a command ID and an exit code.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-phase-context-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: PhaseContext
---
