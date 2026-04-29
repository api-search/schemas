---
description: DeleteWebhookInput schema from Amazon CodeBuild
layout: schema
name: DeleteWebhookInput
properties_list:
- description: ''
  name: projectName
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-delete-webhook-input-schema.json
slug: amazon-codebuild-delete-webhook-input
source_filename: amazon-codebuild-delete-webhook-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-delete-webhook-input-schema.json\",\n  \"title\": \"DeleteWebhookInput\",\n  \"description\": \"DeleteWebhookInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the CodeBuild project.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"projectName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-delete-webhook-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: DeleteWebhookInput
---
