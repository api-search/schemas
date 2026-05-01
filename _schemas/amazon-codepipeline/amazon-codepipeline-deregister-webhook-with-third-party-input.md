---
description: DeregisterWebhookWithThirdPartyInput schema from Amazon CodePipeline
layout: schema
name: DeregisterWebhookWithThirdPartyInput
properties_list:
- description: ''
  name: webhookName
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-deregister-webhook-with-third-party-input-schema.json
slug: amazon-codepipeline-deregister-webhook-with-third-party-input
source_filename: amazon-codepipeline-deregister-webhook-with-third-party-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-deregister-webhook-with-third-party-input-schema.json\",\n  \"title\": \"DeregisterWebhookWithThirdPartyInput\",\n  \"description\": \"DeregisterWebhookWithThirdPartyInput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webhookName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookName\"\n        },\n        {\n          \"description\": \"The name of the webhook you want to deregister.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-deregister-webhook-with-third-party-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: DeregisterWebhookWithThirdPartyInput
---
