---
description: The event criteria that specify when a webhook notification is sent to your URL.
layout: schema
name: WebhookFilterRule
properties_list:
- description: ''
  name: jsonPath
  type: object
- description: ''
  name: matchEquals
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-webhook-filter-rule-schema.json
slug: amazon-codepipeline-webhook-filter-rule
source_filename: amazon-codepipeline-webhook-filter-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-webhook-filter-rule-schema.json\",\n  \"title\": \"WebhookFilterRule\",\n  \"description\": \"The event criteria that specify when a webhook notification is sent to your URL.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jsonPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JsonPath\"\n        },\n        {\n          \"description\": \"A JsonPath expression that is applied to the body/payload of the webhook. The value selected by the JsonPath expression must match the value specified in the <code>MatchEquals</code> field. Otherwise, the request is ignored. For more information, see <a href=\\\"https://github.com/json-path/JsonPath\\\">Java JsonPath implementation</a> in GitHub.\"\n        }\n      ]\n    },\n    \"matchEquals\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchEquals\"\n        },\n        {\n          \"description\": \"The value selected by the <code>JsonPath</code> expression must match what is supplied in the <code>MatchEquals</code> field. Otherwise, the request is ignored. Properties from the target action configuration can be included as placeholders in this value by surrounding the action configuration key with curly brackets. For example, if the value supplied here is \\\"refs/heads/{Branch}\\\" and the target action has an action configuration property called \\\"Branch\\\" with a value of \\\"main\\\", the <code>MatchEquals</code> value is evaluated as \\\"refs/heads/main\\\". For a list of action configuration properties for built-in action types, see <a href=\\\"https://docs.aws.amazon.com/codepipeline/latest/userguide/reference-pipeline-structure.html#action-requirements\\\">Pipeline Structure Reference Action Requirements</a>.\"\n        }\n      ]\n\
  \    }\n  },\n  \"required\": [\n    \"jsonPath\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-webhook-filter-rule-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: WebhookFilterRule
---
