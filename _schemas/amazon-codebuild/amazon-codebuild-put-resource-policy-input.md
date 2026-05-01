---
description: PutResourcePolicyInput schema from Amazon CodeBuild
layout: schema
name: PutResourcePolicyInput
properties_list:
- description: ''
  name: policy
  type: object
- description: ''
  name: resourceArn
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-put-resource-policy-input-schema.json
slug: amazon-codebuild-put-resource-policy-input
source_filename: amazon-codebuild-put-resource-policy-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-put-resource-policy-input-schema.json\",\n  \"title\": \"PutResourcePolicyInput\",\n  \"description\": \"PutResourcePolicyInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" A JSON-formatted resource policy. For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/project-sharing.html#project-sharing-share\\\">Sharing a Project</a> and <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/report-groups-sharing.html#report-groups-sharing-share\\\">Sharing a Report Group</a> in the <i>CodeBuild User Guide</i>. \"\n        }\n      ]\n    },\n  \
  \  \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The ARN of the <code>Project</code> or <code>ReportGroup</code> resource you want to associate with a resource policy. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"policy\",\n    \"resourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-put-resource-policy-input-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: PutResourcePolicyInput
---
