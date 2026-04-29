---
description: PutWebhookInput schema from Amazon CodePipeline
layout: schema
name: PutWebhookInput
properties_list:
- description: ''
  name: webhook
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-put-webhook-input-schema.json
slug: amazon-codepipeline-put-webhook-input
source_filename: amazon-codepipeline-put-webhook-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-webhook-input-schema.json\",\n  \"title\": \"PutWebhookInput\",\n  \"description\": \"PutWebhookInput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webhook\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookDefinition\"\n        },\n        {\n          \"description\": \"The detail provided in an input file to create the webhook, such as the webhook name, the pipeline name, and the action name. Give the webhook a unique name that helps you identify it. You might name the webhook after the pipeline and action it targets so that you can easily recognize what it's used for later.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\
  \n        },\n        {\n          \"description\": \"The tags for the webhook.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"webhook\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-webhook-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PutWebhookInput
---
