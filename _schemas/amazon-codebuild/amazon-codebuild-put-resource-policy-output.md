---
description: PutResourcePolicyOutput schema from Amazon CodeBuild
layout: schema
name: PutResourcePolicyOutput
properties_list:
- description: ''
  name: resourceArn
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-put-resource-policy-output-schema.json
slug: amazon-codebuild-put-resource-policy-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-put-resource-policy-output-schema.json\",\n  \"title\": \"PutResourcePolicyOutput\",\n  \"description\": \"PutResourcePolicyOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The ARN of the <code>Project</code> or <code>ReportGroup</code> resource that is associated with a resource policy. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-put-resource-policy-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: PutResourcePolicyOutput
---
