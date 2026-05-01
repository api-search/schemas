---
description: The action engine, or executor, related to the supported integration model used to create and update the action type. The available executor types are <code>Lambda</code> and <code>JobWorker</code>.
layout: schema
name: ExecutorConfiguration
properties_list:
- description: ''
  name: lambdaExecutorConfiguration
  type: object
- description: ''
  name: jobWorkerExecutorConfiguration
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-executor-configuration-schema.json
slug: amazon-codepipeline-executor-configuration
source_filename: amazon-codepipeline-executor-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-executor-configuration-schema.json\",\n  \"title\": \"ExecutorConfiguration\",\n  \"description\": \"The action engine, or executor, related to the supported integration model used to create and update the action type. The available executor types are <code>Lambda</code> and <code>JobWorker</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lambdaExecutorConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaExecutorConfiguration\"\n        },\n        {\n          \"description\": \"Details about the <code>Lambda</code> executor of the action type.\"\n        }\n      ]\n    },\n    \"jobWorkerExecutorConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobWorkerExecutorConfiguration\"\
  \n        },\n        {\n          \"description\": \"Details about the <code>JobWorker</code> executor of the action type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-executor-configuration-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ExecutorConfiguration
---
