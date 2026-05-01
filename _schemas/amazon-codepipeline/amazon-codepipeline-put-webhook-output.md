---
description: PutWebhookOutput schema from Amazon CodePipeline
layout: schema
name: PutWebhookOutput
properties_list:
- description: ''
  name: webhook
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-put-webhook-output-schema.json
slug: amazon-codepipeline-put-webhook-output
source_filename: amazon-codepipeline-put-webhook-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-webhook-output-schema.json\",\n  \"title\": \"PutWebhookOutput\",\n  \"description\": \"PutWebhookOutput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webhook\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListWebhookItem\"\n        },\n        {\n          \"description\": \"The detail returned from creating the webhook, such as the webhook name, webhook URL, and webhook ARN.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-webhook-output-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PutWebhookOutput
---
