---
description: The action engine, or executor, for an action type created for a provider, where the action is to be used by customers of the provider. The action engine is associated with the model used to create and update the action, such as the Lambda integration model.
layout: schema
name: ActionTypeExecutor
properties_list:
- description: ''
  name: configuration
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: policyStatementsTemplate
  type: object
- description: ''
  name: jobTimeout
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-type-executor-schema.json
slug: amazon-codepipeline-action-type-executor
source_filename: amazon-codepipeline-action-type-executor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-executor-schema.json\",\n  \"title\": \"ActionTypeExecutor\",\n  \"description\": \"The action engine, or executor, for an action type created for a provider, where the action is to be used by customers of the provider. The action engine is associated with the model used to create and update the action, such as the Lambda integration model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutorConfiguration\"\n        },\n        {\n          \"description\": \"The action configuration properties for the action type. These properties are specified in the action definition when the action type is created.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ExecutorType\"\n        },\n        {\n          \"description\": \"The integration model used to create and update the action type, <code>Lambda</code> or <code>JobWorker</code>. \"\n        }\n      ]\n    },\n    \"policyStatementsTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyStatementsTemplate\"\n        },\n        {\n          \"description\": \"<p>The policy statement that specifies the permissions in the CodePipeline customer account that are needed to successfully run an action.</p> <p>To grant permission to another account, specify the account ID as the Principal, a domain-style identifier defined by the service, for example <code>codepipeline.amazonaws.com</code>.</p> <note> <p>The size of the passed JSON policy document cannot exceed 2048 characters.</p> </note>\"\n        }\n      ]\n    },\n    \"jobTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/JobTimeout\"\n        },\n        {\n          \"description\": \"The timeout in seconds for the job. An action execution can have multiple jobs. This is the timeout for a single job, not the entire action execution.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"configuration\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-executor-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionTypeExecutor
---
