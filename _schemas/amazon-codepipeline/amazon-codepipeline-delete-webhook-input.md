---
description: DeleteWebhookInput schema from Amazon CodePipeline
layout: schema
name: DeleteWebhookInput
properties_list:
- description: ''
  name: name
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-delete-webhook-input-schema.json
slug: amazon-codepipeline-delete-webhook-input
source_filename: amazon-codepipeline-delete-webhook-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-delete-webhook-input-schema.json\",\n  \"title\": \"DeleteWebhookInput\",\n  \"description\": \"DeleteWebhookInput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookName\"\n        },\n        {\n          \"description\": \"The name of the webhook you want to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-delete-webhook-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: DeleteWebhookInput
---
