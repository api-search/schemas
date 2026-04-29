---
description: Represents information about a webhook and its definition.
layout: schema
name: WebhookDefinition
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: targetPipeline
  type: object
- description: ''
  name: targetAction
  type: object
- description: ''
  name: filters
  type: object
- description: ''
  name: authentication
  type: object
- description: ''
  name: authenticationConfiguration
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-webhook-definition-schema.json
slug: amazon-codepipeline-webhook-definition
source_filename: amazon-codepipeline-webhook-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-webhook-definition-schema.json\",\n  \"title\": \"WebhookDefinition\",\n  \"description\": \"Represents information about a webhook and its definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookName\"\n        },\n        {\n          \"description\": \"The name of the webhook.\"\n        }\n      ]\n    },\n    \"targetPipeline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline you want to connect to the webhook.\"\n        }\n      ]\n    },\n    \"targetAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionName\"\n\
  \        },\n        {\n          \"description\": \"The name of the action in a pipeline you want to connect to the webhook. The action must be from the source (first) stage of the pipeline.\"\n        }\n      ]\n    },\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookFilters\"\n        },\n        {\n          \"description\": \"A list of rules applied to the body/payload sent in the POST request to a webhook URL. All defined rules must pass for the request to be accepted and the pipeline started.\"\n        }\n      ]\n    },\n    \"authentication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookAuthenticationType\"\n        },\n        {\n          \"description\": \"<p>Supported options are GITHUB_HMAC, IP, and UNAUTHENTICATED.</p> <ul> <li> <p>For information about the authentication scheme implemented by GITHUB_HMAC, see <a href=\\\"https://developer.github.com/webhooks/securing/\\\">Securing\
  \ your webhooks</a> on the GitHub Developer website.</p> </li> <li> <p> IP rejects webhooks trigger requests unless they originate from an IP address in the IP range whitelisted in the authentication configuration.</p> </li> <li> <p> UNAUTHENTICATED accepts all webhook trigger requests regardless of origin.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"authenticationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookAuthConfiguration\"\n        },\n        {\n          \"description\": \"Properties that configure the authentication applied to incoming webhook trigger requests. The required properties depend on the authentication type. For GITHUB_HMAC, only the <code>SecretToken </code>property must be set. For IP, only the <code>AllowedIPRange </code>property must be set to a valid CIDR range. For UNAUTHENTICATED, no properties can be set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"targetPipeline\"\
  ,\n    \"targetAction\",\n    \"filters\",\n    \"authentication\",\n    \"authenticationConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-webhook-definition-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: WebhookDefinition
---
