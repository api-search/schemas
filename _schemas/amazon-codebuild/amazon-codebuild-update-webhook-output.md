---
description: UpdateWebhookOutput schema from Amazon CodeBuild
layout: schema
name: UpdateWebhookOutput
properties_list:
- description: ''
  name: webhook
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-update-webhook-output-schema.json
slug: amazon-codebuild-update-webhook-output
source_filename: amazon-codebuild-update-webhook-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-update-webhook-output-schema.json\",\n  \"title\": \"UpdateWebhookOutput\",\n  \"description\": \"UpdateWebhookOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webhook\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Webhook\"\n        },\n        {\n          \"description\": \" Information about a repository's webhook that is associated with a project in CodeBuild. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-update-webhook-output-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: UpdateWebhookOutput
---
