---
description: RegisterWebhookWithThirdPartyInput schema from Amazon CodePipeline
layout: schema
name: RegisterWebhookWithThirdPartyInput
properties_list:
- description: ''
  name: webhookName
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-register-webhook-with-third-party-input-schema.json
slug: amazon-codepipeline-register-webhook-with-third-party-input
source_filename: amazon-codepipeline-register-webhook-with-third-party-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-register-webhook-with-third-party-input-schema.json\",\n  \"title\": \"RegisterWebhookWithThirdPartyInput\",\n  \"description\": \"RegisterWebhookWithThirdPartyInput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webhookName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookName\"\n        },\n        {\n          \"description\": \"The name of an existing webhook created with PutWebhook to register with a supported third party. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-register-webhook-with-third-party-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: RegisterWebhookWithThirdPartyInput
---
