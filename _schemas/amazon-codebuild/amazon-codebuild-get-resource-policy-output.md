---
description: GetResourcePolicyOutput schema from Amazon CodeBuild
layout: schema
name: GetResourcePolicyOutput
properties_list:
- description: ''
  name: policy
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-get-resource-policy-output-schema.json
slug: amazon-codebuild-get-resource-policy-output
source_filename: amazon-codebuild-get-resource-policy-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-get-resource-policy-output-schema.json\",\n  \"title\": \"GetResourcePolicyOutput\",\n  \"description\": \"GetResourcePolicyOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The resource policy for the resource identified by the input ARN parameter. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-get-resource-policy-output-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: GetResourcePolicyOutput
---
