---
description: The toolchain template file provided with the project request. AWS CodeStar uses the template to provision the toolchain stack in AWS CloudFormation.
layout: schema
name: Toolchain
properties_list:
- description: ''
  name: source
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: stackParameters
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-toolchain-schema.json
slug: codestar-toolchain
source_filename: codestar-toolchain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-toolchain-schema.json\",\n  \"title\": \"Toolchain\",\n  \"description\": \"The toolchain template file provided with the project request. AWS CodeStar uses the template to provision the toolchain stack in AWS CloudFormation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ToolchainSource\"\n        },\n        {\n          \"description\": \"The Amazon S3 location where the toolchain template file provided with the project request is stored. AWS CodeStar retrieves the file during project creation.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The service role\
  \ ARN for AWS CodeStar to use for the toolchain template during stack provisioning.\"\n        }\n      ]\n    },\n    \"stackParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateParameterMap\"\n        },\n        {\n          \"description\": \"The list of parameter overrides to be passed into the toolchain template during stack provisioning, if any.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-toolchain-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: Toolchain
---
