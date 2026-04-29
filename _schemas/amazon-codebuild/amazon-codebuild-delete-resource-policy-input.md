---
description: DeleteResourcePolicyInput schema from Amazon CodeBuild
layout: schema
name: DeleteResourcePolicyInput
properties_list:
- description: ''
  name: resourceArn
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-delete-resource-policy-input-schema.json
slug: amazon-codebuild-delete-resource-policy-input
source_filename: amazon-codebuild-delete-resource-policy-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-delete-resource-policy-input-schema.json\",\n  \"title\": \"DeleteResourcePolicyInput\",\n  \"description\": \"DeleteResourcePolicyInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The ARN of the resource that is associated with the resource policy. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-delete-resource-policy-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: DeleteResourcePolicyInput
---
