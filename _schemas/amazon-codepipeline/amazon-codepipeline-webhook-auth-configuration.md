---
description: The authentication applied to incoming webhook trigger requests.
layout: schema
name: WebhookAuthConfiguration
properties_list:
- description: ''
  name: AllowedIPRange
  type: object
- description: ''
  name: SecretToken
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-webhook-auth-configuration-schema.json
slug: amazon-codepipeline-webhook-auth-configuration
source_filename: amazon-codepipeline-webhook-auth-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-webhook-auth-configuration-schema.json\",\n  \"title\": \"WebhookAuthConfiguration\",\n  \"description\": \"The authentication applied to incoming webhook trigger requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AllowedIPRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookAuthConfigurationAllowedIPRange\"\n        },\n        {\n          \"description\": \"The property used to configure acceptance of webhooks in an IP address range. For IP, only the <code>AllowedIPRange</code> property must be set. This property must be set to a valid CIDR range.\"\n        }\n      ]\n    },\n    \"SecretToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookAuthConfigurationSecretToken\"\n        },\n\
  \        {\n          \"description\": \"The property used to configure GitHub authentication. For GITHUB_HMAC, only the <code>SecretToken</code> property must be set.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-webhook-auth-configuration-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: WebhookAuthConfiguration
---
