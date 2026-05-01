---
description: ListWebhooksInput schema from Amazon CodePipeline
layout: schema
name: ListWebhooksInput
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-list-webhooks-input-schema.json
slug: amazon-codepipeline-list-webhooks-input
source_filename: amazon-codepipeline-list-webhooks-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-webhooks-input-schema.json\",\n  \"title\": \"ListWebhooksInput\",\n  \"description\": \"ListWebhooksInput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token that was returned from the previous ListWebhooks call, which can be used to return the next set of webhooks in the list.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of results to return in a single call. To retrieve the remaining results, make another call\
  \ with the returned nextToken value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-webhooks-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ListWebhooksInput
---
