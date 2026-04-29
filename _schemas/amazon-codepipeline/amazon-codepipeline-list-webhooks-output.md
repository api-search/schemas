---
description: ListWebhooksOutput schema from Amazon CodePipeline
layout: schema
name: ListWebhooksOutput
properties_list:
- description: ''
  name: webhooks
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-list-webhooks-output-schema.json
slug: amazon-codepipeline-list-webhooks-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-webhooks-output-schema.json\",\n  \"title\": \"ListWebhooksOutput\",\n  \"description\": \"ListWebhooksOutput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webhooks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookList\"\n        },\n        {\n          \"description\": \"The JSON detail returned for each webhook in the list output for the ListWebhooks call.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If the amount of returned information is significantly large, an identifier is also returned and can be used in a subsequent ListWebhooks call to return\
  \ the next set of webhooks in the list. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-webhooks-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ListWebhooksOutput
---
