---
description: CreateWebhookOutput schema from Amazon CodeBuild
layout: schema
name: CreateWebhookOutput
properties_list:
- description: ''
  name: webhook
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-create-webhook-output-schema.json
slug: amazon-codebuild-create-webhook-output
source_filename: amazon-codebuild-create-webhook-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-create-webhook-output-schema.json\",\n  \"title\": \"CreateWebhookOutput\",\n  \"description\": \"CreateWebhookOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webhook\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Webhook\"\n        },\n        {\n          \"description\": \"Information about a webhook that connects repository events to a build project in CodeBuild.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-create-webhook-output-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: CreateWebhookOutput
---
